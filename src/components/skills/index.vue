<template>
  <div class="skills">
    <p class="first_title">职业技能</p>
    <div class="skills_list">
      <div v-for="skill in skills.skillList" class="skill_item">
        <p class="skill_name">{{skill.name}}</p>
        <div class="skill_index">
          <em :style="{width:skill.value+'%'}"></em>
        </div>
      </div>
    </div>
  </div>
</template>
<script type='text/ecmascript-6'>
    export default {
        name: 'skills',
        components: {},
        props:['skills'],
        data() {
            return {
                msg: 'This is vue components.'
            }
        }
    }
</script>
<style scoped lang="stylus" ref="stylesheet/stylus">
.skills
  background #fff;
  padding 30px;
  .first_title
    margin-top 0;
    margin-bottom 30px;
    color #545e69;
    font-size 24px;
    font-weight bold;
  .skills_list
    .skill_item
      margin-bottom 10px;
      .skill_name
        color #888;
        font-size 16px;
        font-weight bold;
        margin-bottom 8px;
      .skill_index
        width 100%;
        background #ddd;
        em
          display block;
          height 10px;
          background #66cb8c;
</style>
