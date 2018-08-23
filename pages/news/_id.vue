<template>
  <div>
    <h2>News-content</h2>
    <p>newsId:{{$route.params.id}}</p>
    <ul>
      <li><nuxt-link :to="{name:'news'}">NEWS</nuxt-link></li>
    </ul>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

</style>