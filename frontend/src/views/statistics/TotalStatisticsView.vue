<template>
  <div class="container">
    <h1 class="header-font">About US</h1>
    <div class="row">
        <div class="col-12">
            <div class="p-3 m-3 border bg-light">
            <h4>시간대별 매칭율</h4>
            <time-bar-chart></time-bar-chart>
            </div>
        </div>
        <div class="col bg-dark"></div>
    </div>
    <div class="row">
        <div class="col-6">
            <div class="p-3 m-3 border bg-light">
                <h4>남녀비율</h4>
                <gender-rate-chart></gender-rate-chart>
            </div>
        </div>
        <div class="col-6">
            <div class="p-3 m-3 border bg-light">
                <h4>MBTI Rate Top5</h4>
                <total-mbti-chart></total-mbti-chart>
            </div>
        </div>
    </div>
    <h1 class="header-font mt-5">Teammates</h1>
    <team-intro></team-intro>
  </div>
</template>

<script>
import TimeBarChart from './components/TimeBarChart.vue'
import GenderRateChart from './components/GenderRateChart.vue'
import TotalMbtiChart from './components/TotalMbtiChart.vue'
import TeamIntro from './components/TeamIntro.vue'
export default {
  components: { TimeBarChart, GenderRateChart, TotalMbtiChart, TeamIntro }
}
</script>

<style scoped>
.container {
  border: 2px solid #FAFAFA;
  padding: 30px 30px;
  width: 1000px !important;
  /* height: 550px !important; */
  background: rgba(178, 174, 174, 0.4);
  /* border: 5px solid #2c3e50;
  border-radius: 10px; */
}

.header-font {
  margin-bottom: 20px;
  color: #000000;
}
</style>
