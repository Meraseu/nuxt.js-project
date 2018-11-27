<template>
    <section class="post-list">
        <PostPreview id="1" :is-admin="isAdmin" thumbnail="https://www.brookings.edu/wp-content/uploads/2017/11/metro_20171121_tech-empowers-tech-polarizes-mark-muro.jpg" title="Hello there!" previewText="This my first post!" />
        <PostPreview id="2" :is-admin="isAdmin" thumbnail="https://www.brookings.edu/wp-content/uploads/2017/11/metro_20171121_tech-empowers-tech-polarizes-mark-muro.jpg" title="Hello there!" previewText="This my second post!" />
        <PostPreview id="3" :is-admin="isAdmin" thumbnail="https://www.brookings.edu/wp-content/uploads/2017/11/metro_20171121_tech-empowers-tech-polarizes-mark-muro.jpg" title="Hello there!" previewText="This my third post!" />
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview: PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style lang="scss" scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
