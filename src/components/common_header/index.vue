<template>
  <div class="common_header">
    <div class="container">
      <div class="fl clearfix">
        <div class="u_head fl" v-bind:style="{backgroundImage:'url('+userInfo.headImgUrl+')'}" ></div>
        <div class="u_info fl">
          <p class="u_name">{{userInfo.uname}}</p>
          <p class="u_works">{{userInfo.uworks}}</p>
          <div class="social">
            <a class="fa fa-github-alt"></a>
            <a class="fa fa-weibo"></a>
            <a class="fa fa-qq"></a>
            <a class="fa fa-wechat"></a>
          </div>
        </div>
      </div>
      <div class="contact_me fr">
        <i class="fa fa-paper-plane"></i>
        Contact Me
      </div>
    </div>
  </div>
</template>

<script type='text/ecmascript-6'>
  export default {
    name: 'common_header',
    props:['userInfo'],
    data () {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus" ref="stylesheet/stylus">
  .common_header
    border-top 10px solid #778492;
    background #F5F5F5;
    .container
      padding 30px 0;
      .u_head
        background-size 100% auto;
        height 180px;
        width 180px;
        border-radius 50%;
        margin-right 30px;
      .u_info
        .u_name
          color #49515a;
          font-size 38px;
          margin-bottom 5px;
          margin-top 30px;
        .u_works
          color #778492;
          font-family "Lato", arial, sans-serif;
          font-weight 400;
          font-size 24px;
          margin-top 0;
          margin-bottom 15px;
        .social
          a
            background: #b0b7bf;
            width: 36px;
            height: 36px;
            display: inline-block;
            -webkit-border-radius: 50%;
            -moz-border-radius: 50%;
            -ms-border-radius: 50%;
            -o-border-radius: 50%;
            border-radius: 50%;
            -moz-background-clip: padding;
            -webkit-background-clip: padding-box;
            background-clip: padding-box;
            color: #fff!important;
            text-align: center;
            line-height 36px;
            font-size 20px;
            cursor pointer;
            text-decoration none;
            transition background .3s linear;
            margin  0 5px;
          a:hover
            background #5d6b71;
      .contact_me
        display inline-block;
        padding 6px 12px;
        margin-bottom 0;
        font-size 18px;
        line-height 1.42857143;
        text-align center;
        white-space nowrap;
        vertical-align middle;
        -ms-touch-action manipulation;
        touch-action manipulation;
        cursor pointer;
        -webkit-user-select none;
        -moz-user-select none;
        -ms-user-select none;
        user-select none;
        background-image none;
        border 1px solid transparent;
        border-radius 4px;
        font-weight bold;
        background #54ba4e;
        color #fff;
        margin-top 50px;
</style>
