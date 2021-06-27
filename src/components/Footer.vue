<template>
  <div id="footer">
    <div class="container">
      <div class="row footer_content">
        <div class="col-lg-3">
          <div class="logo">
            <img src="../assets/logo.svg" alt="" />
            <p>Artificial Intelligence</p>
            <h4>
              Lorem ipsum is placeholder text commonly used in the graphic,
              print, and layouts and visual mockups.
            </h4>
            <ul>
              <li><a href="">Company@gmail.com.com</a></li>
              <li><a href="">Phone: (064) 332-1233</a></li>
              <li><a href="">450 Wall Street, USA, New York</a></li>
            </ul>
          </div>
        </div>
        <div class="col-lg-2">
          <h2>INFORMATION</h2>
          <ul>
            <li><a href="">New Collection</a></li>
            <li><a href="">About Store</a></li>
            <li><a href="">Contact Us</a></li>
            <li><a href="">Latest News</a></li>
            <li><a href="">Our Sitemap</a></li>
            <li><a href="">Orders History</a></li>
          </ul>
        </div>
        <div class="col-lg-2">
          <h2>FOOTER MENU</h2>
          <ul>
            <li><a href="#">Instagram profile</a></li>
            <li><a href="#">New Collection</a></li>
            <li><a href="#">Contact Us</a></li>
            <li><a href="#">Latest News</a></li>
            <li><a href="#">Terms & Conditions</a></li>
            <li><a href="#">Purchase Theme </a></li>
          </ul>
        </div>
        <div class="col-lg-2">
          <h2>USEFUL LINKS</h2>
          <ul>
            <li><a href="#">Instagram profile</a></li>
            <li><a href="#">New Collection</a></li>
            <li><a href="#">New Collection</a></li>
            <li><a href="#">Latest News</a></li>
            <li><a href="#">Terms & Conditions</a></li>
            <li><a href="#">Purchase Theme</a></li>
          </ul>
        </div>
        <div class="col-lg-3">
          <h2>ABOUT THE STORE</h2>
          <p>
            Lorem ipsum is placeholder text commonly used in the graphic, print,
            and layouts and visual mockups.
          </p>
          <div>
            <a href="">www.company.com</a>
            <ul>
              <li><a href=""></a></li>
              <li><a href=""></a></li>
              <li><a href=""></a></li>
              <li><a href=""></a></li>
              <li><a href=""></a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    msg: "hello",
  }),
};
</script>

<style lang="scss">
@import "../assets/scss/_colors.scss";
#footer {
  padding: 50px 0 30px 0;
  background: $header-top-bg-color;
  .footer_content {
    .logo {
      display: flex;
      align-items: start;
      p {
        margin: 0;
        margin-bottom: 10px;
        margin-top: 10px;
      }
      h4 {
        font-weight: 100;
        margin-bottom: 20px;
      }
    }
    div {
      display: flex;
      flex-direction: column;
    }
  }
}

li {
  margin-top: 10px;
  a {
    color: #fff;
    font-weight: 600;
  }
}
</style>
