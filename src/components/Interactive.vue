<template>
  <section class="interactive_container">
    <div class="interactive_wrapper">
      <div class="interactive_marquee">
        <span class="interactive_para">Interactive web design</span>
        <span class="interactive_para">Interactive web design</span>
        <span class="interactive_para">Interactive web design</span>
      </div>
      <!-- banner interactive image -->
      <div class="interactive_block">
        <div class="interactive_block_wrapper">
          <div class="interactive_block_title_box">
            <img
              class="interactive_title_img"
              src="../assets/images/interactive/title.png"
              alt=""
            />
            <img
              class="interactive_banner_img"
              src="../assets/images/interactive/green_bg.png"
              alt=""
            />
            <div class="interactive_hands_img_box">
                <img src="../assets/images/interactive/hand_left.png" alt="" class="hand_img left_hand">
                <img src="../assets/images/interactive/hand_right.png" alt="" class="hand_img right_hand">
            </div>
            <div class="interactive_circle_img_box">
                <img src="../assets/images/interactive/yellow.png" alt="" class="yellow_circle">
                <img src="../assets/images/interactive/purple.png" alt="" class="purple_circle">
            </div>
          </div>
          <!-- banner 文字 x 文字 -->
          <div class="interactive_ui_web_box">
            <span>前端工程師</span>
            <div class="interactive_close_img_box">
              <img
                class="interactive_close_img"
                src="../assets/images/interactive/close.png"
                alt=""
              />
            </div>
            <span class="ui_designer">UI設計師</span>
          </div>
        </div>
      </div>
      <div class="interactive_marquee">
        <span class="interactive_para">Interactive web design</span>
        <span class="interactive_para">Interactive web design</span>
        <span class="interactive_para">Interactive web design</span>
      </div>
    </div>
  </section>
</template>

<script>
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";
import { TextPlugin } from "gsap/TextPlugin";

gsap.registerPlugin(ScrollTrigger);
export default {
  mounted() {
    gsap.registerPlugin(ScrollTrigger, TextPlugin);

    gsap.to(".interactive_para", {
      xPercent: "-50",
      ease: "none",
      duration: 10,
      repeat: -1,
    });
  },
};
</script>

<style lang="scss" scoped>
@import "/src/assets/scss/base/style.scss";
@import "/src/assets/scss/interactive.scss";
</style>
