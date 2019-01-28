<template>
  <div>
    <h1>Works 作品紹介</h1>
    <article v-for="d in data">
      <div v-for="p in d.picture" v-if="p.id === '1'">
        <router-link :to="'/works/' + d.slug">
          <img :src="p.path">
        </router-link>
      </div>
      <div>
        <h1 v-cloak>
          <router-link :to="'/works/' + d.slug">{{ d.title }}</router-link>
        </h1>
        <p class="product-description" v-cloak>{{ d.text }}</p>
        <p class="product-year" v-cloak>制作年：{{ d.year }}</p>
      </div>
    </article>
  </div>
</template>

<script>
export default {
  title: "....",
  description: "...",
  props: ['data']
};
</script>