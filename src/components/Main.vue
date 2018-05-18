<template>
  <div class="hello animated fadeInUp">
    <div class = "language-menu" @click="changeLanguage()">{{language}}</div>
    <img class="avatar-bg" src="../assets/bg2.svg"/>
    <img class="avatar-bg-lg" src="../assets/bg4.svg"/>
    <div class="avatar">
      <img src="../assets/eufb.jpg"/>
      <p>Pedro Gabriel</p>
      <p>{{content.avatar.role}}</p>
    </div>
    <div class="icons">
      <a href="https://www.github.com/pedroglp" class="fab fa-github-square icon" target="_blank"></a>
      <a href="https://www.linkedin.com/in/pedroglp/" class="fab fa-linkedin icon" target="_blank"></a> 
      <a href="https://facebok.com/pedroglp" class="fab fa-facebook-square icon" target="_blank"></a>
      <a href="mailto:pedrogabriellancelloti@poli.ufrj.br" class="fas fa-envelope-square icon"></a>
    </div>
    <hr></hr>
    <carousel :perPage="1" :minSwipeDistance="13">
      <slide>
        <h1>
          <div v-html="content.about.title"></div>
        </h1>
          <div class="paragraph" v-html="content.about.text"></div>
      </slide>
      <slide>
        <h1>
          <div v-html="content.experiences.title"></div>
        </h1>
          <div class="paragraph" v-html="content.experiences.text"></div>
      </slide>
      <slide>
        <h1>
          <div v-html="content.skills.title"></div>
        </h1>
          <div class="paragraph" v-html="content.skills.text"></div>
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
