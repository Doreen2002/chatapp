<template>

  <HelloWorld v-for ="con in content" :key = "con.id" :title="con.title"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import {ref} from 'vue';

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  setup(){
    const content = ref([{
  id : 1, title: 'Test Title 1'
}, {
  id : 2, title: 'Test Title 2'
}])
return {content}
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
