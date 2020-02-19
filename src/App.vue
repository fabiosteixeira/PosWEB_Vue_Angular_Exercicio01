<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld mg="Welcome to Your Vue.js App"/> -->
    <Header/>
    <div class="redBorder">
      <Menu/>
    </div>
    <div class="redBorder">
      <PostContent
        :items="listPost"
      />
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Menu from './components/Menu.vue'
import PostContent from './components/PostContent'

export default {
  name: 'App',
  data(){
      return {
        listPost: [
          {id: 1, text: 'Primeiro post', imgPath: 'logo.png'},
          {id: 2, text: 'Segundo post', imgPath: 'logo.png'},
          {id: 3, text: 'Terceiro post', imgPath: 'logo.png'}
        ]
      } 
  },
  components: {
    // HelloWorld
    Header, 
    Menu,
    PostContent
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
