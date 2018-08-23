<template>
    <div>
        <h1>姓名：{{info.name}}</h1>
        <h1>年龄：{{info.age}}</h1>
        <h1>兴趣：{{info.interest}}</h1>
    </div>
</template>

<script>
    import axios from 'axios'
    export default {
        data(){
            return {
                name: '11111'
            }
        },
        // asyncData(){
        //     return axios.get('https://api.myjson.com/bins/l14co')
        //                 .then(res => {
        //                     return {info: res.data}
        //                 })
        // }
        async asyncData(){
            let {data} = await axios.get('https://api.myjson.com/bins/l14co')
            return {info: data}
        }
    }
</script>

<style scoped>

</style>