<template>
  <div>
    <h1>{{ heading }}</h1>
    <h2><slot></slot></h2>
  </div>
</template>

<script>

export default {
  name: 'Header',
  props: {
    heading: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  margin: 40px 0 0;
}
</style>
