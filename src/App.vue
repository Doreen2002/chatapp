<template>
<div :style="{fontSize:fontSize + 'em'}">
  <HelloWorld v-for ="con in content" :key = "con.id" :title="con.title" @enlarge-text="fontSize+=1"/>
</div>
  
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
const fontSize = ref(0)
return {content, fontSize}
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
