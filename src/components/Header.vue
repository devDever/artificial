<template>
  <header>
    <div class="header_top">
      <div class="container">
        <ul class="header_top__list">
          <div>
            <li class="logo">
              <img src="../assets/logo.svg" alt="" />
              <p>Artificial Intelligence</p>
            </li>

            <li class="main_menu d-none d-lg-flex">
              <ul>
                <li><a href="">Home</a></li>
                <li><a href="">About</a></li>
                <li><a href="#client_wrapper">Services</a></li>
                <li><a href="">Blog</a></li>
                <li><a href="">Contact</a></li>
              </ul>
            </li>
          </div>
          <li class="sign_btn">
            <button class="base_btn">Sign in</button>
          </li>
        </ul>
      </div>
    </div>

    <div class="header_main">
      <div class="container">
        <div class="row header_main__content">
          <div
            class="col-lg-7 col-xl-7 col-sm-12 col-md-12 col-xs-12 main_title"
          >
            <h3>Next genaretion platform</h3>
            <h1>Artificial intelligence & Syber security</h1>
            <p>
              Lorem ipsum is placeholder text commonly used in the graphic,
              <br />
              print, and publishing industries for previewing layouts and visual
              <br />
              mockups.
            </p>
            <div>
              <a href="#"><button class="base_btn">Get Started</button></a>
              <a href="#"><button class="base_btn">Watch Video</button></a>
            </div>
          </div>
          <div class="col-lg-5 main_img d-none d-lg-block">
            <img style="width: 100%" src="../assets/img/rocket.png" alt="" />
          </div>
          <div class="col-12 flex-wrap main_partners">
            <img
              v-for="partner in partners"
              :src="partner.src"
              :alt="partner.name"
              :key="partner"
            />
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data: () => {
    return {
      partners: [
        { name: "Ipsum", src: require("../assets/img/g1.png") },
        { name: "Ipsum", src: require("../assets/img/g2.png") },
        { name: "Ipsum", src: require("../assets/img/g3.png") },
        { name: "Ipsum", src: require("../assets/img/g4.png") },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../assets/scss/_colors.scss";
.base_btn {
  font-size: 16px;
}
header {
  font-weight: 600;

  color: #fff;
  // background-color: #08101e;
  background: linear-gradient(
    180deg,
    rgb(23, 14, 36) 50%,
    rgb(24, 14, 36) 100%
  );
  .header_top {
    background-color: $header-top-bg-color;
    height: 100px;
    display: flex;
    align-items: center;
  }
  .header_top__list {
    display: flex;
    justify-content: space-between;
    & > div {
      display: flex;
    }
  }
}

.main_partners {
  margin-top: 100px !important;
  display: flex;
  justify-content: space-between;
  img {
    max-width: 200px;
    min-width: 100px;
  }
}
.main_menu {
  display: flex;
  align-items: center;
  margin-left: 80px;
  ul {
    display: flex;
    li {
      margin-right: 40px;
      margin-top: none;
      a {
        color: #fff;
        font-size: 18px;
      }
    }
  }
}

.logo {
  display: flex;
  align-items: center;
  p {
    color: $base-color;
    font-size: 22.5455px;
    margin-left: 15px;
  }
}

.header_main {
  margin-top: 155.15px;
  padding-bottom: 100px;
  p {
    font-weight: 100;
    opacity: 0.7;
  }
  h1 {
    margin: 10.23px 0 41px 0;
    font-size: 55px;
  }
  h3 {
    font-weight: 600;
    text-transform: uppercase;
    color: $base-color;
  }
  button.base_btn {
    margin-top: 51.14px;
    &:first-child {
      margin-right: 24.23px;
    }
  }
}
</style>
