<template>
  <div class="big">
    <div class="manage_main">
      <p>当前位置：常用工具</p>
      <div class="manage_msg">
        <img src="../../../static/img/noopen.png" alt="">
        <i>此功能本期暂不开放</i>
      </div>
    </div>
  </div>

</template>

<script>
  export default {
    name: "RoleMan",
    data() {
      return {}
    }

  }
</script>

<style scoped>
  .manage_main {
    height: 87vh;
    min-width: 1159px;
    background-color: #f6f7ff
  }

  .manage_main p {
    display: inline-block;
    color: #444;
    font-size: 12px;
    margin-top: 17px;
    margin-left: 18px;
  }

  .manage_msg {
    min-height: 77vh;

    margin:11px 18px 0;
    background-color: #fff;
    text-align: center;
    box-shadow: 0 0 8px 3px rgba(0, 0, 0, 0.1);
  }

  .manage_msg i {
    display: block;
    color: #316caf;
    font-size: 14px;
  }

  .manage_msg img {
    display: block;
    margin: 0 auto;
    padding: 20vh 430px 0;
  }
</style>





<!--本期不上线，所以先注掉-->

<!--<template>-->
  <!--&lt;!&ndash;主体背景部分&ndash;&gt;-->
  <!--<div class="tool_main">-->
    <!--<i>当前位置：常用工具</i>-->
    <!--&lt;!&ndash;主体内容部分&ndash;&gt;-->
    <!--<div class="tool_msg">-->
      <!--&lt;!&ndash;内容单独盒子&ndash;&gt;-->
      <!--<div class="main-content">-->
        <!--<div class="single_msg clearfix">-->
          <!--&lt;!&ndash;左边Logo部分&ndash;&gt;-->
          <!--<div class="left_logo">-->
            <!--<img src="../../../static/img/MHR.png" alt="">-->
          <!--</div>-->
          <!--&lt;!&ndash;右边功能部分&ndash;&gt;-->
          <!--<div class="right_msg">-->
            <!--<p class="one">系统连通性测试</p>-->
            <!--&lt;!&ndash;点击出现弹窗&ndash;&gt;-->
            <!--<i class="two" @click="centerDialogVisible = true">点击使用</i><br>-->
            <!--&lt;!&ndash;弹窗部分&ndash;&gt;-->
            <!--<el-dialog-->
              <!--title="系统连通性测试"-->
              <!--:visible.sync="centerDialogVisible"-->
              <!--width="633"-->
              <!--center>-->
              <!--&lt;!&ndash;弹窗主体内容&ndash;&gt;-->
              <!--<div class="diaBox"-->
                   <!--style="height:100px;margin-top: 10px;border-bottom: 1px solid #ebebeb;padding-bottom: 10px;">-->
                <!--<p class="eqiIp">设备ip:</p><input type="text">-->
                <!--<p class="loginId">登录账号:</p><input type="text">-->
                <!--<p class="loginPass">登录密码:</p><input type="text">-->
              <!--</div>-->
              <!--&lt;!&ndash;弹窗脚部&ndash;&gt;-->
              <!--<span slot="footer" class="dialog-footer">-->
          <!--<el-button type="primary" size="small" @click="centerDialogVisible = false">测试</el-button>-->
          <!--</span>-->
            <!--</el-dialog>-->
            <!--<p class="three">使用说明：无限使用无限使用无限使用无限使用无限使用无限使用无限使用无限使用</p>-->
            <!--<img src="../../../static/img/noread.jpg" alt="">-->
            <!--<p class="four">未读</p>-->
          <!--</div>-->
        <!--</div>-->
        <!--<div class="single_msg clearfix">-->
          <!--&lt;!&ndash;左边Logo部分&ndash;&gt;-->
          <!--<div class="left_logo">-->
            <!--<img src="../../../static/img/MHR.png" alt="">-->
          <!--</div>-->
          <!--&lt;!&ndash;右边功能部分&ndash;&gt;-->
          <!--<div class="right_msg">-->
            <!--<p class="one">查询IP所在网段</p>-->
            <!--&lt;!&ndash;点击出现弹窗&ndash;&gt;-->
            <!--<i class="two" @click="centerDialogVisible = true">点击使用</i><br>-->
            <!--&lt;!&ndash;弹窗部分&ndash;&gt;-->
            <!--<el-dialog-->
              <!--title="系统连通性测试"-->
              <!--:visible.sync="centerDialogVisible"-->
              <!--width="633"-->
              <!--center-->
              <!--:close-on-click-modal="false">-->
              <!--&lt;!&ndash;弹窗主体内容&ndash;&gt;-->
              <!--<div class="diaBox"-->
                   <!--style="margin-top: 10px;padding-bottom: 10px;">-->
                <!--<div style="height: 100px;border-bottom: 1px solid #ebebeb;">-->
                  <!--<p class="eqiIp">设备ip:</p><input type="text">-->
                  <!--<p class="loginId">登录账号:</p><input type="text">-->
                  <!--<p class="loginPass">登录密码:</p><input type="text">-->
                <!--</div>-->
                <!--<div style="height: 50px">-->
                  <!--<p class="eqiIp">对端ip:</p><input type="text">-->
                  <!--<p class="loginId">对端端口:</p><input type="text">-->
                <!--</div>-->
              <!--</div>-->

              <!--&lt;!&ndash;弹窗脚部&ndash;&gt;-->
              <!--<span slot="footer" class="dialog-footer">-->
          <!--<el-button type="primary" size="small" @click="centerDialogVisible = false">测试</el-button>-->
          <!--</span>-->
            <!--</el-dialog>-->
            <!--<p class="three">使用说明：无限使用无限使用无限使用无限使用无限使用无限使用无限使用无限使用</p>-->
            <!--<img src="../../../static/img/noread.jpg" alt="">-->
            <!--<p class="four">未读</p>-->
          <!--</div>-->
        <!--</div>-->
      <!--</div>-->
    <!--</div>-->
  <!--</div>-->
