<template>
  <div class="Works">
    <h1 class="page-title">作品紹介</h1>
    <article v-for="d in data">
      <!--  v-for でpropsで指定したdataを繰り返す -->
      <div v-for="p in d.picture" v-if="p.id === '1'">
        <!-- v-if で写真の一枚目のみ呼び出し -->
        <a href="https://myportfoliowebsite-31c0d.firebaseapp.com/">
          <img src="../assets/anamochi.png">
        </a>
        <!-- 詳細へのリンクと画像のURL -->
      </div>

      <div class="work-text">
        <!-- 作品のタイトル -->
        <h1 v-cloak>
          <a
            href="https://myportfoliowebsite-31c0d.firebaseapp.com/"
            class="product-title"
          >{{ d.title }}</a>
        </h1>
        <!-- 作品の解説 -->
        <p class="product-description" v-cloak>―{{ d.description }}―</p>
        <p class="product-description" v-cloak>{{ d.text }}</p>
        <p class="product-description" v-cloak>使用技術：{{ d.role }}</p>
        <!-- 制作年 -->
        <p class="product-year" v-cloak>制作期間：{{ d.year }}</p>
      </div>
    </article>
  </div>
</template>

<script>
export default {
  title: "....",
  description: "...",
  props: ["data"]
};
</script>


<style>
.Works{
  padding: 0 50px
}
.page-title{
  margin: 5% 0;
}

article {
  display: flex;
}

img {
  width: 88%;
  height: 100%;
}
a{
  color: black;
  text-decoration: none;
}
a:hover{
  color: rgb(0, 68, 255);
}

.work-text {
    line-height: 21px;
  letter-spacing: 1.5px;
  padding: 5px;
  display: block;
  width: 65%;
}
.product-description:nth-child(3){
  text-align: left;
}

.product-description:nth-child(4){
  text-align: left;
  font-size: 14px;
}
</style>
