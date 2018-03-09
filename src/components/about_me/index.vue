<template>
  <div id='c_about_me'>
    <h2 class="title">关于我</h2>
    <p class="introduce_text">
      {{aboutMe.introduce}}
    </p>
  </div>
</template>

<script type='text/ecmascript-6'>
  export default {
    name: 'about_me',
    props:['aboutMe'],
    data () {
      return {
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus" ref="stylesheet/stylus">
  .title
    margin-top 0;
    margin-bottom 30px;
    color #545e69;
    font-size 24px;
  #c_about_me
    background #fff;
    padding 30px;
</style>
