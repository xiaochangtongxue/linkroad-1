<template>
  <div style="width:92%;height:28vh;background-color:rgba(255,255,255,0.7);margin-top:2vh;margin-left:2vh;box-shadow:0 0 2px 2px #2CF8DE">
    <div id="chartRam" :style="{width: '98%', height: '100%'}"></div>
  </div>
</template>

<script>
    export default {
        name: "Ram",
        props:[
          'code',
          "time"
        ],
      methods:{
          test(){
            console.log(222)
          },
          draw(){
            let chartRam = this.$echarts.init(document.getElementById('chartRam'));
            let option = {
              title: {
                text: 'TOP5-内存使用情况',
                textStyle: {
                  fontSize:'12'
                },
              },
              tooltip: {
                trigger: 'axis'
              },
              legend: {
                // orient: 'vertical',
                x:'left',      //可设定图例在左、右、居中
                y:'top',     //可设定图例在上、下、居中
                padding:[18,0,0,15],   //可设定图例[距上方距离，距右方距离，距下方距离，距左方距离]
                data: ['邮件营销', '联盟广告', '视频广告', '直接访问', '搜索引擎']
              },
              grid: {
                left: '3%',
                right: '4%',
                bottom: '3%',
                containLabel: true
              },
              xAxis: {
                type: 'category',
                boundaryGap: false,
                data: ['周一', '周二', '周三', '周四', '周五', '周六', '周日']
              },
              yAxis: {
                type: 'value'
              },
              series: [
                {
                  name: '邮件营销',
                  type: 'line',
                  stack: '总量',
                  data: [120, 132, 101, 134, 90, 230, 210]
                },
                {
                  name: '联盟广告',
                  type: 'line',
                  stack: '总量',
                  data: [220, 182, 191, 234, 290, 330, 310]
                },
                {
                  name: '视频广告',
                  type: 'line',
                  stack: '总量',
                  data: [150, 232, 201, 154, 190, 330, 410]
                },
                {
                  name: '直接访问',
                  type: 'line',
                  stack: '总量',
                  data: [320, 332, 301, 334, 390, 330, 320]
                },
                {
                  name: '搜索引擎',
                  type: 'line',
                  stack: '总量',
                  data: [820, 932, 901, 934, 1290, 1330, 1320]
                }
              ]
            };
            chartRam.setOption(option, true);
        }
      },
      watch:{
          code: function (value) {
            console.log(value)
            console.log(this.time)
          },
          time:function (value) {
            console.log(this.code)
            console.log(value)
          }
      },
      mounted() {
          console.log(this.code)
          console.log(this.time)
         this.draw() //函数调用
      }
    }
</script>

<style scoped>

</style>
