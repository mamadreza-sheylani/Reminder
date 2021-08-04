<template>
    <header>
        <h1>{{title}}</h1>
        <Button @button-click="$emit('toggle-add-task')" :text="showAddTask?'cancel':'Add Task'" :color="showAddTask?'red':'#3fb27f'" />
    </header>
</template>
<script>
import Button from './Button'
export default {
    name:'Header',
    components:{
        Button
    },
    props:{
        title:String,
        showAddTask:Boolean
    }
}
</script>
<style scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>