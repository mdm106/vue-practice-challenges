<template>
  <td>
    {{ item.name }}
  </td>
</template>

<script>

export default {
  name: 'BasketItemName',
  props: {
    item: Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>