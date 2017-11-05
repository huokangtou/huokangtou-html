<template>
  <div class="my_info_left clearfix">
    <div class="my_info_left_ph">
      <div class="my_info_ul clearfix">
        <p class="my_info_ul_title">个人中心</p>
        <ul>
          <li>
            <a href="/member/data/">个人资料<i></i></a>
          </li>
          <li>
            <a href="/member/info/" class="act">帐号信息<i></i></a>
          </li>
          <li>
            <a href="/member/mycredit/">我的信用<i></i></a>
          </li>
        </ul>
      </div>
      <div class="my_info_ul clearfix">
        <p class="my_info_ul_title">我的奖励</p>
        <ul>
          <li>
            <a href="/member/myiscore/">我的i币<i></i></a>
          </li>
          <li>
            <a href="/member/myscore/">我的积分<i></i></a>
          </li>
          <li>
            <a href="/member/myconvert/">我的兑换<i></i></a>
          </li>
        </ul>
      </div>
      <div class="my_info_ul clearfix">
        <p class="my_info_ul_title">我的参与</p>
        <ul>
          <li>
            <a href="/member/myjoin/">任务记录<i></i></a>
          </li>
          <!--
          <li>
          <a href="#">我的活动<i></i></a>
          </li>
          -->
          <li>
            <a href="/member/mymessage/">我的消息<i></i></a>
          </li>
          <li>
            <a href="/member/myinvite/">我的邀请<i></i></a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
