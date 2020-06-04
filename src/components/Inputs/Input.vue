<template>  
    <input type="text" v-bind:placeholder="placeholder" @change="handleChange" class="w-100 input">
</template>

<script>
    export default {
        name:"input",
        props:{
            handleChangee:Function,
            placeholder:String,
        },
        methods:{
            handleChange(event){
                this.handleChange(event.target.value)
            }
        }
    }
</script>

<style>

</style>