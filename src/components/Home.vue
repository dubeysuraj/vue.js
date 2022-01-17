<template>
    <div class="Home">
        <h1>Home Component</h1>
        <Users />
        <Products />
    </div>
    
</template>

<script>
import Users from './Users.vue'
import Products from './Products.vue'
export default {
    name: 'Home',
    components:{
        Users,
        Products,
    }
}
</script>

<style scoped>
    .Home{
        background-color: rgb(236, 145, 145) ;
        height: 500px;
    }
</style>