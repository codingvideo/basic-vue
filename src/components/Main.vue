<template>
  <div class="main">
    <p>{{ count }}</p>
    <button v-on:click="clickIncrease">Increase</button>
    <button v-on:click="clickDecrease">Decrease</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      count: 0
    }
  },
  methods: {
    clickIncrease() {
      this.count++;
    },
    clickDecrease() {
      this.count--;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
