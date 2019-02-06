<template>
  <div class="top">
    <div>
      <h1 class="page-title">I am...</h1>
      <div class="Iam">
        <div class="Iam_about">
          <table>
            <tbody>
              <tr>
                <th>Name</th>
                <td>　矢野 智輝</td>
              </tr>
              <tr>
                <th>Birthday</th>
                <td>　1992/04/27</td>
              </tr>
              <tr>
                <th>Hobby</th>
                <td>　遠出・読書</td>
              </tr>
              <tr>
                <th>Tokugi</th>
                <td>　空手・ベース</td>
              </tr>
              <tr>
                <th>Hitokoto</th>
                <td>　おしゃべり好きです。</td>
              </tr>
            </tbody>
          </table>
        </div>

        <div class="Iam_gakureki">
          <ul>
            <li class="listH">学歴</li>
            <li>2011年3月 徳島県立城東高等学校 卒業</li>
            <li>2015年3月 近畿大学 法学部 法律学科 卒業</li>
          </ul>
          <ul>
            <li class="listH">取得経験のある資格</li>
            <li>普通自動車運転免許（第一種）</li>
            <li>マイクロソフト認定資格（MCSE）</li>
            <li>シスコ技術者認定 CCNA</li>
            <li>ITIL Foundation Certification</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
 
<script>
export default {
  name: "Top",
  title: "Top",
  description: "yanoのポートフォリオサイト",
  props: ["data"]
};
</script>


<style>
h1 {
  text-align: center;
}

.Iam {
  display: flex;
  justify-content: center;
}

.Iam_about {
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.233);
  text-align: left;
  border-radius: 30px;
  width: 350px;
  margin: 0 25px;
  padding: 38px 40px;
  line-height: 30px;
}
table{
  padding: 0 20px;
}
th {
  margin: 0 2px;
}

.Iam_gakureki {
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.233);
  text-align: left;
  width: 400px;
  padding: 25px 1px;
  margin: 0 25px;
  line-height: 25px;
  border-radius: 30px;
}
.Iam_gakureki ul li {
  display: list-item;
}

.listH {
  font-weight: bold;
  margin: 5px;
}
</style>
