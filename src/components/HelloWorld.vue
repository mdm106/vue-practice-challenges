<template>
  <div>
    <Header heading="This is a test" />
    <Paragraph />
    <Square />
    <People v-bind:arrayPeople="['Tom', 'Harry', 'John']" />
  </div>
</template>

<script>
import Header from './Header.vue'
import Paragraph from './Paragraph.vue'
import Square from './Square.vue'
import People from './People.vue'

export default {
  name: 'HelloWorld',
  components: {
    Header,
    Paragraph,
    Square,
    People
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
