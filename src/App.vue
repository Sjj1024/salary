<script setup lang="ts">
import Month from "./components/mon.vue";

// 从2020年到2022年10工资
const monthMoney = [
  {
    year: "2022",
    month: "10",
    day: "17",
    week: "周三",
    times: "10:52",
    pay: "16,754.11",
    residue: "17,243.01",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "9",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "21,658.23",
    residue: "27,873.09",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "8",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "19,921.05",
    residue: "20,545.23",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "7",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "19,136.86",
    residue: "20,945.21",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "6",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "21,348.52",
    residue: "30,459.03",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "5",
    day: "16",
    week: "周三",
    times: "10:52",
    pay: "23,566.81",
    residue: "27,351.95",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "4",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "20,239.27",
    residue: "45,539.34",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "3",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "19,834.01",
    residue: "32,943.23",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "2",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "80,356.36",
    residue: "103,592.37",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "2",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "19,385.45",
    residue: "23,236.01",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2022",
    month: "1",
    day: "17",
    week: "周三",
    times: "10:52",
    pay: "18,349.65",
    residue: "21,942.68",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "12",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "19,190.35",
    residue: "20,553.86",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "11",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "19,245.68",
    residue: "19,373.05",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "10",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "17,834.42",
    residue: "17,904.31",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "9",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "17,754.64",
    residue: "19,671.33",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "8",
    day: "16",
    week: "周三",
    times: "10:52",
    pay: "17,462.30",
    residue: "20,632.23",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "7",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "17,640.09",
    residue: "18,032.93",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "6",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "17,092.15",
    residue: "18,529.62",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "5",
    day: "17",
    week: "周三",
    times: "10:52",
    pay: "17,035.71",
    residue: "17,210.60",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "4",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "18,298.52",
    residue: "18,427.02",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "3",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "17,562.56",
    residue: "17,852.22",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "2",
    day: "18",
    week: "周三",
    times: "10:52",
    pay: "65,005.82",
    residue: "82,267.46",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "2",
    day: "18",
    week: "周三",
    times: "10:52",
    pay: "17,005.82",
    residue: "17,262.64",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2021",
    month: "1",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "16,064.41",
    residue: "17,661.67",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "12",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "17,232.45",
    residue: "19,912.02",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "11",
    day: "16",
    week: "周三",
    times: "10:52",
    pay: "16,274.10",
    residue: "20,892.62",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "10",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "16,892.02",
    residue: "17,982.32",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "9",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "16,265.31",
    residue: "16,268.34",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "8",
    day: "17",
    week: "周三",
    times: "10:52",
    pay: "16,391.52",
    residue: "18,901.31",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "7",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "17,601.28",
    residue: "17,614.20",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "6",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "16,756.12",
    residue: "16,758.46",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "5",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "16,846.15",
    residue: "16,961.53",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "4",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "16,807.62",
    residue: "17,647.58",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "3",
    day: "16",
    week: "周三",
    times: "10:52",
    pay: "16,091.11",
    residue: "17,821.26",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "2",
    day: "17",
    week: "周三",
    times: "10:52",
    pay: "60,920.61",
    residue: "87,599.17",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "2",
    day: "17",
    week: "周三",
    times: "10:52",
    pay: "16,920.61",
    residue: "26,678.56",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2020",
    month: "1",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "17,346.83",
    residue: "17,873.64",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2019",
    month: "12",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "19,754.11",
    residue: "7,873.13",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2019",
    month: "11",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "19,754.11",
    residue: "7,873.63",
    name: "上海华为技术有限公司",
    card: "4916",
  },
  {
    year: "2019",
    month: "10",
    day: "15",
    week: "周三",
    times: "10:52",
    pay: "12,754.11",
    residue: "27,873.13",
    name: "上海华为技术有限公司",
    card: "4916",
  },
];
</script>

<template>
  <div class="main">
    <img src="./assets/header.png" class="header" />
    <div class="item-box">
      <div class="item" v-for="month in monthMoney" :key="month.pay">
        <Month :msg="month" />
      </div>
    </div>
    <img src="./assets/footer.png" class="footer" />
  </div>
</template>

<style scoped>
.main {
  width: 100%;
  height: 100%;
  padding: 90px 0 0 0;
  position: relative;
  background-color: #f8f8f8;
}

.item-box {
  height: 100%;
  background-color: #f8f8f8;
  overflow-y: scroll;
  padding-bottom: 90px;
}

.header {
  position: absolute;
  top: 0;
  width: 100%;
  height: 74px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: top center;
  background-image: url("./assets/header.png");
}

.footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 76px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: top center;
  background-image: url("./assets/footer.png");
}

.item {
  padding: 10px;
}
</style>
