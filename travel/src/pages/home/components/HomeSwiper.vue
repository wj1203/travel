<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img
          class="swiper-img"
          :src="item.imgUrl"
        />
      </swiper-slide>
      <!-- 小圆点 -->
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOption: {
         pagination:'.swiper-pagination',
         loop:true
      },
      swiperList:[
          {
              id:'01',
              imgUrl:'https://imgs.qunarzz.com/p/tts9/1806/52/39318582f0307502.jpg_r_390x260x90_c6d0d7fa.jpg'
          },
          {
              id:'02',
              imgUrl:'https://imgs.qunarzz.com/vs_ceph_vs_tts/28bc78ad-b548-481a-9c01-91802812b228.jpg_r_480x320x90_067ae8a7.jpg'
          }
      ]
    };
  }
};
</script>

<style scoped>
    /* 样式穿透 使scoped属性失效 */
.wrapper >>> .swiper-pagination-bullet-active{
    background:#fff;
}
.wrapper {
  /* 保持宽高比 100/66 */
  overflow: hidden;
  width: 100%;
  height: 0;
  padding-bottom: 66.6%;
}
.swiper-img {
  width: 100%;
}
</style>