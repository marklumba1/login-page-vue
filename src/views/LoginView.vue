<template>
    <div class="login-container">   
        <div class="login-inner">
            <Login v-if="loginMode" @switch="handleSwitch"/> 
            <Registration v-else @switch="handleSwitch"/>
        </div>
        
    </div>
</template>

<script setup>
 import { ref } from "vue";
import Login from "../components/Login.vue"
 import Registration from "../components/Registration.vue"

 const loginMode = ref(true)
 const handleSwitch = () => {
    loginMode.value = !loginMode.value
 }
</script>

<style lang="scss" scoped>
@import "../assets/styles/variables";
    .login-container {
        height: 100vh;
        width: 100vw;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        .login-inner{
            min-width: 300px;
        }
        .signup{
                font-size: 10px;
            }
       
    }
    .img-container{
        background-color: red;
        width: 100px;
    }
</style>