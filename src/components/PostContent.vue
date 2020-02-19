<template>
    <ul id="example-1">
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

</style>