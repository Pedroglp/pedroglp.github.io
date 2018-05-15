<template>
  <div class="hello animated fadeInUp">
    <div class = "language-menu" @click="changeLanguage()">{{language}}</div>
    <img class="avatar-bg" src="../assets/bg2.svg"/>
    <div class="avatar">
      <img src="../assets/eufb.jpg"/>
      <p>Pedro Gabriel</p>
      <p>{{content.avatar.role}}</p>
    </div>
    <div class="icons">
      <a href="https://www.github.com/pedroglp" class="fab fa-github-square icon" target="_blank"></a>
      <a href="https://www.linkedin.com/pedroglp" class="fab fa-linkedin icon" target="_blank"></a> 
      <a href="https://facebok.com/pedroglp" class="fab fa-facebook-square icon" target="_blank"></a>
      <a href="mailto:pedrogabriellancelloti@poli.ufrj.br" class="fas fa-envelope-square icon"></a>
    </div>
    <hr></hr>
    <carousel :perPage="1">
      <slide>
        <h1>
          {{content.about.title}}
        </h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
          Nunc maximus, nulla ut commodo sagittis, sapien dui mattis dui, non pulvinar lorem felis nec erat
        </p>
      </slide>
      <slide>
        <h1>
          {{content.experiences.title}}
        </h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
          Nunc maximus, nulla ut commodo sagittis, sapien dui mattis dui, non pulvinar lorem felis nec erat
        </p>
      </slide>
      <slide>
        <h1>
          {{content.skills.title}}
        </h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
          Nunc maximus, nulla ut commodo sagittis, sapien dui mattis dui, non pulvinar lorem felis nec erat
        </p>
      </slide>
    </carousel>
    <div class = "callme-box">
      <a  href="tel:+5521989106926" class="fas fa-phone icon callme-icon"></a>
    </div>
  </div>
</template>

<script>

import text from '../assets/translations'

export default {
  name: 'HelloWorld',
  data () {
    return {
      animation: '',
      language: 'EN',
      content: text['pt']
    }
  },
  methods:{
    changeLanguage(){
      if (this.language == 'EN') {
        this.language = 'PT';
        this.content = text['en'];
      }
      else{
        this.language = 'EN';
        this.content = text['pt']
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
