<template>
  <div>
    <div v-for="article in articles">
      <h2><a v-bind:href="article.path">{{article.title}}</a></h2>
    </div>
  </div>
</template>

<script>
export default {
  computed: {
    articles() {
      return this.$site.pages
        .filter(article => article.path.startWith('/articles/'))
        .sort((a, b) => new Date(b.frontmatter.data) - new Date(a.frontmatter.date));
    }
  }
}
</script>