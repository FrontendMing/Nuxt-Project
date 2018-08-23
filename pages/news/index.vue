<template>
  <div>
    <h2>About index news</h2>
    <p>NEWSID:{{$route.params.newsId}}</p>
    <ul>
      <li><nuxt-link :to="{name:'index'}">HOME</nuxt-link></li>
      <li><nuxt-link :to="{name:'news-id',params:{id:123,title:'new title'}}">news-1</nuxt-link></li>
      <li><nuxt-link :to="{name:'news-id',params:{id:mmm}}">news-2</nuxt-link></li>
    </ul>
  </div>
</template>

<script>
  export default {
    transition: 'test'
  }
</script>

<style scoped>

</style>