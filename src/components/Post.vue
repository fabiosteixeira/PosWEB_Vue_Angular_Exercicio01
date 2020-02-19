<template>
    <div>
        <img :src="getImgUrl(post.imgPath)" alt="">
        <div>{{post.text}}</div>
        <div>{{post.imgPath}}</div>
    </div>
</template>

<script>
export default {
    name: 'Post',
    props: {
        post: Object
    }, 
    methods:{
        getImgUrl(path) {
            return require('../assets/'+path)
        }
    }
}
</script>