<template>
  <div id="app">
    <h2>Type in the box</h2>
    <input type="text" v-on:input="change">
    <p>{{msg}}</p>
  </div>
</template>





<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Here is the message'
    }
  },
  methods: {
    change: function(e) {
      this.msg = e.target.value;
    }
  }
}
</script>



<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a, h2 {
  color: #42b983;
}
</style>
