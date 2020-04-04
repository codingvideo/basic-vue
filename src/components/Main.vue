<template>
  <div class="main">
    <p>{{ count }}</p>
    <ControlBar v-on:clickIncrease="clickIncrease" v-on:clickDecrease="clickDecrease"></ControlBar>
  </div>
</template>

<script>
import ControlBar from './ControlBar.vue'

export default {
  name: 'HelloWorld',
  components: {
    ControlBar
  },
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
