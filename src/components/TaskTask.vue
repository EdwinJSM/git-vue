<template>
    <div @dblclick="$emit('toggle-reminder',id)" :class="[task.reminder ? 'reminder' : '' , 'task']">
        <h3> {{ task.text }}
        <i @click="$emit('delete-task',task.id)"  class="fas fa-times"></i>
        </h3>
        <p> {{ task.day }} </p>
    </div>
    
</template>

<script>
export default{
    name: 'TaskTask',
    props: {
    task: Object
    }
}
</script>

<style scope>
.fas {
  color: red;
  align-items: end;
}

.TaskTask{
  background: #f4f4f4;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}

.task.reminder {
  border-left: 5px solid rgb(0, 0, 0);
}

.task h3 {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>