<!--</template>-->

<!--<script>-->
  <!--export default {-->
    <!--name: "ToolCom",-->
    <!--data() {-->
      <!--return {-->
        <!--value: '',-->
        <!--centerDialogVisible: false-->
      <!--}-->
    <!--},-->
    <!--methods: {}-->
  <!--}-->
<!--</script>-->

<!--<style scoped>-->
  <!--/*弹窗内容部分*/-->

  <!--.main-content {-->
    <!--margin: 0 auto;-->
    <!--width: 1140px;-->
    <!--min-width: 1060px;-->
  <!--}-->

  <!--.diaBox p {-->
    <!--float: left;-->
    <!--margin-top: 23px;-->
  <!--}-->

  <!--.diaBox .eqiIp {-->
    <!--margin-left: 45px;-->
  <!--}-->

  <!--.diaBox .loginId {-->
    <!--margin-left: 63px;-->
  <!--}-->

  <!--.diaBox .loginPass {-->
    <!--margin-left: 30px;-->
  <!--}-->

  <!--.diaBox input {-->
    <!--width: 184px;-->
    <!--height: 23px;-->
    <!--float: left;-->
    <!--margin-top: 16px;-->
    <!--margin-left: 10px;-->
    <!--border: 1px solid #ebebeb-->
  <!--}-->

  <!--.right_msg >>> .el-dialog__header {-->
    <!--height: 30px;-->
    <!--background-color: #66bded;-->
    <!--padding: 7px 20px 0 !important;-->
  <!--}-->

  <!--.right_msg >>> .el-dialog&#45;&#45;center {-->
    <!--/*width: 633px;*/-->
  <!--}-->

  <!--.right_msg >>> .el-dialog__body {-->
    <!--padding: 0 !important;-->
  <!--}-->

  <!--.right_msg >>> .el-dialog__title {-->
    <!--color: #fff;-->
    <!--font-size: 14px;-->
  <!--}-->

  <!--.right_msg >>> .el-dialog__headerbtn {-->
    <!--top: 12px;-->
  <!--}-->

  <!--.right_msg >>> .el-dialog__headerbtn .el-dialog__close {-->
    <!--color: #fff;-->
  <!--}-->

  <!--.right_msg >>> .el-button&#45;&#45;small, .el-button&#45;&#45;small.is-round {-->
    <!--width: 80px;-->
    <!--padding: 5px 15px !important;-->
  <!--}-->

  <!--/*主体背景部分*/-->
  <!--.tool_main {-->
    <!--height: 87vh;-->
    <!--min-width: 1159px;-->
    <!--background-color: #f6f7ff-->
  <!--}-->

  <!--.tool_main i {-->
    <!--display: inline-block;-->
    <!--color: #444;-->
    <!--font-size: 12px;-->
    <!--margin-top: 17px;-->
    <!--margin-left: 18px;-->
  <!--}-->

  <!--/*主体内容部分*/-->
  <!--.tool_msg {-->
    <!--height: 77vh;-->
    <!--margin: 11px 18px 0;-->
    <!--background-color: #fff;-->
    <!--box-shadow: 0 0 8px 3px rgba(0, 0, 0, 0.1);-->
  <!--}-->

  <!--/*内容单独盒子*/-->
  <!--.single_msg {-->
    <!--display: inline-block;-->
    <!--float: left;-->
    <!--width: 351px;-->
    <!--height: 92px;-->
    <!--box-shadow: 0 0 8px 3px rgba(0, 0, 0, 0.1);-->
    <!--margin-top: 15px;-->
    <!--margin-left: 20px;-->
    <!--border-radius: 15px;-->
  <!--}-->

  <!--/*左边logo部分*/-->
  <!--.left_logo {-->
    <!--width: 68px;-->
    <!--height: 92px;-->
    <!--background-color: #f0f5f9;-->
    <!--border-radius: 15px 0 0 15px;-->
    <!--float: left;-->
  <!--}-->

  <!--.left_logo img {-->
    <!--display: inline-block;-->
    <!--width: 38px;-->
    <!--height: 46px;-->
    <!--margin-top: 22px;-->
    <!--margin-left: 16px;-->
  <!--}-->

  <!--/*右边功能部分*/-->
  <!--.right_msg {-->
    <!--position: relative;-->
    <!--width: 283px;-->
    <!--height: 92px;-->
    <!--float: left;-->
    <!--line-height: 16px;-->
  <!--}-->

  <!--.single_msg .one {-->
    <!--display: block;-->
    <!--margin-top: 20px;-->
    <!--margin-left: 15px;-->
    <!--font-size: 12px;-->
    <!--float: left;-->
    <!--color: #333;-->
    <!--font-weight: bold;-->
  <!--}-->

  <!--.single_msg .two {-->
    <!--margin-left: 190px;-->
    <!--margin-top: -16px;-->
    <!--float: left;-->
    <!--color: #66bded;-->
    <!--text-decoration: underline;-->
    <!--font-size: 12px;-->
    <!--cursor: pointer;-->
  <!--}-->

  <!--.single_msg .three {-->
    <!--display: block;-->
    <!--width: 240px;-->
    <!--margin-top: 34px;-->
    <!--margin-left: 15px;-->
    <!--font-size: 12px;-->
    <!--color: #333;-->
  <!--}-->

  <!--.right_msg img {-->
    <!--display: inline-block;-->
    <!--width: 44px;-->
    <!--height: 44px;-->
    <!--position: absolute;-->
    <!--top: 0;-->
    <!--right: 0;-->
    <!--border-radius: 0 15px 0 0;-->
  <!--}-->

  <!--.right_msg .four {-->
    <!--position: absolute;-->
    <!--top: 6px;-->
    <!--right: 2px;-->
    <!--font-size: 12px;-->
    <!--color: #fff;-->
  <!--}-->

<!--</style>-->
