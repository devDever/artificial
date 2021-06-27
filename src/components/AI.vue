<template>
  <div id="ai">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-7 d-none d-lg-block">
          <img src="../assets/img/ai-brain.png" alt="" />
        </div>
        <div class="col-lg-5 col-xs-12 ai-title">
          <h2>Apply AI, Deep Learning and Data Sciece to solve</h2>
          <p>
            Lorem ipsum is placeholder text commonly used in the graphic, print,
            and publishing industries for previewing layouts and visual mockups.
          </p>
          <a href=""><button class="base_btn">Learn More</button></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../assets/scss/_colors.scss";
#ai {
  background: $base-bg-color;
  padding-top: 145px;
  .ai-title {
    h2 {
      font-weight: 800;
      font-size: 40px;
    }
    p {
      opacity: 0.7;
      margin: 30px 0 50px 0;
    }
  }
}
</style>
