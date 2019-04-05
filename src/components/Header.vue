<template>
    <div class="header">
      <div class="logo">M</div>
      <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/external">Find stuff</router-link> |
        <router-link to="/shared">Share stuff</router-link>
      </div>
    </div>
</template>
<script>
export default {
  name: 'Header'
}
</script>
<style scope lang="sass">
.header
  display: flex
  flex-wrap: nowrap
  background: #ccd9e6

.logo
  text-align: center
  padding: 10px
  background: #c5cbd2

#nav
  text-align: left
  padding: 10px
  a
    font-weight: bold
    color: #2c3e50
    &.router-link-exact-active
      color: #42b983
</style>
