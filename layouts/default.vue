<template>
  <div>
    <rlHeader></rlHeader>
    <nuxt />
    <rlFooter></rlFooter>
  </div>
</template>
<script>
import RlHeader from '@/components/partials/Header'
import RlFooter from '@/components/partials/Footer'

export default {
  components: {
    RlHeader,
    RlFooter
  }
}
</script>

<style lang="scss">
@import '~assets/reallink/css/config';

html {
  font-family: 'Helvetica Neue', Helvetica, 'PingFang SC', 'Hiragino Sans GB',
    'Microsoft YaHei', '微软雅黑', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
</style>
