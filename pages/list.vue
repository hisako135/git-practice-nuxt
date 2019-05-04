<template>
  <section class="container">
    <media :posts="postsData"/>
  </section>
</template>

<script>
import Media from '~/components/Media.vue'
import jsonData from '~/assets/json/data.json'

export default {
  components: {
    Media
  },
  computed: {
    postsData() {
      return JSON.parse(JSON.stringify(jsonData).replace(/\\n/g, '<br>'))
    }
  }
}
</script>
