<template>
  <div>
    <Header heading="This is a test" />
    <Paragraph text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quamquam tu hanc copiosiorem etiam soles dicere. Ubi ut eam caperet aut quando? Videmus igitur ut conquiescere ne infantes quidem possint. Magna laus. Bonum patria: miserum exilium. Sed tu istuc dixti bene Latine, parum plane. Duo Reges: constructio interrete. Ergo hoc quidem apparet, nos ad agendum esse natos" />
    <Square />
  </div>
</template>

<script>
import Header from './Header.vue'
import Paragraph from './Paragraph.vue'
import Square from './Square.vue'

export default {
  name: 'HelloWorld',
  components: {
    Header,
    Paragraph,
    Square
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
