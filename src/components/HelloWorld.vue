<template>
  <div>
    <Header heading="This is a test">This goes in the slot</Header>
    <Paragraph />
    <Square v-if=square />
    <People v-bind:arrayPeople="['Tom', 'Harry', 'John']" />
    <Basket />
  </div>
</template>

<script>
import Header from './Header.vue'
import Paragraph from './Paragraph.vue'
import Square from './Square.vue'
import People from './People.vue'
import Basket from './Basket.vue'

export default {
  name: 'HelloWorld',
  components: {
    Header,
    Paragraph,
    Square,
    People,
    Basket
  },
  props: {
    square: {
      type: Boolean,
      default: true
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
