<template>
  <div>
    <article>
      <h1 v-cloak>{{ filteredData.title }}</h1>
      <div v-for="p in filteredData.picture" v-if="p.id === '1'">
        <img :src="p.path">
      </div>
      <p v-cloak>{{ filteredData.text }}</p>
      <p v-cloak>制作年：{{ filteredData.year }}</p>
      <p v-cloak>{{ filteredData.role }}</p>
      <p v-cloak>
        <a :href="filteredData.url" target="_blank">{{ filteredData.urlTitle }}</a>
      </p>
      <div v-for="p in filteredData.picture" v-if="p.id !== '1'">
        <img :src="p.path">
      </div>
    </article>
  </div>
</template> 



<script>
export default {
  props: ["data"],
  computed: {
    filteredData: function() {
      var url =
        window.location.protocol + "//" + window.location.host + "/works/";
      var matchData = this.data.filter(function(item, index) {
        if (item.slug === window.location.href.replace(url, "")) return true;
      });
      return matchData[0];
    }
  }
};
</script> 

<script>
export default {
  props: ["data"],
  computed: {
    filteredData: function() {
      var url =
        window.location.protocol + "//" + window.location.host + "/works/";
      var matchData = this.data.filter(function(item, index) {
        if (item.slug === window.location.href.replace(url, "")) return true;
      });
      return matchData[0];
    }
  }
};
</script>
