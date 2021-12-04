<template>
  <div class="outer-container">
    <section class="landing-section">
      <div class="l-left">
        <div class="dotted-box"></div>
        <div class="l-desc">
          <div class="l-title">We Help You Make Modern Interior</div>
          <div class="l-sub-title">
            We will help you to make an elegant and luxurious interior designed
            by professional interior designer.
          </div>
        </div>
      </div>
      <div class="l-right">
        <img src="~/assets/images/main_sofa.png" alt="" />
      </div>
    </section>
    <hotDeals></hotDeals>
  </div>
</template>

<script>
import hotDeals from '../sections/hot-deals.vue'
export default {
  layout: "default",
  components: {
    hotDeals
  }
};
</script>
<style lang="scss" scoped>
.outer-container {
  margin: 0 auto;
  max-width: 1320px;
  padding: 0 20px;
  .landing-section {
    position: relative;
    display: flex;
    .l-left {
      flex: 0 0 25%;
      .l-desc {
        position: absolute;
        padding: 70px;
        top: 50%;
        max-width: 450px;
        backdrop-filter: blur(10px);
        background-color: rgba(255, 255, 255, 0.5);
        transform: translateY(-50%);

        .l-title {
          font-size: 60px;
          font-family: PlayFair;
          color: #244e4d;
        }
        .l-sub-title {
          margin-top: 20px;
          font-size: 19px;
        }
      }
    }
  }
}
</style>
