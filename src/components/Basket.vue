<template>
  <div>
    <table v-if="basketItems" className="table table-bordered">
    <thead>
        <tr>
            <th>Name</th>
            <th>Price</th> 
        </tr>  
    </thead> 
    <tbody>
        <tr v-for="item in basketItems" :key="item.name">
            <BasketItemName v-bind:item="item" />
            <BasketItemPrice v-bind:item="item" />
        </tr>
    </tbody>
    </table>
    <p v-else >Nothing on the list</p>
    </div>
</template>

<script>
import BasketItemName from './BasketItemName.vue'
import BasketItemPrice from './BasketItemPrice.vue'

export default {
  name: 'Basket',
  components: {
    BasketItemName,
    BasketItemPrice
  },
  props: {
    items: {
      type: Array,
      default: () => [ { name: "Coffee", price: 2.10 },
                { name: "Bananas", price: 3.50 },
                { name: "Milk", price: 250.65 },
                { name: "The Great Milk Shortage by Simon Schama", price: 12.99 },]   
    },
  },
  data: function() {
    return {
      basketItems: [...this.items]
    }
  },
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>