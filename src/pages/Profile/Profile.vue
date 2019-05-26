<template>
  <section class="profile">
      <section class="profile-number">
        <router-link to='/login' class="profile-link">
          <div class="profile_image">
            <img src="./images/head.png">
          </div>
          <div class="user-info">
            <p class="user-info-top">登录/注册</p>
            <p>
              <i class="iconfont icon-shouji"></i>
              <span class="icon-mobile-number">暂无绑定手机号</span>
            </p>
          </div>
          <span class="arrow">
            <i class="iconfont icon-you"></i>
          </span>
        </router-link>
      </section>
      <section class="profile_info_data border-1px">
        <ul class="info_data_list">
          <a href="javascript:" class="info_data_link">
            <span class="info_data_top"><span>0</span> 元</span>
            <span class="info_data_bottom">我的余额</span>
          </a>
          <a href="javascript:" class="info_data_link">
            <span class="info_data_top"><span>0</span> 个</span>
            <span class="info_data_bottom">我的优惠</span>
          </a>
          <a href="javascript:" class="info_data_link">
            <span class="info_data_top"><span>0</span> 分</span>
            <span class="info_data_bottom">我的积分</span>
          </a>
        </ul>
      </section>
      <section class="profile_my_order border-1px">
        <!-- 我的订单 -->
        <a href='javascript:' class="my_order">
          <span>
            <i class="iconfont icon-dingdan"></i>
          </span>
          <div class="my_order_div">
            <span>我的订单</span>
            <span class="my_order_icon">
              <i class="iconfont icon-you"></i>
            </span>
          </div>
        </a>
        <!-- 积分商城 -->
        <a href='javascript:' class="my_order">
          <span>
            <i class="iconfont icon-tubiao309"></i>
          </span>
          <div class="my_order_div">
            <span>积分商城</span>
            <span class="my_order_icon">
              <i class="iconfont icon-you"></i>
            </span>
          </div>
        </a>
        <!-- 硅谷外卖会员卡 -->
        <a href="javascript:" class="my_order">
          <span>
            <i class="iconfont icon-huiyuanqiaguanli"></i>
          </span>
          <div class="my_order_div">
            <span>会员卡</span>
            <span class="my_order_icon">
              <i class="iconfont icon-you"></i>
            </span>
          </div>
        </a>
      </section>
      <section class="profile_my_order border-1px">
        <!-- 服务中心 -->
        <a href="javascript:" class="my_order">
          <span>
            <i class="iconfont icon-fuwu"></i>
          </span>
          <div class="my_order_div">
            <span>服务中心</span>
            <span class="my_order_icon">
              <i class="iconfont icon-you"></i>
            </span>
          </div>
        </a>
      </section>
    </section>
</template>

<script>
export default {
}
</script>

<style lang="stylus" scoped>
@import '../../common/stylus/mixins.styl'
&.profile //我的
  width 100%
  .profile-number
    .profile-link
      clearFix()
      position relative
      display block
      background #FF6347
      padding 20px
      .profile_image
        float left
        width 60px
        height 60px
        border-radius 50%
        overflow hidden
        vertical-align top
        img
          width 100%
        .icon-icon-test
          font-size 62px
      .user-info
        float left
        margin-top 8px
        margin-left 15px
        p
          font-size 20px
          color #fff
          &.user-info-top
            padding-bottom 8px
          .icon-mobile-number
            font-size 14px
            color #fff
      .arrow
        width 12px
        height 12px
        position absolute
        right 20px
        top 40%
        .icon-you
          color #fff
          font-size 16px
  .profile_info_data
    bottom-border-1px(#e4e4e4)
    width 100%
    background #fff
    overflow hidden
    .info_data_list
      clearFix()
      .info_data_link
        float left
        width 33%
        text-align center
        border-right 1px solid #f1f1f1
        .info_data_top
          display block
          width 100%
          font-size 14px
          color #333
          padding 15px 5px 10px
          span
            display inline-block
            font-size 24px
            color #f90
            line-height 26px
        .info_data_bottom
          display inline-block
          font-size 13px
          color #666
          font-weight 400
          padding-bottom 10px
      .info_data_link:nth-of-type(2)
        .info_data_top
          span
            color #ff5f3e
      .info_data_link:nth-of-type(3)
        border 0
        .info_data_top
          span
            color #6ac20b
  .profile_my_order
    top-border-1px(#e4e4e4)
    margin-top 10px
    background #fff
    .my_order
      display flex
      align-items center
      padding-left 30px
      >span
        display flex
        align-items center
        width 20px
        height 20px
        >.iconfont
          margin-left -10px
          font-size 20px
        .icon-dingdan
          color #1C86EE
        .icon-tubiao309
          color #ff5f3e
        .icon-huiyuanqiaguanli
          color #f90
        .icon-fuwu
          color #02a774
      .my_order_div
        width 100%
        border-bottom 1px solid #f1f1f1
        padding 18px 20px 18px 0
        font-size 16px
        color #333
        display flex
        justify-content space-between
        span
          display block
          text-indent 4px
        .my_order_icon
          width 10px
          height 10px
          .icon-you
            color #bbb
            font-size 10px
</style>
