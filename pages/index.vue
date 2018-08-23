<template>
  <div>
    <div class="img">
      <img src="~static/favicon.jpg" alt="">
    </div>
    <ul>
      <li><nuxt-link :to="{name:'index'}">HOME</nuxt-link></li>
      <li><nuxt-link :to="{name:'about'}">ABOUT</nuxt-link></li>
      <li><nuxt-link :to="{name:'news',params:{newsId:'3306'}}">NEWS</nuxt-link></li>
      <li><nuxt-link :to="{name:'asyncData'}">asyncData</nuxt-link></li>
    </ul>
  </div>
</template>

<script>
export default {
  
}
</script>

<style>
.img{
  width: 300px;
  height: 300px;
  background: url(~static/favicon.jpg)
}
</style>
erate
