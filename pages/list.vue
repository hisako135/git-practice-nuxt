<template>
  <section class="container">
    <list :posts="posts"/>
  </section>
</template>

<script>
import List from '~/components/List.vue'

export default {
  components: {
    List
  },
  asyncData({ env, params }) {
    return {
      posts: require(`~/assets/json/data.json`)
    }
  }
}
</script>
