<template>
  <div class="dashboard-container">
    <!--<div  class="dashboard-text">name: {{ name }}</div>-->
    <div><h2>宏利达海棉有限公司</h2></div>
    <div>
      <a href="https://songyuangye.1688.com/?spm=a261y.7663282.autotrace-topNav.1.1906784aoVHhBP" >https://songyuangye.1688.com/?spm=a261y.7663282.autotrace-topNav.1.1906784aoVHhBP </a>
    </div>
    <div> <a href="http://ntdghm.com/index.asp">http://ntdghm.com/index.asp</a></div>

    <div>
      <img src="@/assets/images/wallpaper.png"/>
    </div>

  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'name'
    ])
  }
}
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
}
</style>
