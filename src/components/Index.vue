<template>
  <div>
    <Head></Head>
    <div class="main" :class="flag?'show':'hide'">
      <div class="left">
        <keep-alive>
          <Tab></Tab>
        </keep-alive>
      </div>
      <div class="collapse-btn" @click="collapseChage" :class="flag?'showBtn':'hideBtn'"> {{flag===true?'<':'>'}}</div>
      <div class="content">
        <router-view ></router-view>
      </div>
    </div>
  </div>
</template>
<script>
  import Head from './Head'
  import Tab from './Tab'

  export default {
    name: 'Index',
    components: {Head, Tab},
    data() {
      return {
        flag: true,
      }
    },
    methods: {
      collapseChage() {
        this.flag = !this.flag
      }
    },
  }
</script>

<style scoped>
  .main {
    padding-left: 207px;
  }

  .left {
    float: left;
    margin-left: -207px;
  }

  .content {
    float: left;
    width: 100%;

  }

  .collapse-btn {
    position: absolute;
    width: 11px;
    height: 33px;
    top: 50vh;
    left: 207px;
    cursor: pointer;
    color: #fff;
    font-size: 16px;
    font-weight: bold;
    font-family: "黑体";
    line-height: 32px;
    background-color: #57b5e9;
    border-radius: 0 8px 8px 0;
    z-index: 99;
  }

  .show {
    padding-left: 207px;
  }

  .hide {
    padding-left: 0px;
  }

  .hideBtn {
    left: 0
  }

  .showBtn {
    left: 207px
  }
</style>
