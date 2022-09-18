<template>
  <div class="blog-post-card1-blog-post-card" v-bind:class="rootClassName">
    <div class="blog-post-card1-container">
      <span class="blog-post-card1-text">{{ title }}</span>
      <span class="blog-post-card1-text1">{{ description }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BlogPostCard1',
  props: {
    title: {
      type: String,
      default: 'Lorem ipsum dolor sit amet',
    },
    description: {
      type: String,
      default:
        'Lorem ipsum dolor sit amet, consectetur, adipiscing elit. Sed non volutpat turpis.  ​ Mauris luctus rutrum mi ut rhoncus. Integer in dignissim tortor. Lorem  ​​ ipsum dolor sit amet, consectetur adipiscing elit.',
    },
    rootClassName: String,
  },
}
</script>

<style scoped>
.blog-post-card1-blog-post-card {
  width: 100%;
  display: flex;
  overflow: hidden;
  max-width: var(--dl-size-size-maxwidth);
  transition: 0.3s;
  align-items: center;
  flex-direction: column;
  background-size: cover;
  justify-content: center;
  background-image: url("/playground_assets/ellipse%201.svg");
}
.blog-post-card1-blog-post-card:hover {
  transform: scale(1.02);
}
.blog-post-card1-container {
  display: flex;
  padding: var(--dl-space-space-twounits);
  align-items: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}
.blog-post-card1-text {
  font-size: 1.5rem;
  font-weight: 300;
  margin-bottom: var(--dl-space-space-twounits);
}
.blog-post-card1-text1 {
  color: var(--dl-color-gray-500);
  font-weight: 400;
  margin-bottom: var(--dl-space-space-twounits);
}


</style>
