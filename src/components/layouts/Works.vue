<template>
  <div class="wrapper">
    <main>
      <router-view></router-view>
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