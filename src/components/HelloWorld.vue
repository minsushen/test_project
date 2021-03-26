<template>
  <div class="hello">
    <input type="text" v-model="name">
    <ul>
      <li v-for="(cat, index) in cats" :key="index">{{cat.name}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      name: 'Luna the Destroyer of Dogs',
      cats: [
        {name: 'Simba', age: 11},
        {name: 'Robin', age: 5},
        {name: 'Luna', age: 9},
        {name: 'Cracker', age: 6},
        {name: 'Pig', age: 3}
      ]
    }
  },
  created() {
    console.log('111')
    console.log('222')
    console.log('333')
    console.log('444')
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
