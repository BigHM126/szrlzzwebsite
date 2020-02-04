<template>
  <footer class="footer  dark-wrapper inverse-text footer-bg  footer-bg2">
    <div class="container inner pt-60 pb-60">
      <div class="row">
        <div class="container container-lg">
          <div class="row">
            <div class="col-md-6 mb-5 mb-md-0">
              <div class="card card-lift--hover shadow border-0">
                <router-link to="/landing" title="Landing Page">
                  <b-img-lazy
                    src="~assets/reallink/images/landing.jpg"
                    class="card-img"
                  ></b-img-lazy>
                </router-link>
              </div>
            </div>
            <div class="col-md-6 mb-5 mb-lg-0">
              <div class="card card-lift--hover shadow border-0">
                <router-link to="/profile" title="Profile Page">
                  <b-img-lazy
                    src="~assets/reallink/images/profile.jpg"
                    class="card-img"
                  ></b-img-lazy>
                </router-link>
              </div>
            </div>
          </div>
        </div>

        <div class="container">
          <div class="row row-grid align-items-center my-md">
            <div class="col-lg-6">
              <h3 class="text-primary font-weight-light mb-2">
                欢迎来访，感谢您的支持和帮助！
              </h3>
              <!-- <h4 class="mb-0 font-weight-light">
                我们已经开通如下社交互动平台：
              </h4> -->
            </div>
            <div class="col-lg-6 text-lg-center btn-wrapper">
              <a
                target="_blank"
                rel="noopener"
                href="/"
                class="btn btn-neutral btn-icon-only btn-twitter btn-round btn-lg"
                data-toggle="tooltip"
                data-original-title="Follow us"
              >
                <i class="fa fa-twitter"></i>
              </a>
              <a
                target="_blank"
                rel="noopener"
                href="/"
                class="btn btn-neutral btn-icon-only btn-facebook btn-round btn-lg"
                data-toggle="tooltip"
                data-original-title="Like us"
              >
                <i class="fa fa-facebook-square"></i>
              </a>
              <a
                target="_blank"
                rel="noopener"
                href="/"
                class="btn btn-neutral btn-icon-only btn-dribbble btn-lg btn-round"
                data-toggle="tooltip"
                data-original-title="Follow us"
              >
                <i class="fa fa-dribbble"></i>
              </a>
              <a
                target="_blank"
                rel="noopener"
                href="/"
                class="btn btn-neutral btn-icon-only btn-github btn-round btn-lg"
                data-toggle="tooltip"
                data-original-title="Star on Github"
              >
                <i class="fa fa-github"></i>
              </a>
            </div>
          </div>
          <hr />
          <div class="row">
            <div class="col-sm-4">
              <div class="widget">
                <img
                  src="~assets/reallink/images/logo-white.png"
                  alt="logo"
                  style="width: 124px;"
                />
                <div class="space20"></div>
                <p></p>
                <p>
                  瑞联智造是一家专注与智能制造领域的专业化工业互联网综合服务型公司。我们主要提供智能制造相关的软件、硬件及集成、开发服务。
                </p>
                <div class="space20"></div>
                <hr />
                <p>
                  &copy; 2016-{{ year }}
                  <a href="/">深圳市瑞联智造科技有限公司</a>
                </p>
              </div>
              <!-- /.widget -->
            </div>
            <!-- /column -->

            <div class="col-sm-4">
              <div class="widget" style="text-align: center;">
                <h5 class="widget-title">微信公众号</h5>
                <p></p>
                <b-img-lazy
                  src="~assets/reallink/images/rlzz-weixin.jpg"
                ></b-img-lazy>
                <p style="font-size:12px; color:light">扫一扫，关注我们</p>
              </div>

              <!-- /.widget -->
            </div>
            <!-- /column -->

            <div class="col-sm-4">
              <div class="widget">
                <h5 class="widget-title">联络方式</h5>
                <p>
                  全球技术、立足深圳、服务全国
                </p>

                <div class="space15"></div>
                <ul class="icon-list">
                  <li>
                    <span>深圳市瑞联智造科技有限公司</span>
                  </li>
                  <li>
                    <i class="iconfont icon-email"></i>
                    <a href="mailto:rlzz@szrlzz.com" class="nocolor"
                      >rlzz@szrlzz.com</a
                    >
                  </li>
                  <li>
                    <i class="iconfont icon-service"></i>
                    <span>400-876-1158</span>
                  </li>
                  <li>
                    <i class="iconfont icon-map"></i>
                    <span
                      >广东省深圳市南山区粤海街道高新区中区麻雀岭工业区M-7栋中钢大厦一层</span
                    >
                  </li>
                </ul>
              </div>
              <!-- /.widget -->
            </div>
            <!-- /column -->
          </div>
          <div class="row align-items-center justify-content-md-between">
            <div class="col-md-6">
              <div class="copyright">
                <a
                  href="http://www.colibri.com.cn/"
                  target="_blank"
                  rel="noopener"
                  >科瑞技术(002957)</a
                >
                旗下子公司
              </div>
            </div>
            <div class="col-md-6">
              <ul class="nav nav-footer justify-content-end">
                <li class="nav-item">
                  <a href="http://beian.miit.gov.cn/">粤ICP备17147257号</a>
                </li>
                <li class="nav-item">
                  <a href="/"> 免责声明 </a>
                </li>
                <li class="nav-item">
                  <a href="/"> 版权说明 </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <!-- /.row -->
    </div>
    <!-- /.container -->
  </footer>
</template>
<script>
export default {
  name: 'NuFooter',

  data() {
    return {
      year: new Date().getFullYear()
    }
  }
}
</script>

<style lang="scss">
footer {
  &.footer-bg2 {
    background-image: url(~assets/reallink/images/footer.jpg) !important;
    background-position: center bottom !important;
    background-repeat: no-repeat;
    padding-bottom: 334px;
  }
  &.footer-bg2::before {
    content: ' ';
    background: linear-gradient(to top, rgba(255, 0, 0, 0), rgba(255, 0, 0, 1));
  }
  &.footer-bg2::after {
    content: ' ';
    background: linear-gradient(to top, rgba(255, 0, 0, 1), rgba(255, 0, 0, 0));
  }
  ul {
    padding-left: 0px;
    list-style: none;
  }
  .nav-item {
    padding: 0px 4px;
    a {
      font-size: 14px !important;
    }

    i {
      font-size: 24px !important;
      vertical-align: middle;
      padding: 0px 2px !important;
    }
  }
  a {
    color: #525f7f;
  }
}
</style>
