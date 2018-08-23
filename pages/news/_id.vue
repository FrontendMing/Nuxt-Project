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
    validate({params}){
      return /^\d+$/.test(params.id);
    },
    data(){
      return {
        title: this.$route.params.title || 'seo'
      }
    },
    head(){
      return {
        title: this.title,
        meta: [
          {hid: 'description', name: 'news', content: 'this is news page'}
        ]
      }
    }
  }
</script>

<style scoped>

</style>