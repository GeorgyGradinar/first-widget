<template>
  <div class="home">
    <h1>test</h1>
    <p>{{number}}</p>
    <button @click="number++">+</button>
    <button @click="number--">-</button>
    <Msg :msg="text"></Msg>
  </div>

</template>

<script>

import Msg from '@/components/MsgComp'
export default {
  name: 'App',

  data() {
    return {
      number:0,
      text: ''
    }
  },

  components: {Msg},

}
</script>

<style>
#widget {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
