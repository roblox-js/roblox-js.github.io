<template>
  <div class="component-container" v-bind:class="rootClassName"></div>
</template>

<script>
export default {
  name: 'AppComponent',
  props: {
    rootClassName: String,
  },
}
</script>

<style scoped>
.component-container {
  width: 100%;
  height: 400px;
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
}
</style>
