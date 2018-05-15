<template>
  <div id="app">
    <Main/>
  </div>
</template>

<script>
import Main from './components/Main'

export default {
  name: 'App',
  components: {
    Main
  }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro');
@import url('https://fonts.googleapis.com/css?family=Montserrat');
@import 'assets/css/animate.css';

body{
  margin: 0 0 0 0;
}

#app {
  font-family: 'Montserrat', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #484848;
}

.icons{
  font-size: 1.6em;
  padding: 0 7px;
}

.icon {
  margin: 1.5vh 6px 0;
  text-decoration: none;
  color: #484848;
}

.avatar > img {
  position: relative;
  border-radius: 50%;
  height: 30vh;
  margin-top: 4vh;
  z-index: 2;
}

.avatar p{
  text-align: center;
  margin: 0.7vh 3vw;
}

.avatar-bg{
  z-index: 0;
  position: absolute;
  top: 0;
  left: 0;
  margin-left: auto;
  margin-right: auto;
  width: 100vw;

}

.language-menu{
  text-align: center; 
  color:white;
  background-color: #484848;
  width: 30px;
  position: absolute;
  top: 0;
  right: 0;
  cursor: pointer;
  z-index: 1;
  border: solid white 2px;
  border-top: 0px;
  border-right: 0px;
}

h1 {
  font-family: 'Source Sans Pro', Helvetica, Arial, sans-serif;
  font-weight: bold !important;
  margin-top:0 !important;
  color: black;
}

h2 {
  margin: 2.5vh 0vh;
}

hr {
  margin: 2.5vh 3vw;
  color: #bdbdbd;
}

p {
  text-align: justify;
  text-justify: inter-word;
  margin: 2.5vh 3vw;
}

.callme-box {
  z-index: 1;
  border-radius: 50%;
  background-color: #484848;
  width: 50px;
  height: 50px;
  text-align: center;
  position: fixed;
  bottom: 5px;
  right: 25px;
  box-shadow: 5px 3px 5px rgba(0, 0, 0, 0.2);
}

.callme-icon{
  color: white;
  font-size: 1.6em;
  margin-top: 10px;
}

.avatar-bg-lg {
  z-index: 0;
  position: absolute;
  top: 0;
  left: 0;
  margin-left: auto;
  margin-right: auto;
  width: 100vw;
  max-width: 100%;
  display: none;
}

@media (min-width: 768px) { 
  .lg {
    display: inline;
  }

  .callme-box {
    display: none;
  }

  .avatar > img {
    position: relative;
    border-radius: 50%;
    height: 40vh;
    margin-top: 20vh;
    z-index: 2;
  }

  .avatar p{
    font-size: 1.4em;
  }

  .avatar-bg {
    display: none;
  }

  .avatar-bg-lg {
    display: inline;
  }

  .icons{
    font-size: 2em;
    padding: 0 7px;
  }

  hr {
    margin: 2.5vh 6vw;
    color: #bdbdbd;
  }

  h1 {
    font-size: 3.0em;
  }

  p {
    margin: 2.5vh 6vw;
    font-size: 1.4em;
  }

}

</style>
