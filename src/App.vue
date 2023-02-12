<script>
import Post from './Post.vue'
    export default {
      data() {
        return {
          amount: 1
        }
      },
      components:{
        Post
      },
      methods: {
        addPost(){
          this.amount++
        }
      }
    }
</script>

<template>
    <input type="button" value="Add post" @click="addPost">
    <Post v-for="n in amount" :key="n"/>
</template>

<style scoped>
</style>