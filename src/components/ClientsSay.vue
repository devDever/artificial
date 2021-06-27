<template>
  <div id="client_wrapper">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6 col-xs-12">
          <h2>What our clients say about our awesome solutions</h2>
          <p>
            To take a trivial example, which of us ever undertakes laborious
            physical exercise, except to obtain some advantage from it who do
            not know.
          </p>
          <p>
            Lorem ipsum is placeholder text commonly used in the graphic, print,
            and publishing .
          </p>
          <p>
            Lorem ipsum is placeholder previewing layouts and visual mockups.
          </p>
          <p>
            Lorem ipsum is placeholder text commonly used in the graphic, print,
            and publishing industries for previewing layouts and visual mockups.
          </p>
        </div>
        <div class="col-lg-6 d-none d-lg-block">
          <img style="width: 100%" src="../assets/img/client.png" alt="" />
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
#client_wrapper {
  padding: 170px 0 100px;
  background: $base-bg-color;
  h2 {
    margin-bottom: 40px;
    font-size: 40px;
  }
  p {
    margin: 20px 0;
  }
}
</style>
