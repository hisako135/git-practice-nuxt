<template>
  <section class="container">
    <list :posts="postsData"/>
  </section>
</template>

<script>
import List from '~/components/List.vue'
import jsonData from '~/assets/json/data.json'

export default {
  components: {
    List
  },
  computed: {
    postsData() {
      return JSON.parse(JSON.stringify(jsonData).replace(/\\n/g, '<br>'))
    }
  }
}
</script>
