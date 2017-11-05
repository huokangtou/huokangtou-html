<template>
  <div class="my_header">
    <div class="my_header_auto">
      <a href="/"><div class="header_top_logo"></div></a>
      <a href="javascript:;" class="bread_btn"> </a>
      <div class="ph_title">我的主页</div>
      <div class="head_top_a">
        <div class="logged_in">
          欢迎您，<span class="user_name">1194443714@***</span>
          <a href="/logout/" class="login_out fR">[退出登录]</a>
        </div>
        <div class="clearfix header_top_list">
          <ul class="header_top_list">
            <li v-bind:class="[current==1 ? 'act' : '']">
              <a href="/"><i class="ph_hp"></i><span>我的主页</span></a>
            </li>
            <li v-bind:class="[current==2 ? 'act' : '']">
              <a href="/member/taskcenter/"><i class="ph_tc"></i><span>任务中心</span></a>
            </li>
            <li v-bind:class="[current==3 ? 'act' : '']">
              <a href="/giftlist/"><i class="ph_pl"></i><span>奖品兑换</span></a>
            </li>
          </ul>
        </div>
      </div>
      <div class="user">
<span class="user_name">
<div class="red_point"></div>
<span>1194443714@***</span>
<i class="user_arrow"></i>
</span>
        <div class="user_more">
          <div class="user_portrait">
            <div class="user_portrait_border"></div>

            <img src="/static/images/head_m.jpg" class="user_head"/>

          </div>
          <div class="user_operating">
            <a href="/member/mymessage/" class="user_news">我的消息<font color="#ec6618">(<span class="user_emails">1</span>)</font></a>
            <a href="/logout/" class="logo_out">退出</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: ''
    }
  },
  props : ['current'],
  mounted : function(){
      console.log(this.$route)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
