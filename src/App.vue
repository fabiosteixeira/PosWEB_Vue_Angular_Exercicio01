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
          {id: 1, text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. In a mi egestas, consectetur ante sed, ornare sem. Quisque posuere pharetra elementum. Phasellus eget neque nulla. Donec ultrices sapien mi, non bibendum massa luctus sit amet. Aenean ultricies orci non nisi fringilla auctor. Nam efficitur volutpat interdum. Nam aliquam nisi eu tellus vehicula tempus. Aliquam at tempor felis, in cursus purus.', imgPath: 'logo.png'},
          {id: 2, text: 'Praesent ante sem, commodo egestas congue at, tempus nec magna. Nam facilisis aliquet sapien vitae porttitor. Sed quis lectus sit amet neque tristique fringilla. Proin accumsan molestie pretium. Pellentesque finibus purus at molestie hendrerit. In vel sollicitudin diam, ut malesuada est. Donec dictum metus vitae lobortis hendrerit. Proin ac tempor enim, eu mollis libero. Pellentesque volutpat tempor fringilla.', imgPath: 'logo.png'},
          {id: 3, text: 'Cras condimentum dui tellus. Ut eget lacus quis mi tincidunt convallis. Pellentesque nec erat dui. Vivamus aliquet accumsan pharetra. Mauris tempus vel velit sit amet eleifend. Aliquam in pulvinar erat, non aliquet orci. Etiam cursus, ligula maximus tristique tempor, diam nulla gravida felis, id molestie ex felis eu nisi. Sed ante orci, vehicula ac sem id, scelerisque rutrum velit. Quisque ipsum dui, commodo sit amet nunc eget, mollis egestas elit. Pellentesque pulvinar ligula eu metus gravida, eget ullamcorper lorem maximus. Aliquam erat massa, vulputate quis mattis lobortis, sagittis ut magna. Quisque a felis ac ante luctus tempus non faucibus ipsum. Curabitur dignissim felis neque, a faucibus ante luctus non. Maecenas varius justo sem. Vestibulum augue odio, iaculis sodales egestas eu, fermentum vel felis.', imgPath: 'logo.png'}
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
