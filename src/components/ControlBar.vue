<template>
  <div class="control-bar">
    <button v-on:click="clickIncrease">Increase</button>
    <button v-on:click="clickDecrease">Decrease</button>
  </div>
</template>

<script>
export default {
  name: 'ControlBar',
  methods: {
    clickIncrease() {
      this.$emit('clickButton', 1);
    },
    clickDecrease() {
      this.$emit('clickButton', -1);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
