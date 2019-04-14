<template>
    <div>
        <ul class="list">
            <li class="list-item" v-bind:key="key" v-for="(item, key) in items">
              <div>
                <div class="list-item__img"><img :src="item.thumbnail" /></div>
                <div class="list-item__description">
                  <div class="rating">{{ item.donatorRating }}</div>
                  <div class="name">{{ item.name }}</div>
                  <div class="quantity">Quantos? {{ item.quantity }}</div>
                </div>
              </div>
            </li>
        </ul>
    </div>
</template>
<script>
export default {
  name: 'List',
  props: {
    items: Object
  }
}
</script>

<style lang="sass" scoped>
ul
  padding-left: 0
  list-style: none
  li.list-item
    margin: 0px -5px
    text-align: left
    border-top: 1px #000 solid
    &:last-of-type
      border-top: 1px #000 solid
      border-bottom: 1px #000 solid
    > div
      display: flex
      .list-item__img
        > img
          height: 100%
          width: 100px
      .list-item__description
        padding-left: 10px
        padding: 5px 10px
</style>
