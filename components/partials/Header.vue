<template>
  <header class="rl-header container">
    <!--     <div class="row justify-content-between align-items-center"></div> -->

    <b-navbar toggleable="lg" type="light" class="row  justify-content-between">
      <b-navbar-brand href="/" class="col-sm-2 pl-sm-0 w-100 "
        ><b-img
          src="~assets/reallink/images/logo-white.png"
          fluid
          alt="logo"
        ></b-img
      ></b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <!-- <b-nav-item
            v-for="(item, index) in navLinks"
            :key="index"
            :href="item.path"
            class="h5"
            >{{ item.name }}</b-nav-item
          > -->

          <b-nav-item href="/products/" class="h5">在线产品</b-nav-item
          ><b-nav-item href="/lines/" class="h5">解决方案</b-nav-item
          ><b-nav-item href="https://szrlzzdocs.netlify.com/" class="h5"
            >帮助支持</b-nav-item
          ><b-nav-item href="/blogs/" class="h5">业内新闻</b-nav-item
          ><b-nav-item href="/partners/" class="h5">生态联盟</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="mx-auto">
          <b-button pill variant="primary">
            <b-icon icon="laptop"></b-icon> 预约演示
          </b-button>
        </b-navbar-nav>
        <b-navbar-nav class="mx-2 align-center">
          <b-input-group size="sm" class="mb-2" rounded="circle">
            <b-form-input type="search" placeholder="搜索"></b-form-input
            ><b-input-group-append is-text>
              <b-icon icon="search"></b-icon>
            </b-input-group-append>
          </b-input-group>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </header>
</template>

<script>
export default {
  name: 'RlHeader',

  data() {
    return {
      navLinks: [
        { name: '在线产品', icon: '', path: '/products/' },
        { name: '解决方案', icon: '', path: '#' },
        { name: '帮助支持', icon: '', path: 'https://szrlzzdocs.netlify.com/' },
        { name: '业内新闻', icon: '', path: '#' },
        { name: '生态联盟', icon: '', path: '#' }
      ]
    }
  }
}
</script>

<style lang="scss"></style>
