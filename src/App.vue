<!-- <template>
  <div class="box">
    <canvas class="box" ref="myChart"></canvas>
  </div>
</template>

<script>
import Chart from "chart.js/auto";
export default {
  mounted() {
    const ctx = this.$refs.myChart.getContext("2d");
    const myChart = new Chart(ctx, {
      type: "bar",
      data: {
        labels: ["jan", "Feb", "Mar", "Apr", "May"],
        datasets: [
          {
            label: "Oylar hisoboti",
            data: [15, 10, 20, 5, 9],
            backgroundColor: [
              "rgba(255, 99, 132, 0.2)",
              "rgba(25, 99, 132, 0.2)",
              "rgba(45, 100, 32, 0.2)",
              "rgba(255, 99, 132, 0.2)",
              "rgba(255, 99, 132, 0.2)",
            ],
            borderColor: [
              "rgba(255, 99, 132, 1)",
              "rgba(255, 99, 132, 1)",
              "rgba(255, 99, 132, 1)",
            ],
            borderWidth: 1,
          },
        ],
      },
    });
  },
};
</script>

<style scoped></style> -->
--> //example-2
<template>
  <div class="box">
    <div class="left-box">
      <canvas ref="myChart"></canvas>
    </div>
    <div class="right-box">
      <h2>Indicator of population of countries in percentage.</h2>
    </div>
  </div>
</template>

<script>
import Chart from "chart.js/auto";
export default {
  mounted() {
    const ctx = this.$refs.myChart.getContext("2d");
    const myChart = new Chart(ctx, {
      type: "pie",
      data: {
        labels: [
          "O'zbekiston",
          "Qozog'iston",
          "Tojikiston",
          "Qirg'iziston",
          "Turkmaniston",
        ],
        datasets: [
          {
            label: "Aholi foizi (%)",
            data: [36155381, 18962892, 8486300, 6550000, 6000000],
            backgroundColor: [
              "rgba(255, 99, 132, 0.8)",
              "rgba(54, 99, 132, 0.8)",
              "rgba(259, 206, 67, 0.8)",
              "rgba(63, 206, 67, 0.8)",
              "rgba(900, 286, 67, 0.8)",
            ],
          },
        ],
      },
    });
  },
};
</script>

<style scoped></style>
