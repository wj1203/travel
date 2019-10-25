<template>
  <div class="header">
    <div class="header-left">
      <span class="iconfont">&#xe6b7;</span>
    </div>
    <div class="header-center">
      <span class="iconfont">&#xe639;</span>
      搜索
    </div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-down">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeHeader"
};
</script>

<style lang='stylus' scoped>
@import '~styles/varibles.styl';

.header {
  display: flex;
  line-height: 0.86rem;
  background: $bgColor;
  color: #fff;

  .header-left {
    width: 0.64rem;
    float: left;
  }

  .header-center {
    flex: 1;
    height: 0.64rem;
    line-height: 0.64rem;
    margin-top: 0.1rem;
    margin-left: 0.2rem;
    background: #fff;
    border-radius: 0.1rem;
    color: #ccc;
  }

  .header-right {
    width: 1.24rem;
    float: right;
    text-align: center;

    .arrow-down {
      font-size: 0.24rem;
    }
  }
}
</style>
