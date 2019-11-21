<template>
    <div>
        <input type="text" v-model="name">
        <input type="text" v-model="password">
        <button @click="login">登录成功去首页</button>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                name: "",
                password: "",
                msg: 12
            }
        },
        methods: {
            login() {
                if(!this.name || !this.password) {
                    alert('不能为空')
                    return
                }
                // 说明两个input都有值，可以调到首页
                console.log(this)
                // push是往浏览器历史记录栈内加入新的路由，可以后退回上一个路由
                this.$router.push('/home/' + this.msg)
                // replace 是替换当前路由，不会往栈内推送新的路由，所以回不到之前的页面
                // this.$router.replace('/home/' + this.msg)
            }
        },
    }
</script>

<style scoped>

</style>