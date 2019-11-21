<template>
    <div>
        用户界面
        <br>
        <router-link to="account/login" tag="button">登录</router-link>
        <router-link to="account/register" tag="button">注册</router-link>


        <router-view/>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>

</style>