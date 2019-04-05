<template>
    <div class="wrapper">
      <h1>Find stuff</h1>
      <button @click="test">Teste</button>
      <!-- :items="items"  -->
      <SearchableList />
   </div>
</template>
<script>
import SearchableList from '../components/SearchableList.vue'

export default {
  name: 'External',
  components: { SearchableList },
  methods: {
    test() {

    }
  }
}
</script>
<style scope lang="sass">
.wrapper
  padding: 0px 5px
</style>
