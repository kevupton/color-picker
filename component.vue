<template>
  <sketch-picker :value="value" @input="$emit('intput', $event)" />
</template>

<script>
module.exports = {
  components: {
    "sketch-picker": node_modules['vue-color'].Sketch
  },
  props: {
    value: {
      default: '',
      type: [String, Object]
    }
  },
};
</script>

<style>
</style>
