<template>
  <p>{{ text }}</p>
</template>

<script>

export default {
  name: 'Paragraph',
  props: {
    text: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p {
  margin: 20px;
}
</style>
