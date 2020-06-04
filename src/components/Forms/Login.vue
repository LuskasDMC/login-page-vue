<template>
    <div class="row justify-content-center">
        <img src="images/avatar.webp" class="rounded-circle w-25 d-block">
        <span class="w-100"/>
        <div class="col-6 pt-4">
            <div><Input placeholder="E-mail"/></div> 
            <div class="pt-3"><Input placeholder="Senha"/></div> 
            <div class="pt-3"><Button text="Login"/></div>
            <div class="row pt-3 justify-content-center">
                <p class="text-center text-dark w-100 font-weight-bold" >Or login with</p>
                <div class="col-8 col-sm-7 col-md-9 col-lg-6">
                    <Card text="Facebook" image="images/faceLogo.png" color="#4169E1"/>
                </div>
                <div class="col-8 col-sm-7 col-md-9 col-lg-6">
                    <Card text="Google" image="images/googleLogo.png"  color="#B22222"/>
                </div>
            </div>
        </div>
        <p class="text-center" id="register-question">Ainda não é registrado? <u>Clique aqui</u></p>
    </div>
</template>

<script>
    import Input from "../Inputs/Input"
    import Button from "../Buttons/Button"
    import Card from "../Cards/OtherLogin"
    export default {
        components:{
            Input,
            Button,
            Card
        }
    }
</script>