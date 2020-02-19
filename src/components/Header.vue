<template>
    <div class="principal redBorder">
        <div>
            <img src="../assets/logo.png" alt="logo">
        </div>     
        <div class="menuDireito">
            <a href="">Topic 1</a>
            <a href="">Topic 2</a>
            <a href="">Topic 3</a>
            <a href="">Topic 4</a>
            <div class="search">
                <input type="text" placeholder="Buscar...">
            </div>            
        </div>                 
    </div>
</template>

<script>
export default {    
    name: 'Header'
}
</script>

<style scoped>
    .principal{
        display: flex;            
        justify-content: space-between;
        align-items: flex-start;
    }

    .menuDireito{
        margin-top: 20px;
    }

    a {
        margin: 0px 20px;
    }

    .search{
        display: flex;
        justify-content: flex-end;
        margin: 30px 20px;
    }

    input{
        flex: 1;
    }
</style>