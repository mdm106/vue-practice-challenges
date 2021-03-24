<template>
  <div>
    <ul v-if="people.length > 0">
      <li v-for="person in people" :key="person.index">
        {{ person }}
      </li>
    </ul>
    <p v-else>Nothing to see here</p>
    <label for="addname">New Name:</label>
    <input type="text" id="addname" name="addname" v-model="newName">
    <button @click="addName">Add name</button>
  </div>
</template>

<script>

export default {
  name: 'People',
  props: {
    arrayPeople: {
      type: Array,
      default: () => []
    },
  },
  data: function() {
    return {
      people: [...this.arrayPeople],
      newName: ''
    }
  },
  methods: {
    addName() {
      this.people.push(this.newName);
      
      this.newName = '';
      }			
}

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
