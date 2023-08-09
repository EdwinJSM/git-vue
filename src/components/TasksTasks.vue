<template>
<div :key="Tasks.id" v-for="Tasks in Tasks">
    <h3>{{ Tasks.text }}</h3>
</div>
</template>

<script>
export default{
    name: 'TasksTasks',
    props :{
        Tasks: Array,
    }
}
</script>