<template>
    <div class="error-layout">
      <div class="error-content">
        <h1 class="error-title">Error 404</h1>
        <nuxt-link to="/">to main page</nuxt-link>
      </div>
    </div>
</template>

<script>
    export default {
        name: "error"
    }
</script>

<style lang="sass" scoped>
  .error-layout
    display: flex
    justify-content: center
    align-items: center
    width: 100%
  .error-content
    display: flex
    flex-direction: column
    align-items: center
    padding-top: 4rem
  .error-title
    color: orangered
    margin-bottom: 1rem
</style>
