<template>
  <section class="container">
    <ul class="list-unstyled">
      <li
        v-for="(post, index) in posts"
        :key="index"
        class="media my-4">
        <img
          :alt="post.filename"
          :src="`img/${post.filename}`"
          class="mr-3">
        <div class="media-body">
          <h5 class="mt-0 mb-1">{{ post.title }}</h5>
          <p>{{ post.desc }}</p>
        </div>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  props: {
    posts: {
      type: Object,
      default: function() {
        return {}
      }
    }
  }
}
</script>
