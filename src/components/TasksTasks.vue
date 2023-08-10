<template>
<div :key="Tasks.id" v-for="Tasks in Tasks">
    <TaskTask :task="Tasks"/>
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
    }
}
</script>