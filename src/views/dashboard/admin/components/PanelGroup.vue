<template>
  <el-row :gutter="40" class="panel-group">
    <el-col :xs="6" :sm="6" :lg="6" class="card-panel-col">
      <div class="card-panel">
        <div class="card-panel-icon-wrapper icon-people">
          <!--<svg-icon icon-class="peoples" class-name="card-panel-icon" />-->
          <img src="../../../../assets/other_image/touxiang.png" style="vertical-align: middle;">
        </div>
        <div class="card-panel-description">
          <div class="card-panel-text">
            <p>奕江科技</p>
            <p>13355558888</p>
          </div>
          <!--<count-to :start-val="0" :end-val="102400" :duration="2600" class="card-panel-num" />-->
        </div>
      </div>
    </el-col>
    <el-col :xs="18" :sm="18" :lg="18" class="card-panel-col">
      <div class="card-panel">
        <div class="card-panel-icon-wrapper icon-people" style="margin:0 auto;width:47%;height:100%;">
          <div style="margin:13% 0 0 33%;">
            <img src="../../../../assets/other_image/cunzheng_2.png" style="margin:0 12px 4px 0;vertical-align: middle;">
            <span style="font-size:18px;">区块链版权存证</span>
          </div>
        </div>
        <b style="display:inline-block;height:73%;border-left:2px solid #eee;margin:24px;"></b>
        <div class="card-panel-description" style="width:47%;height:100%;margin:0 auto;padding:16px;">
          <div class="card-panel-text" style="margin:14% 0 0 40%;">
            <h1 style="font-size:60px;color:#10429a;font-weight:400;">18</h1>
          </div>
        </div>
      </div>
    </el-col>
  </el-row>
</template>

<script>
import CountTo from 'vue-count-to'

export default {
  components: {
    CountTo
  },
  methods: {
//    handleSetLineChartData(type) {
//      this.$emit('handleSetLineChartData', type)
//    }
  }
}
</script>

<style lang="scss" scoped>
.panel-group {
  //margin-top: 18px;

  .card-panel-col {
    margin-bottom: 24px;
  }

  .card-panel {
    height: 180px;
    cursor: pointer;
    font-size: 12px;
    position: relative;
    overflow: hidden;
    color: #666;
    background: #fff;
    box-shadow: 4px 4px 40px rgba(0, 0, 0, .05);
    border-color: rgba(0, 0, 0, .05);

    /*&:hover {*/
      /*.card-panel-icon-wrapper {*/
        /*color: #fff;*/
      /*}*/

      /*.icon-people {*/
        /*background: #40c9c6;*/
      /*}*/

      /*.icon-message {*/
        /*background: #36a3f7;*/
      /*}*/

      /*.icon-money {*/
        /*background: #f4516c;*/
      /*}*/

      /*.icon-shopping {*/
        /*background: #34bfa3*/
      /*}*/
    /*}*/

    /*.icon-people {*/
      /*color: #40c9c6;*/
    /*}*/

    /*.icon-message {*/
      /*color: #36a3f7;*/
    /*}*/

    /*.icon-money {*/
      /*color: #f4516c;*/
    /*}*/

    /*.icon-shopping {*/
      /*color: #34bfa3*/
    /*}*/

    .card-panel-icon-wrapper {
      float: left;
      margin: 30px 0 0 30px;
      padding: 16px;
      transition: all 0.38s ease-out;
      border-radius: 6px;
    }

    .card-panel-icon {
      float: left;
      font-size: 48px;
    }

    .card-panel-description {
      float: right;
      font-weight: bold;
      margin: 40px;
      margin-left: 0px;

      .card-panel-text {
        line-height: 18px;
        color: rgba(0, 0, 0, 0.45);
        font-size: 16px;
        margin-bottom: 12px;
      }

      .card-panel-num {
        font-size: 20px;
      }
    }
  }
}

@media (max-width:550px) {
  .card-panel-description {
    display: none;
  }

  .card-panel-icon-wrapper {
    float: none !important;
    width: 100%;
    height: 100%;
    margin: 0 !important;

    .svg-icon {
      display: block;
      margin: 14px auto !important;
      float: none !important;
    }
  }
}
</style>
