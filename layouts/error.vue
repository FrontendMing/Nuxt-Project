<template>
    <div>
        <h2 v-if="error.statusCode == 404">404页面，你需要的页面没有找到</h2>
        <h2 v-else>500页面，服务器错误</h2>
        <ul>
            <li><nuxt-link to="/">HOME</nuxt-link></li>
        </ul>
    </div>
</template>

<script>
    export default {
        props: ['error']
    }
</script>

<style scoped>

</style>