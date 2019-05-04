<template>
  <ul class="list-unstyled">
    <li
      v-for="(post, index) in posts"
      :key="index"
      class="media my-4">
      <div 
        :style="`background-image:url(img/${post.filename}`"
        class="media-img mr-3">
        <img
          :alt="post.filename"
          :src="`img/${post.filename}`">
      </div>
      <div class="media-body">
        <h5 class="mt-0 mb-1">{{ post.title }}</h5>
        <p v-html="post.desc"/>
      </div>
    </li>
  </ul>
</template>

<script>
export default {
  props: {
    posts: {
      type: Object,
      default: () => {}
    }
  }
}
</script>

<style lang="scss" scoped>
.media-img {
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
  flex: 0.5;
  height: 0;
  padding-top: 40%;
  width: 100%;
  > img {
    display: none;
  }
}
</style>
