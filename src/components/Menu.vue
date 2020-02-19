<template>
    <div class="redBorder">
        <a href="">Section 1</a>
        <a href="">Section 2</a>
        <a href="">Section 3</a>
        <a href="">Section 4</a>
    </div>
</template>

<script>
export default {
    name: 'Menu'
}
</script>

<style scoped>
    div{
        display: flex;
        justify-content: center;
        margin: 10px;
    }

    a{
        margin: 10px 20px;
    }
</style>