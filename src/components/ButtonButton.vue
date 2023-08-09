<template> 
<button @click="onClick()" :style="{background: color}" class="btn">{{text}}</button>
</template>

<script>
export default {
    name: 'ButtonButton',
    props: {
        text: String,
        color: String
    },
    methods: {
        onclick(){
            console.log('click')
    },
}
}
</script>