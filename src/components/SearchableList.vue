<template>
    <div>
        <div class="search-box">
            <input type="text" value="FGDFGDFafasfdasf">
            <button>Pesquisar</button>
        </div>
         <!-- :items="items" -->
        <List />
    </div>
</template>
<script lang="ts">
import List from './List.vue';

export default {
    name: 'SearchableList',
    components: { List }
}
</script>

<style lang="sass" scoped>
.search-box
    display: flex
    height: 30px

    input[type='text']
        font-size: 16px
        border-radius: 0px
        border: 1px #2c3e50 solid
        padding-left: 5px
        @media (max-width: 400px)
            width: 80%
        &:focus
            box-shadow: 0px 0px 1px 1px #42b983
            z-index: 1

    button
        font-size: 13px
        height: 100%
        @media (max-width: 400px)
            height: 100%
            width: 20%

</style>

