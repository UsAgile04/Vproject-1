<template>
  <div class="wrapper">
    <main>
     <router-view v-bind:data="myData"></router-view>
    </main>
  </div>
</template>


<script>
import myData from "../../../static/data.json";
export default {
  data() {
    return {
      myData: myData
    };
  }
};
</script>