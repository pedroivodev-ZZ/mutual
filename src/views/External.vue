<template>
    <div class="wrapper">
      <h1>Find stuff</h1>
      <SearchableList :items="items" />
   </div>
</template>
<script>
import SearchableList from '../components/SearchableList.vue'

export default {
  name: 'External',
  components: { SearchableList },
  data () {
    return {
      items: [
        { id: 1, name: 'Furadeira', quantity: 1, thumbnail: 'img/furadeira.jpg', donatorRating: 5 },
        { id: 1, name: 'Cobertor', quantity: 2, thumbnail: 'img/cobertores.jpg', donatorRating: 4 }
      ]
    }
  },
  methods: {

  }
}
</script>
<style scope lang="sass">
.wrapper
  padding: 0px 5px
</style>
