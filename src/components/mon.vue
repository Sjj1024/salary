<script setup lang="ts">
import mon from "../assets/svgmon.svg";

defineProps<{
  msg: {
    year: string;
    month: string;
    day: string;
    week: string;
    times: string;
    pay: string;
    residue: string;
    name: string;
    card: string;
  };
}>();

// const count = ref(0);
</script>

<template>
  <div class="box">
    <div class="it-header">
      <div class="times">
        <span>{{ msg.year }}年 </span>
        <span class="month-info">{{ msg.month }}月{{ msg.day }}日</span>
      </div>
      <div class="sum">详情</div>
    </div>

    <div class="main">
      <div class="company">
        <div class="com-name">{{ msg.name }}</div>
        <div class="com-sail">
          <!-- <img src="../assets/icon2.png" alt="" class="icon-mon" /> -->
          <img :src="mon" alt="" class="icon-mon" />
          <!-- <object
            data="../assets/svgmon.svg"
            type="image/svg+xml"
            class="icon-mon"
          ></object> -->
          <!-- <embed
            src="../assets/svgmon.svg"
            type="image/svg+xml"
            class="icon-mon"
          /> -->
          <div>工资</div>
        </div>
      </div>
      <div>
        <div class="sales">
          <div class="sal-add">+￥{{ msg.pay }}</div>
          <div class="sal-end">余额:￥{{ msg.residue }}</div>
        </div>
        <div></div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.box {
  width: 100%;
  height: 130px;
  margin-bottom: 5px;
  background-color: #fff;
  padding: 12px;
  border-radius: 15px;
}

.month-info {
  font-size: 16px;
  font-weight: 400;
  color: gray;
}

.it-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.icon-mon {
  width: 18px;
  height: 18px;
  margin-right: 10px;
}

.sum {
  color: gray;
}

.times {
  font-size: 24px;
  font-weight: 600;
  color: #333;
}

.main {
  display: flex;
  justify-content: space-between;
  margin-top: 8px;
}

.com-name,
.sal-add {
  color: #121212;
  font-size: 17px;
  text-align: left;
}

.sal-add,
.sal-end {
  text-align: end;
}

.com-sail {
  font-weight: 700;
  display: flex;
  align-items: center;
}

.com-sail,
.sal-end {
  margin-top: 10px;
  color: gray;
  font-size: 14px;
}
</style>
