<template>
  <div class="container">
    <button v-on:click="count++">You clicked me {{ count }} times.</button>
  </div>
</template>

<script>
export default {
  name: 'ButtonCounter',
  data: function() {
    return {
      count: 0,
    }
  }
}
</script>
<style scoped>
</style>