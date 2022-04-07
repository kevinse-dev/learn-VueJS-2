<template>
<div>
  <h2 v-if="num == 0" >The number is Zero</h2>
  <h2 v-else-if="num < 0" >The Number is Negative</h2>
  <h2 v-else-if="num > 0" >The Number is Positive</h2>
  <h2 v-else >not a Number</h2>

  <div v-if="!display">
  <h2>vishwas</h2> 
  <h2>codevolution</h2>
  <h2>Vue</h2>
  </div>


  <h2 v-show="showElement">using V-show</h2>
  <h2 v-if="showElement" >using v-if</h2>
</div>
</template>

<script>

export default {
  name:'app',
  data(){
    return{
      num: 'j',
      display:true,
      showElement:false
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
