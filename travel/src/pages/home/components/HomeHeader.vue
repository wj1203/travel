<template>
  <div class="header">
    <div class="header-left">返回</div>
    <div class="header-center">搜索</div>
    <div class="header-right">城市</div>
  </div>
</template>

<script>
export default {
  name: "HomeHeader"
};
</script>

<style lang='stylus' scoped>
.header {
  display: flex;
  line-height: 0.86rem;
  background: #00bcd4;
  color: #fff;

  .header-left {
    width: 0.64rem;
    float: left;
  }

  .header-center {
    flex: 01;
    height : .64rem
    line-height: .64rem;
    margin-top: .1rem;
    margin-left: .2rem;
    background: #fff;
    border-radius: .1rem;
    color: #ccc;
  }

  .header-right {
    width: 1.24rem;
    float: right;
    text-align: center;
  }
}
</style>
