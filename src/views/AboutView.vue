<template>
  <footer class="sponsors_footer">
    <div class="sponsors_wrapper">
      <div class="sponsors_title">
        <span class="sponspors_en_title">sponsors</span>
        <span class="sponspors_cn_title">鑽石級贊助商</span>
      </div>
      <!-- 圖片這邊改用 v-for 跑 -->
      <div class="sponsors_imgs_container">
        <div class="sponsor_cards">
          <a href="https://blockstudio.tw/"
            ><img
              src="../assets/images/footer/block_studio_logo.png"
              alt="Block_Studio"
              class="Block_Studio"
          /></a>
          <a href="https://www.kdanmobile.com/zh-tw"
            ><img
              src="../assets/images/footer/kdan_logo.png"
              alt="KDAN"
              class="kdan"
          /></a>
          <a href="https://titansoft.com/tw"
            ><img
              src="../assets/images/footer/titan_logo.png"
              alt="Titansoft"
              class="Titansoft"
          /></a>
        </div>
      </div>
    </div>
    <div class="footer_copyright">
      <span class="copyright">{{ footerText }}</span>
    </div>
  </footer>
</template>
<script>
export default {
  data() {
    return {
      footerText: "Copyright © 2022 HexSchool.All rights reserved.",
    };
  },
};
</script>

<style scoped lang="scss">
@import "/src/assets/scss/base/style.scss";
.sponsors_footer {
  width: 100%;
  color: #fff;
}
.sponsors_title {
  padding: 60px;
  position: relative;
  width: 350px;
  margin-right: auto;
  margin-left: auto;
}
.sponspors_en_title {
  position: relative;
  font-size: 48px;
  line-height: 72px;
  letter-spacing: 10%;
  font-weight: 400;
}
.sponspors_en_title::before {
  content: url(../assets/images/footer/star_large.png);
  position: absolute;
  top: 30%;
  left: -12%;
}
.sponspors_en_title::after {
  content: url(../assets/images/footer/star_little.png);
  position: absolute;
  top: -20%;
  right: -5%;
}
.sponspors_cn_title {
  font-size: 32px;
  line-height: 48px;
}
.sponsors_wrapper {
  text-align: center;
  background-color: #151f3f;
}
.sponsors_imgs_container {
  width: 100%;
  display: flex;
  justify-content: center;
  padding-bottom: 80px;
}
.sponsor_cards {
  width: 33%;
  display: flex;
  justify-content: space-around;
}
.sponsors_title span {
  display: block;
}
.footer_copyright {
  text-align: center;
  background-color: #06102b;
  padding: 1rem;
}
.copyright {
  font-size: 14px;
  line-height: 20px;
  font-weight: 500;
}
</style>