<template>
    <div>
        我是购物车aaa
    </div>
</template>

<script>
    export default {
        created() {
            console.log(this)
            console.log(this.$route.query.id)
        }
    }
</script>

<style scoped>

</style>