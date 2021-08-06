<template>
    <footer>
        <p>Copyrights Reserved &copy; 2021</p>
        <!-- <a href="/about">about</a> -->
        <router-link v-show="aboutPage" to="/about">about</router-link>
    </footer>
</template>
<script>
export default {
    name:"Footer",
    computed:{
        aboutPage(){
            if(this.$route.path === '/about'){
                return false
            }else{
                return true
            }
        }
    }
}
</script>
<style scoped>
footer{
    background: #f9f9f9;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 40px;
    padding: 10px;
    color: rgb(70, 70, 70);
    border-radius: 10px;
}
footer a{
    color: #1b1bec;
    text-decoration: none;
}
</style>