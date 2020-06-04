<template>
        <div v-bind:class="classModal">
            <div class="row h-100">
                <transition name="slide-fade">
                    <div 
                        class="
                            col-0 col-sm-0 col-md-6  
                            border-right 
                            d-none d-sm-none d-md-block 
                            p-0
                            " 
                        v-if="isShowingContent"
                    >
                        <info/>
                    </div>
                </transition>
                <transition name="slide-fade">
                    <div 
                        class="
                            d-flex col-12 col-sm-12 col-md-6 col-lg-6 
                            align-items-center
                            " 
                        v-if="isShowingContent"
                    >
                        <login/>
                    </div>
                </transition>
            </div>
        </div>
</template>

<script>
    import login from '../Forms/Login'
    import info from '../Modal/Info/Info'
    export default {
        data(){
            return {
                classModal: ["white-model"],
                isShowingContent:false
            }
        },
        components:{
            login,
            info,
        },
        created(){
            function loadComponent(){
                setTimeout(
                    ()=> this.isShowingContent = true
                ,1300)
            }

            setTimeout(
                ()=> {
                    this.classModal.push("white-model-expand")
                    loadComponent.bind(this)()
                }
            ,400)
        },
    }
</script>