<template>
<div :key="Tasks.id" v-for="Tasks in Tasks">
    <TaskTask @delete-task="$emit('deleteTask', task.id)" 
    :task="Tasks"/>
</div>
</template>

<script>
import TaskTask from './TaskTask.vue';
export default{
    name: 'TasksTasks',
    props :{
        Tasks: Array
    },
    components : {
        TaskTask
    },
    emits:['deletetask'],
    
}
</script>