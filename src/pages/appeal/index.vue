<template>
  <div>
    <div class="mod1">
      <div class="modcontent">
        <div class="slider" style="width: 100%;">
          <swiper :indicator-dots="swiperParams.indicatorDots"
                  :autoplay="swiperParams.autoplay"
                  :interval="swiperParams.interval"
                  indicator-color="rgba(255, 255, 255, .5)"
                  indicator-active-color="rgba(255, 255, 255, 1)"
                  :duration="swiperParams.duration"
                  :circular="swiperParams.circular" style="height: 150px;width: 100%;">
            <swiper-item>
              <div style="">
                <div style="width: 100%;height:150px;">
                  <image lazy-load="true" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" class="slide-image">
                  </image>
                </div>
              </div>
            </swiper-item>
            <swiper-item>
              <div style="">
                <div style="width: 100%;height:150px;">
                  <image lazy-load="true" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" class="slide-image">
                  </image>
                </div>
              </div>
            </swiper-item>
          </swiper>

          <div class="title">
            <span>关爱老人，同老人家一起过生日</span>
            <img src="/static/index/laba.png" alt="">
          </div>

          <div class="timecontent">
            <div></div>
          </div>
        </div>
        <!--上面ending-->
        <div class="list_item_bottom">
          <div class="list_item_bottom_b">
            <img src="/static/tabs/my.png" alt="" style="width: 12px;height: 14px;">
            <span>50人</span>
          </div>
          <div style="position: relative;" class="list_item_bottom_b">
            <img src="/static/tabs/my.png" alt="" style="width: 12px;height: 14px;">
            <span>杭州市上城区赞成中心</span>
          </div>
          <div style="position: relative;" class="list_item_bottom_b">
            <img src="/static/tabs/my.png" alt="" style="width: 12px;height: 14px;">
            <span>2019-02-14 14:34</span>
          </div>
        </div>

        <!--ending-->
      </div>
    </div>


    <div class="mod2" style="padding-left: 15px;padding-right: 15px;">
      <div style="height: auto;width: 100%">
        <p style="color: #404A59;font-size: 15px;letter-spacing: 1px;">求助描述</p>
        <p style="color: #7A8594;font-size: 14px;letter-spacing: 1px;margin-top: 20px;">服务描述服务描述服务描述服务描述，服务描述服务描述服务描述服务描述，服务描述服务描述服务描述服务描述，服务描述服务描述服务描述服务描述，服务描述服。</p>
        <ul>
          <li><img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" alt=""></li>
        </ul>
      </div>
    </div>

    <div class="mod3" style="padding-left: 15px;padding-right: 15px;margin-bottom:15px;">
      <div style="height: 123px;width: 100%">
        <p style="color: #111111;font-size: 15px;letter-spacing: 1px;">发布者</p>
        <div class="headercontent">
          <img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1551800022250&di=a88f57e134f69a134878e55cad2bd30c&imgtype=0&src=http%3A%2F%2Fuploads.5068.com%2Fallimg%2F1712%2F151-1G220094P9.jpg" alt="">
          <div class="contentren">
            <p style="color: #404A59;font-size: 16px;letter-spacing: 1px;">阿里巴巴志愿者协会</p>
            <p style="font-size: 12px;">
              <span>服务</span>
              <span>28</span>
              <span>评价</span>
              <span>5.0</span>
            </p>
          </div>
          <!--guanzhuanniu-->
          <div class="guanzhubtn">
            关注
          </div>
          <!--ending-->
        </div>
      </div>
    </div>

    <footer style="padding: 10px 15px;">
      <div class="contentimg">
        <div class="contentimg_item" id="contentimg_item" style="float: left">
          <div>
            <img src="/static/index/tab1.png" alt="">
            <p>分享</p>
          </div>
          <div>
            <img src="/static/index/tab2.png" alt="">
            <p>留言</p>
          </div>
        </div>

        <div class="contentimg_item" style="position: relative;float: right">
          <div style="" class="bangzhu">帮助他</div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
  export default {
    name: "index",
    data ()　{
      return{
        swiperParams:　{
          indicatorDots: true,
          autoplay: true,
          interval: 1000,
          duration: 900,
          circular: true
        },
      }
    }
  };
</script>

<style scoped>
  .mod1{
    padding-left: 15px;
    padding-right: 15px;
    height: 328px;
  }
  .mod1 .modcontent{
    width: 100%;
    height: 328px;
    /*background: red;*/
  }

  .title{
    margin-top: 9px;
  }
  .title span{
    color: #222222;
    font-size: 18px;
    letter-spacing: 2px;
    vertical-align: middle;
  }
  .title img{
    width: 21px;
    height: 19px;
    vertical-align: middle;
    margin-left: 10px;
  }

  .slider{
    border-bottom: 1px dashed #B5BFCE;
  }
  image{
    border-radius: 10px;
    height: 100%;
    width: 100%;
  }

  .list_item_bottom{
    height: 91px;
    width: 100%;
    /*background: antiquewhite;*/
  }
  .list_item_bottom div.list_item_bottom_b{
    height: 33.3%;
    width: 100%;
    line-height: 30px;
  }
  .list_item_bottom div img,span{
    vertical-align: middle;
  }
  .list_item_bottom div span{
    color: #B5BFCE;
    font-size: 12px;
    margin-left: 6px;
  }

  .mod2{
    margin-top: 15px;
  }
  .mod2 ul{
    margin-top: 20px;
  }
  .mod2 ul li:last-child{
    padding-bottom: 15px;
  }
  .mod2 ul li img{
    width: 100%;
    height: 150px;
    border-radius: 10px;
  }
  .headercontent{
    margin-top: 15px;
    position: relative;
  }
  .headercontent img{
    height: 63px;
    width: 63px;
  }
  .contentren{
    height: 50px;
    width: 200px;
    position: absolute;
    top: 50%;
    margin-top: -25px;
    left: 74px;
  }
  .guanzhubtn{
    width: 73px;height: 25px;position: absolute;
    top: 50%;margin-top: -12.5px;background: #FF952F;color: white;font-size: 15px;letter-spacing: 1px;text-align: center;right: 0px;
    border-radius: 10px;
    line-height: 25px;
  }
  .contentimg{
    width: 100%;
    height: 64px;
    background: white;
    position: fixed;
    bottom: 0;
    z-index: 999999;
  }
  .contentimg_item{
    width: 50%;
    height: 100%;
  }
  #contentimg_item{
    display: flex;
  }
  #contentimg_item div{
    flex: 1;
    text-align: center;
    color: #7A8594;
    font-size: 14px;
    letter-spacing: 1px;
  }
  #contentimg_item div img{
    height: 22px;
    width: 22px;
    margin-top: 10px;
  }
  .bangzhu{
    height: 44px;width: 80%;background: #F06552;position: absolute;border-radius: 10px;color: white;letter-spacing: 1px;
    line-height: 44px;
    text-align: center;
    top: 50%;
    margin-top: -22px;
  }
</style>
