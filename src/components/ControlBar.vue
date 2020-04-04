<template>
  <div class="control-bar">
    <button v-on:click="_clickIncrease">Increase</button>
    <button v-on:click="_clickDecrease">Decrease</button>
  </div>
</template>

<script>
export default {
  name: 'ControlBar',
  methods: {
    _clickIncrease() {
      this.$emit('clickIncrease');
    },
    _clickDecrease() {
      this.$emit('clickDecrease');
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
