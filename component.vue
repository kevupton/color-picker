<template>  
  <div>
    <h3 v-if="meta.label">{{ meta.label }}</h3>
    <sketch-picker :value="value" @input="$emit('input', $event)" />
  </div>
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
    },
    meta: Object,
  },
};
</script>

<style>
</style>
