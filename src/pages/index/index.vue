<template>
  <div>
    <div class="mod1">
      <div class="location">
        <div style="float: left">
          <span class="locationname">杭州</span>
          <img src="/static/index/location.png" alt="" class="locationicon">
        </div>
        <div class="search">
          <input type="text" placeholder="搜索求助名称">
        </div>
        <img src="/static/index/xiaoxi.png" alt="" style="width: 15px;height: 18px;" class="xiaoxi">
      </div>
    </div>
    <!--lunbo-->
    <div class="mod2">
      <swiper :indicator-dots="swiperParams.indicatorDots"
              :autoplay="swiperParams.autoplay"
              :interval="swiperParams.interval"
              indicator-color="rgba(255, 255, 255, .5)"
              indicator-active-color="rgba(255, 255, 255, 1)"
              :duration="swiperParams.duration"
              :circular="swiperParams.circular" style="height: 150px;width: 100%;">
        <swiper-item>
          <div style="padding-left: 15px;padding-right: 15px;">
            <div style="width: 100%;height:150px;">
              <image lazy-load="true" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" class="slide-image">
              </image>
            </div>
          </div>
        </swiper-item>
        <swiper-item>
          <div style="padding-left: 15px;padding-right: 15px;">
            <div style="width: 100%;height:150px;">
              <image lazy-load="true" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" class="slide-image">
              </image>
            </div>
          </div>
        </swiper-item>
      </swiper>
    </div>

    <div class="mod3">
      <div class="mod3first">
        <div>谁在寻求帮助</div>
        <div>能提供的服务</div>
      </div>
      <div class="mod3slider">
        <scroll-view scroll-x="true" class="top" :scroll-left="scrollLeft" :scroll-with-animation="animate">
          <div class="tabbar">
            所有
          </div>
          <div class="tabbar">
            温暖公益
          </div>
          <div class="tabbar">
            居家生活
          </div>
          <div class="tabbar">
            强身健体
          </div>
          <div class="tabbar">
            包罗万象
          </div>
          <div class="tabbar">
            居家生活
          </div>
          <div class="tabbar">
            温暖公益
          </div>
          <div class="tabbar">
            居家生活
          </div>
          <div class="tabbar">
            强身健体
          </div>
          <div class="tabbar">
            包罗万象
          </div>
        </scroll-view>
      </div>
    </div>


    <!--列表-->
    <div class="mod4">
      <div class="mod4list">
        <!--start-->
        <div class="list_item" @click="goQiuzhu">
          <div class="list_item_img">
            <img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" alt="">
            <div class="title">
              <span>关爱老人，同老人家一起过生日</span>
              <img src="/static/index/laba.png" alt="">
            </div>
            <div class="time" style="position: relative">
              <img class="header" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" alt="">
              <span class="name">沐沐菌</span>
              <span class="nameicon">已实名</span>
              <div style="position: absolute;right: 0px;top: 0px">
                <img src="/static/index/icon.png" alt="" style="" style="height: 16px;width: 16px;margin-right:5px">
                <span class="times" style="color: #FF952F;font-size: 15px;">2小时20分钟</span>
              </div>
            </div>

            <div class="list_item_bottom">
              <div class="list_item_bottom_b">
                <img src="/static/tabs/my.png" alt="" style="width: 12px;height: 14px;">
                <span>50人</span>
              </div>
              <div style="position: relative;" class="list_item_bottom_b">
                <img src="/static/tabs/my.png" alt="" style="width: 12px;height: 14px;">
                <span>杭州市上城区赞成中心</span>
                <div class="fabushijian">发布于2019-02-14 14:34</div>
              </div>
            </div>
          </div>
        </div>
        <!--ending-->
        <div class="list_item">
          <div class="list_item_img">
            <img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" alt="">
            <div class="title">
              <span>关爱老人，同老人家一起过生日</span>
              <img src="/static/index/laba.png" alt="">
            </div>
            <div class="time" style="position: relative">
              <img class="header" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" alt="">
              <span class="name">沐沐菌</span>
              <span class="nameicon">已实名</span>
              <div style="position: absolute;right: 0px;top: 0px">
                <img src="/static/index/icon.png" alt="" style="" style="height: 16px;width: 16px;margin-right:5px">
                <span class="times" style="color: #FF952F;font-size: 15px;">2小时20分钟</span>
              </div>
            </div>

            <div class="list_item_bottom">
              <div class="list_item_bottom_b">
                <img src="/static/tabs/my.png" alt="" style="width: 12px;height: 14px;">
                <span>50人</span>
              </div>
              <div style="position: relative;" class="list_item_bottom_b">
                <img src="/static/tabs/my.png" alt="" style="width: 12px;height: 14px;">
                <span>杭州市上城区赞成中心</span>
                <div class="fabushijian">发布于2019-02-14 14:34</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      // lunboshezhi
      swiperParams:　{
        indicatorDots: true,
        autoplay: true,
        interval: 1000,
        duration: 900,
        circular: true
      },
      // tabbarshezhi
      animate: true,
      scrollLeft: 0
    }
  },
  methods: {
    goQiuzhu () {
      wx.navigateTo({
        url:"/pages/appeal/main"
      })
    }
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  .mod1{
    padding-left: 15px;
    padding-right: 15px;
  }
  .mod1 .location{
    width: 100%;
    height: 50px;
    /*background: red;*/
    line-height: 50px;
    position: relative;
  }
  .location .locationname{
    color: #404A59;
    font-size: 15px;
    letter-spacing: 2px;
    vertical-align: middle;
  }
  .location .locationicon {
    height: 16px;
    width: 13px;
    /*top: 50%;*/
    vertical-align: middle;
    margin-left: 10px;
  }
  .location .search{
    position: absolute;
    width: 70%;
    height: 30px;
    /*background: green;*/
    left: 72px;
    top: 50%;
    margin-top: -15px;
  }
  .location .search input{
    width: 100%;
    height: 100%;
    text-align: center;
    color: #919191;
    font-size: 12px;
    letter-spacing: 1px;
    background: white;
  }
  .location .xiaoxi{
    position: absolute;
    top: 50%;
    right: 0px;
    margin-top: -9px;
  }
  /*lunbo*/
  .slide-image{
    height: 100%;
    width: 100%;
    border-radius: 10px;
  }

  .mod3{
    margin-top: 15px;
  }
  .mod3first{
    display: flex;
    height: 60px;
    line-height: 60px;
    font-weight: bold;
    color: #404A59;
    font-size: 18px;
  }
  .mod3first div{
    flex: 1;
    text-align: center;
    letter-spacing: 2px;
  }

  /*tabbarshezhi*/
  .top{
    width: 100%;
    text-align: center;
    /*line-height: 42px;*/
    white-space: nowrap;
    background: #fff;
    height: 49px;
  }
  .tabbar{
    padding: 0px 12px;
    height: 26px;
    font-size: 12px;
    line-height: 49px;
    /*height: 42px;*/
    display: inline-block;
    color: #404A59;
    position: relative;
    letter-spacing: 1px;
    /*font-weight: bold;*/
  }
  /*liebiao*/
  .mod4{
    padding-left: 15px;
    padding-right: 15px;
    height: 278px;
  }
  .mod4 .mod4list{
    padding: 10px;
    height: 278px;
  }
  .mod4 .mod4list .list_item{
    width: 100%;
    height: 278px;
    /*background: red;*/
    position: relative;
    margin-bottom: 15px;
  }
  .mod4 .mod4list .list_item .list_item_img{
    width: 100%;
    height: 212px;
    /*background: green;*/
    border-bottom: 1px dashed #B5BFCE;
  }
  .mod4 .mod4list .list_item .list_item_img img{
    width: 100%;
    height: 120px;
    border-radius: 10px;
  }
  .mod4 .mod4list .list_item .list_item_img .title{
    margin-top: 9px;
  }
  .mod4 .mod4list .list_item .list_item_img .title span{
    color: #222222;
    font-size: 15px;
    letter-spacing: 2px;
    vertical-align: middle;
  }
  .mod4 .mod4list .list_item .list_item_img .title img{
    width: 21px;
    height: 19px;
    vertical-align: middle;
    margin-left: 10px;
  }
  .time{
    margin-top: 15px;
  }
  .time img,span{
    vertical-align: middle;
    letter-spacing: 2px;
  }
  .time .header{
    width: 22px!important;
    height: 22px!important;
  }
  .time .name{
    color: #7A8594;
    font-size: 12px;
    margin-left: 10px;
  }
  .time .nameicon{
    padding: 1px 5px;
    background: #E4647F;
    font-size: 10px;
    color: white;
    border-radius: 5px;
    margin-left: 5px;
  }
  .list_item_bottom{
    height: 66px;
    width: 100%;
    /*background:pink;*/
    position: absolute;
    bottom: 0px;
  }
  .list_item_bottom div.list_item_bottom_b{
    height: 50%;
    width: 100%;
    line-height: 33px;
  }
  .list_item_bottom div img,span{
    vertical-align: middle;
  }
  .list_item_bottom div span{
    color: #B5BFCE;
    font-size: 12px;
    margin-left: 6px;
  }
  .fabushijian{
    position: absolute;
    right: 0px!important;
    top: 0px;
    font-size: 10px;
    color: #B5BFCE;
    width: 200px;
    text-align: right;
  }
</style>
