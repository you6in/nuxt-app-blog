<template>
  <nav>
    <el-row>
      <nuxt-link to="/"><h1>Blog</h1></nuxt-link>
    </el-row>


  </nav>
</template>

<script>
    export default {
        name: "AppNavigation"
    }
</script>

<style lang="sass" scoped>
  nav
    display: flex
    align-items: center
    justify-content: center
    height: 100%
    border-bottom: 1px solid #e6e6e6
</style>
