<template>
    <ul id="postList">
      <li v-for="item in items" v-bind:key="item.id">
        <Post
          :post="item"
        />
      </li>
    </ul>
</template>

<script>
import Post from './Post'
export default {
    name: 'PostContent',
    props: {
      items: Array
    },
    components: {
      Post
    }
}
</script>

<style scoped>
  ul {
    list-style-type: none;
    margin: 10px;
    padding: 0px;
  }

  li{
    margin-bottom: 10px;
  }
</style>