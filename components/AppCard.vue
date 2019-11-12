<template>
<div class="card">
  <h1 :id="this.post.fields.slug">{{ this.post.fields.title }}</h1>
  <div v-html="convertToHtml">
  </div>
</div>
</template>
<script>
export default {
  props: {
    post: {
      tupe: Object,
      default: () => {},
    }
  },
  computed: {
    convertToHtml() {
      return this.$md.render(this.post.fields.content);
    }
  }
}
</script>
