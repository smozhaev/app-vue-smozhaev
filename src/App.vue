<template>
  <div>
    <div v-for="comment in comments" :key="comment">
      <p>{{comment.id}}</p>
    </div>
    <ComentsBlock></ComentsBlock>
  </div>
  
</template>

<script>
import ComentsBlock from './components/ComentsBlock.vue'

export default {
  name: 'App',
  components: {
    ComentsBlock
  },
  data() {
    return {
      comments: [
        {id:1, text:"lorem"},
        {id:2,text:"lorem"},
        {id:3,text:"lorem"},
        {id:4,text:"lorem"},
        {id:5,text:"lorem"},
        {id:6,text:"lorem"},
      ] 
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
