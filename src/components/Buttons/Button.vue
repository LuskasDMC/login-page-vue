<template>
    <div>
        <button  class="button-default w-100"><b>{{text}}</b></button>
    </div>
</template>

<script>
    export default {
        props:{
            text:String,
        }
    }   
</script>