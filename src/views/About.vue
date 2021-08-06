<template>
    <div class="about-container">
        <h3>Version 1.0.3</h3>
        <p>Customized By Mike</p>
        <router-link to="/">Back</router-link>
    </div>
</template>
<script>
export default {
    name:'About',
    
}
</script>
<style scoped>
.about-container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: #f9f9f9;
    border-radius: 10px;
    padding: 20px;
    /* margin: 40px; */
}
.about-container a{
    color: #1b1bec;
    text-decoration: none;
}
</style>