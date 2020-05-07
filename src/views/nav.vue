<template>
    <nav>
        <router-link to="/" > HOME </router-link>
        <router-link to="/mywork" > MY WORK </router-link>
        <router-link to="/about" > ABOUT </router-link>
        <router-link to="/contact" > CONTACT </router-link>  
    </nav>

</template>

<script>
    export default {
        
    }
</script>

<style scoped>
nav {
    height: 49px;
    padding: 10px;
    text-align: center;
    font-family: 'Raleway', sans-serif;   
}

a {
    padding:10px;
    text-decoration: none;
}




</style>