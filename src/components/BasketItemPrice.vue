<template>
  <td>
    {{ item.price }}
  </td>
</template>

<script>

export default {
  name: 'BasketItemPrice',
  props: {
    item: Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>