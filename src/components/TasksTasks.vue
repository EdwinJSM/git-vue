<template>
<div :key="Tasks.id" v-for="Tasks in Tasks">
    <TaskTask @toggle-reminder="$emit ('toggle-reminder', id)" @delete-task="$emit('delete-task', id)" :task="Tasks"/>
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
    emits:['delete-task', 'toggle-reminder'],
    
}
</script>