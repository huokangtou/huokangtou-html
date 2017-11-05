<template>
  <div>
    <div class="my_info">
      <div class="my_info_auto clearfix">
        <Menu></Menu>
        <div class="my_info_right">

          <div class="user_center ph_hide">
            <div class="user_center_title">
              基本信息
              <span class="user_center_title_more gray ml10">
  数据更新于15时01分
  </span>
            </div>
          </div>
          <div class="user_center_info clear">
            <div class="rule_info" title="积分和i币规则说明"></div>
            <div class="user_center_info_ph clearfix ph_hide">
              <div class="user_portrait">
                <div class="user_portrait_border"></div>

                <img src="/static/images/head_m.jpg" class="user_head">

              </div>
              <div class="personal_data">
                <div class="personal_div">
                  <span class="personal_name">1194443714@***</span>

                  <a href="javascript:;" onclick="javascript:sign0();" class="btn regist">签到</a>

                </div>
                <div class="security">
                  <span>安全等级</span>
                  <table class="security_level">
                    <tbody><tr>
                      <td><div class="color_box lv1"></div></td>
                      <td><div class="color_box lv2"></div></td>
                      <td><div class="color_box"></div></td>
                    </tr>
                    </tbody></table>
                  <span>中</span>
                </div>
              </div>
            </div>
            <div class="personal_credit">
              <ul>
                <li>
                  <div class="personal_credit_lv">信用等级</div>
                  <div class="personal_lv_num level1">中</div>
                </li>
                <li>
                  <div class="personal_credit_lv">可用积分</div>
                  <div class="personal_jf_num orange">135</div>
                </li>
                <li>
                  <div class="personal_credit_lv">可用i币</div>
                  <div class="personal_xs_num brown">0</div>
                </li>
              </ul>
            </div>
          </div>
          <div class="my_account ph_hide">
            <div class="my_account_info">
              <div class="user_center clear">
                <div class="user_center_title fL">账户信息</div>
              </div>
              <div class="user_account edit_user_account">
                <div class="user_account_list ed_weixin clear">
                  <div class="user_account_name fL">绑定微信</div>

                  <div class="user_account_status fL">
                    <span class="unBound orange">未绑定</span>
                    <!--<span class="unBound_info">绑定手机后才能兑换奖品！</span>-->
                  </div>

                  <a href="/member/info/bindweixin/" class="whiteBtnSmall bind_weixin fR" path="weixin">立即绑定<i></i></a>


                </div>
                <div class="user_account_list ed_phone clear">
                  <div class="user_account_name fL">绑定手机</div>

                  <div class="user_account_status fL">
                    <span class="unBound orange">未绑定</span>
                    <span class="unBound_info">绑定手机后才能兑换奖品！</span>
                  </div>
                  <a href="/member/info/bindmobile/" class="whiteBtnSmall bind_phone fR" path="phone">立即绑定<i></i></a>

                </div>
                <div class="user_account_list clear">
                  <div class="user_account_name fL">绑定邮箱</div>

                  <div class="user_account_status fL">
                    <span class="unBound orange">1194443714@qq.com</span>
                  </div>
                  <a href="/member/info/changeemail/" class="whiteBtnSmall re_email fR" path="email">更换绑定<i></i></a>

                </div>
                <div class="user_account_list set_password_div clear">
                  <div class="user_account_name fL">登录密码</div>

                  <div class="user_account_status fL">
                    <span class="unBound orange">已设置</span>
                  </div>
                  <a href="/member/info/pwd/" class="whiteBtnSmall set_password fR" path="passw">修改密码<i></i></a>

                </div>
                <div class="user_account_list perfect_info_div clear">
                  <div class="user_account_name fL">个人资料</div>
                  <div class="user_account_status fL">

                    <span class="unBound orange">未完善</span>
                    <span class="unBound_info">完善资料确保账号安全！</span>

                  </div>
                  <a href="/member/data/" class="whiteBtnSmall perfect_info fR">立即完善<i></i></a>
                </div>
              </div>
              <div class="user_center clear">
                <div class="user_center_title fL">第三方帐号</div>
              </div>
              <div class="user_account edit_third_account">
                <div class="user_account_list clear">
                  <div class="user_account_name fL"><i class="Other_icon sina"></i>新浪微博</div>

                  <div class="user_account_status fL">
                    <span class="unBound orange">未绑定</span>

                  </div>
                  <a href="/openapi/sina/?furl=bind" class="whiteBtnSmall bound_phone fR">立即绑定<i></i></a>

                </div>
                <div class="user_account_list clear">
                  <div class="user_account_name fL"><i class="Other_icon qq"></i>腾讯QQ</div>

                  <div class="user_account_status fL">
                    <span class="unBound orange">未绑定</span>

                  </div>
                  <a href="/openapi/qq/?furl=bind" class="whiteBtnSmall bound_email fR">立即绑定<i></i></a>

                </div>
                <div class="user_account_list clear">
                  <div class="user_account_name fL"><i class="Other_icon tencent"></i>腾讯微博</div>

                  <div class="user_account_status fL">
                    <span class="unBound orange">未绑定</span>

                  </div>
                  <a href="/openapi/weibo/?furl=bind" class="whiteBtnSmall set_password fR">立即绑定<i></i></a>

                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import Menu from '@/components/Menu'
import Footer from '@/components/Footer'
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components:{
    Menu,
    Footer
  },
  mounted : function(){

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
