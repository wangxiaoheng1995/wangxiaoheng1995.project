<template>
  <div class="project_list_c">
    <p class="first_title">我的项目</p>
    <ul class="project_list">
      <li v-for="item in projectList.list " class="clearfix">
        <div class="project_img fl">
          <a :href="item.projectUrl"><img :src="item.imgUrl" alt=""></a>
        </div>
        <div class="fl pro_text">
          <p class="title"><a :href="item.projectUrl">{{item.title}}</a></p>
          <p class="text">{{item.smText}}</p>
          <p class="browse"><a :href="item.projectUrl">浏览网页</a></p>
        </div>
      </li>
      <li class="look_move"><a href="">查看更多</a></li>
    </ul>
  </div>
</template>
<script type='text/ecmascript-6'>
    export default {
        name: 'projectList',
        props:['projectList'],
        data() {
            return {
                msg: 'This is vue components.'
            }
        }
    }
</script>
<style scoped lang="stylus" ref="stylesheet/stylus">
.first_title
  margin-top 0;
  margin-bottom 30px;
  color #545e69;
  font-size 24px;
  font-weight bold;
.project_list
  li
    padding 15px 0;
    border-bottom 1px solid #ddd;
  li:last-child
    border 0;
  li.look_move
    text-align center;
    font-size 18px;
    padding-bottom 0;
    margin-top 20px;
  .pro_text
    width 465px;
  .project_img
    padding 0 15px;
    img
      width 250px;
      height 190px;
      border 1px solid #ddd;
  .title a
    color #778492;
    font-size 18px;
    margin-top 0;
    font-family 'Montserrat', sans-serif;
    font-weight 700;
  .text
    margin 5px 0;
    color #434343;
    font-size 16px;
  .browse a
    color #3aaa64;
    font-size 16px;
</style>
