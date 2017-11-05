<template>
  <div>
    <div class="task_center">
      <div class="task_center_auto">
        <div class="all_notice">
          <i class="notice_icon_1"></i>
          <p>
            2017年开始，爱调研社区平台将在每年的12月31日将会对上一年度获得的且未使用积分和i币进行无效处理，请及时兑换奖品。

            <a href="http://www.idiaoyan.com/help/wzgg/?index=expire" class="ml10 orange" target="_blank">&gt; 查看详情</a>

          </p>
          <i class="notice_icon_2" sitemsg_id="5865d2ba611ebf52ab2ba33b"></i>
        </div>
        <div class="task_center_credit">
          <div class="task_center_credit_l clearfix">
            <div class="user_portrait bigger">
              <div class="user_portrait_border"></div>

              <img src="http://h.com:8002/html/indexStatic/images/head_m.jpg" class="user_head">

            </div>
            <div class="personal_div">
              <span class="personal_name">1194443714@***</span>
              <a href="/member/mycredit/" class="view_rule gray">查看信用积分规则&gt;</a>
            </div>
          </div>
          <div class="task_center_credit_r clearfix">
            <ul>
              <li>
                <div class="personal_credit_lv">我的信用积分</div>
                <div class="personal_jf_num white">50</div>
              </li>
              <li>
                <div class="personal_credit_lv">我的信用等级</div>
                <div class="personal_lv_num white">中</div>
              </li>
              <li>
                <div class="personal_credit_lv">奖励系数</div>
                <div class="personal_xs_num white"><span class="f20">x</span><span>1.0</span></div>
              </li>
            </ul>
          </div>
        </div>

        <div> 平台筛选：
          <RadioGroup v-model="platform" type="button">
            <Radio label="点调"></Radio>
            <Radio label="米调"></Radio>
            <Radio label="深圳"></Radio>
            <Radio label="杭州"></Radio>
          </RadioGroup>
        </div>

        <div class="user_center clear">
          <div class="user_center_title fL">我的任务</div>
          <a href="/member/myjoin/" class="more fR">查看参与过的任务&gt;</a>
        </div>
        <!-- 列表 -->
        <div class="new_task thisdiv">
          <div class="new_task_list clearfix">
            <div class="new_task_num" style="width: 200px; overflow: hidden;">
              <div class="new_task_num_detail">
                <span>400.0</span><span class="f14">积分</span>
              </div>
              <div class="new_task_num_more">
                <p>基础奖励<span>400.0</span></p>
                <p>信用奖励<span>0.0</span></p>
              </div>
            </div>
            <div class="new_task_name">
              <p class="pos_title">服务满意度R171010</p>
              <p class="sub_title" title=""></p>
            </div>
            <div class="new_task_jion fR">
              <a href="https://www.surveyunion.com/answer/ba/2MzNyMDI/?personid=E_7_569664b2c1a87d299e7e1f09" target="_blank" class="new_task_jion_a">立即参与</a>
            </div>
          </div>
        </div>
        <div>
          <Page :total="100" show-elevator show-sizer></Page>
        </div>

      </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
  import MenuComponent from '@/components/Menu'
  import FooterComponent from '@/components/Footer'
  export default {
    name: 'HelloWorld',
    data () {
      return {
        platform:'点调',
        msg: 'Welcome to Your Vue.js App'
      }
    },
    components:{
      MenuComponent,
      FooterComponent
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
