<template>
  <div class="page-container">
    <div class="my-head">
      <common_header :userInfo="userInfo"></common_header>
    </div>
    <div class="my-main">
      <div class='container clearfix'>
       <div class="main-left">
         <div class="about_me_container">
           <about_me :aboutMe="aboutMe"></about_me>
         </div>
         <div class="project_container">
          <project_list :projectList="projectList"></project_list>
         </div>
       </div>
        <div class="main-right">
          <div class="block contact_c">
            <contact :contact="contact"></contact>
          </div>
          <div class="block skills_c">
            <skills :skills="skills"></skills>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script type='text/ecmascript-6'>
  import common_header from '../../components/common_header'
  import about_me from '../../components/about_me'
  import project_list from '../../components/project_list'
  import contact from '../../components/contact'
  import skills from '../../components/skills'
  export default {
    name:'index',
    components:{
      common_header,
      about_me,
      project_list,
      contact,
      skills,
    },
    data () {
      return {
        userInfo: {
          headImgUrl:'/static/images/head.jpg',
          uname:'王小恒',
          uworks:'web前端开发'
        },
        aboutMe:{
          introduce:'我叫王小恒，1995年出生。2013年毕业于洞头职业教育中心，计算机专业，接触过计算机软硬件、设计软件、视频处理、可视化编程等等。2016年毕业于浙江工贸职业技术学院，印刷品设计专业，学习印刷品平面设计与排版以及色彩学。毕业后因为一个契机又重新接触编程，自学了一段时间的web前端开发，自己觉得喜欢这一方面的技术，也适合做这一块。2016年11月就业于杭州艾米网络科技有限公司至今。自我评价：思维敏捷，逻辑清晰，热爱探索，乐意琢磨，喜欢编程，自己摸索过一些前端热门技术，如：“vuejs,微信小程序”等技术。',
        },
        projectList:{
          list:[
            {
              title:'HEALBIO',
              imgUrl:'/static/images/project1.png',
              smText:'化妆品展示的响应式网页，运用媒体查询做响应式',
              projectUrl:'http://a.qqbaidu.xyz/xh/HEALBIO/'
            },
            {
              title:'福星彩最专业的线上娱乐平台',
              imgUrl:'/static/images/project2.png',
              smText:'乐透app推广网页，一个全屏轮播的动效页面,运用jq和animate',
              projectUrl:'http://a.qqbaidu.xyz/xh/bann/'
            },
            {
              title:'流量监控后台',
              imgUrl:'/static/images/project3.png',
              smText:'流量监控后台界面网页,运用缩放单位rem做的自适应页面',
              projectUrl:'http://a.qqbaidu.xyz/xh/lladmin/'
            },
            {
              title:'泰隆银行与摩拜单车联合活动',
              imgUrl:'/static/images/project4.png',
              smText:'泰隆银行与摩拜单车联合活动,运用缩放单位rem做的H5页面',
              projectUrl:'http://a.qqbaidu.xyz/xh/mobike/'
            },
            {
              title:'泰隆银行回家的路产品宣传互动',
              imgUrl:'/static/images/project5.png',
              smText:'泰隆银行回家的路产品宣传互动,运用缩放单位rem做的H5页面，涉及到百度地图和echarts数据图表的联动嵌套',
              projectUrl:'http://a.qqbaidu.xyz/xh/mwhRel-z/'
            },
            {
              title:'房产类商城前端页面',
              imgUrl:'/static/images/project6.png',
              smText:'运用缩放单位rem做的H5页面',
              projectUrl:'http://a.qqbaidu.xyz/xh/page/cn/'
            },
            {
              title:'农场大数据前端',
              imgUrl:'/static/images/project7.png',
              smText:'运用jq+echarts+ztree写的单页',
              projectUrl:'http://a.qqbaidu.xyz/xh/yc/'
            },
            {
              title:'时之歌二次元宣传单页',
              imgUrl:'/static/images/project8.png',
              smText:'运用jq+echarts+ztree写的单页',
              projectUrl:'http://a.qqbaidu.xyz/xh/yuno/yuno/yuno.html'
            },
            ]
        },
        contact:{
          address:'浙江省杭州市江干区',
          number:'15267731625',
          email:'15267731625@163.com'
        },
        skills:{
          skillList:[
            {name:'html & html5',value:90},
            {name:'css & css3',value:90},
            {name:'javascript & jQuery',value:80},
            {name:'Map',value:60},
            {name:'highCharts & eCharts',value:70},
            {name:'vuejs & weChat',value:60},
            {name:'php & nodejs',value:30},
            ]
        }
      }
    }
  }
</script>
<style scoped lang="stylus" ref="stylesheet/stylus">
  .my-main
    padding 60px 0;
    background #dae3e7;
  .main-left
    width 820px;
    float left;
  .about_me_container
    margin-bottom 30px;
  .project_container
    background #fff;
    padding 30px;
  .main-right
    width 290px;
    float right;
    .block
      margin-bottom 30px;
</style>
