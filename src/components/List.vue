<template>
    <div>
        <ul>
            <!-- <li v-bind:key="key" v-for="(item, key) in items">{{ item.name }}</li> -->
            <li></li>
        </ul>
    </div>
</template>
<script>
export default {
    name: 'List'
}
</script>

<style lang="sass" scoped>
ul
    padding-left: 0
    list-style: none
    li
        margin: 0px -5px
        text-align: left
        padding-left: 10px
        padding: 5px 10px
        border-top: 1px #000 solid
        &:last-of-type
            border-top: 1px #000 solid
            border-bottom: 1px #000 solid
</style>

