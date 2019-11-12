<template>
  <body class="body">
    <div class="side">
      <ul>
        <li v-for="post in $store.state.posts" :key="post.id">
          <nuxt-link :to="{ hash: '#'+post.fields.slug  }">
            {{ post.fields.title }}
          </nuxt-link>
        </li>
      </ul>
    </div>
    <main class="main">
      <app-card v-for="post in $store.state.posts" :key="post.id" :post="post" />
    </main>
  </body>
</template>

<script>
import AppCard from '~/components/AppCard.vue';
export default {
  components: {
    AppCard,
  },
  mounted() {
    Prism.highlightAll();
  }
}
</script>
