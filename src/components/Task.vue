<template>
    <div @dblclick="$emit('toggle-reminder',task.id)" :class="[task.reminder ? 'reminder':'','task']">
        <h3>{{task.text}}
            <i @click="$emit('delete-task',task.id)" class="fas fa-trash"></i>
        </h3>
        <p>{{task.day}}</p>
    </div>
</template>
<script>
export default {
    name:"Task",
    props:{
        task:Object
    }
}
</script>
<style scoped>
.fas{
    color: #e20000;
}
.task{
    background: #f9f9f9;
    margin: 10px;
    padding: 10px 20px;
    cursor: pointer;
    border-radius: 10px;
}
.reminder{
    border-left: 5px solid #3fb27f;
}
.task h3{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
</style>