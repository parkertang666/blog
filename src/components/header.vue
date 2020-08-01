<template>
  <header class="header">
    <div class="wrapper row">
      <!-- <h1 class="logo-warpper col-6 col-lg-2">
        <a href="http://">
          <img class="logo-img" width="150px" src="/img/bg.png" alt srcset>
        </a>
      </h1>-->
      <!-- <ul class="navbar-nav mr-auto"> -->
      <div class="col-2 navber-case">
        <h1 class="logo-wrapper">
          <a class="logo-item" href="http://">
            <img class="logo-img" src="/img/bg.png" width="140px" alt srcset>
          </a>
        </h1>
      </div>
      <nav class="col-10 navber-wrapper">
        <!-- <ul class="navber-case float-right">
          <li class="navber-list">
            <a class="case" href="http://">前端开发</a>
            <ul class="downpord">
              <li class="sub-list"><a class="sub-case" href="http://">HTML5 + CSS3</a></li>
              <li class="sub-list"><a class="sub-case" href="http://">Bootstarp</a></li>
              <li class="sub-list"><a class="sub-case" href="http://">Vue+Jquery</a></li>            
            </ul>
          </li>
        </ul>-->
        <ul class="nav justify-content-end">
          <li class="nav-item">
            <a class="nav-link active" href="#">网站首页</a>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              data-toggle="dropdown"
              href="#"
              role="button"
              aria-haspopup="true"
              aria-expanded="false"
            >WEB前端</a>
            <div class="dropdown-menu">
              <a class="dropdown-item" href="#">ECMAjavascript</a>
              <a class="dropdown-item" href="#">HTML5+CSS3</a>
              <a class="dropdown-item" href="#">VueJS</a>
              <!-- <div class="dropdown-divider"></div> -->
              <a class="dropdown-item" href="#">Bootstarp</a>
            </div>
          </li>
                   <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              data-toggle="dropdown"
              href="#"
              role="button"
              aria-haspopup="true"
              aria-expanded="false"
            >服务器端</a>
            <div class="dropdown-menu">
              <a class="dropdown-item" href="#">NodeJS</a>
              <a class="dropdown-item" href="#">模版引擎</a>
              <a class="dropdown-item" href="#">Linux</a>
              <!-- <div class="dropdown-divider"></div> -->
              <a class="dropdown-item" href="#">数据库相关</a>
            </div>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">软件 & 工具</a>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              data-toggle="dropdown"
              href="#"
              role="button"
              aria-haspopup="true"
              aria-expanded="false"
            >前端相关</a>
            <div class="dropdown-menu">
              <a class="dropdown-item" href="#">网站模板</a>
              <a class="dropdown-item" href="#">前端小程序</a>
              <a class="dropdown-item" href="#">Linux</a>
              <!-- <div class="dropdown-divider"></div> -->
              <a class="dropdown-item" href="#">前端Dome</a>
            </div>
          </li>
          
          <li class="nav-item">
            <a class="nav-link" href="#">友情链接</a>
          </li>
          <li class="nav-item">
            <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">关于本站</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.wrapper {
  width: 1200px;
  margin-left: auto;
  margin-right: auto;
  padding: 0 10px;
}

@media screen and (max-width: 1199px) {
  .wrapper {
    width: 100%;
    margin: 0px;
    padding: 0 5px;
  }
}
</style>

<style lang="scss" scoped>
.header {
  background: #1c2327;
  padding-top: 5px;

  &::before {
    position: absolute;
    top: 0;
    left: 0px;
    width: 100%;
    height: 5px;
    background: #000
      linear-gradient(
        to left,
        #4cd964,
        #5ac8fa,
        #007aff,
        #34aadc,
        #5856d6,
        #ff2d55
      );
    content: "";
  }
}

.logo-wrapper {
  margin: 0;
  padding: 0px;
  height: 45px;
  padding: 5px 0;
  box-sizing: content-box;
  line-height: 50px;

  & .logo-item {
    overflow: hidden;
    display: block;
    // width: 135px;
    height: 45px;
    /* margin: 5px 0 0 0; */
    position: relative;
    // margin: 5px 0;
  }
  & .logo-img {
    /* overflow: hidden; */
    position: absolute;
    top: -45px;
  }
}

.nav-item {
  margin: 10px 0;

  & a {
    color: #f5f5f5;
  }
}
</style>