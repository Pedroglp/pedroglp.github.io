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
  border-radius: 50%;
  height: 30vh;
  margin-top: 4vh;
}

.avatar p{
  text-align: center;
  margin: 0.7vh 3vw;
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
  margin-top: -8px;
  margin-right: -8px;
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
  background-color: black;
  width: 50px;
  height: 50px;
  text-align: center;
  position: fixed;
  bottom: 5px;
  right: 5px;
  box-shadow: 5px 3px 5px rgba(0, 0, 0, 0.2);

}

.callme-icon{
  color: white;
  font-size: 1.6em;
  color: white;
  margin-top: 10px;
}

</style>
