<template>
  <div class="home">
首页

<div id="chart1"></div>
  </div>
</template>

<script>
// @ is an alias to /src
import echarts from 'echarts'

export default {
  data () {
    return {
      chart: ''
    }
  },

  mounted () {
    this.chart = echarts.init(document.getElementById('chart1'))
    var option = {
      xAxis: {
        type: 'category',
        data: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
      },
      yAxis: {
        type: 'value'
      },
      series: [{
        data: [820, 932, 901, 934, 1290, 1330, 1320],
        type: 'line'
      }]
    }
    this.chart.setOption(option)
  }

}
</script>

<style >
  #chart1 {
    height: 400px;
  }
</style>
