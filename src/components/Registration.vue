<template>
    <div class="register-container">
        <p>Registration Form</p>
        <div class="input-container">
            <input type="text" placeholder="Username">
            <input type="password" placeholder="Password">
            <input type="password" placeholder="Confirm Password">
        </div>
        <button>Register</button>
        <p class="bottom-link">Back to <span class="link" @click="$emit('switch')">Login</span></p>
    </div>
   
</template>

<script>
   
</script>

<style lang="scss" scoped>
@import "../assets/styles/variables";
@import "../assets/styles/mixins";
    .register-container{
        @include form;
    }
</style>