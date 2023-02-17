<template>
    <div class="login-form-container">
        <h1>Login Page</h1>
        <p>Welcome back!</p>
        <div class="input-container">
            <input type="text" placeholder="Username">
            <input type="password" placeholder="Password">
        </div>
        <button>Login</button>
        <p class="bottom-link">Dont have an account? <span class="link" @click="$emit('switch')">Sign Up</span></p>
    </div>
   
   
</template>

<script>
  
</script>

<style lang="scss" scoped>
@import "../assets/styles/variables";
@import "../assets/styles/mixins";

.login-form-container{
    @include form;  
}


       
</style>