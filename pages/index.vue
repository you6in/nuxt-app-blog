<template>
  <el-row type="flex" justify="center">
    <el-col :xs="24" :sm="18" :md="12" :lg="10">
      <app-post
        v-for="post in posts"
        :key="post._id"
        :post="post"
      ></app-post>
    </el-col>
  </el-row>
</template>

<script>
import AppPost from './../components/main/Post'

export default {
  head: {
    title: 'Main page | ' + process.env.appName
  },
  components: {
    AppPost
  },
  async asyncData({store}) {
    const posts = await store.dispatch('post/fetch')
    return {posts}
  }
}
</script>

<style>

</style>
