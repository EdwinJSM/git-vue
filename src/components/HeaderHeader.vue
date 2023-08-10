<template>
   <header>
    <h1> {{ title }}</h1>
    <ButtonButton text="Add" color=" Green"/>
    <ButtonButton text="Delete" color="Red"/>
    <ButtonButton text="Update" color="Blue"/>
   </header>
</template>

<script>
import ButtonButton from './ButtonButton.vue';

 export default{
    name: 'HeaderHeader',
    props: {
        title: String,
    },
    components: { 
        ButtonButton 
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