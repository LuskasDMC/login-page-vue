<template>
    <div class="row border rounded p-1">
        <div class="col-4">
            <img v-bind:src="image" class="icon">
        </div>
        <div v-bind:style="{color: color,fontSize:'.9rem',fontFamily:'Roboto, sans-serif'}"  class="col-8 d-flex justify-content-center align-items-center">
            <a href="#" style="text-decoration:none;color:inherit;">{{text}}</a>
        </div>
    </div>
</template>

<script>
    export default {
        props:{
            text:String,
            image:String,
            color:String
        },
    }
</script>