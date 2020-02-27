<template>
    <div class="redBorder">
        <div>
            {{post.title}}
        </div>
        <div class="container">
            <div>
                <img :src="getImgUrl(post.imgPath)" alt="">
            </div>
            <div>
                <div>{{post.text}}</div>
                <div>{{post.imgPath}}</div>
            </div>
        </div>
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

<style scoped>
    .container {
        display: flex;
        align-items: center;
    }

    img{
        padding: 10px;
    }
</style>