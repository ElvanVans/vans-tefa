<template>
    <div>
        <canvas id="statistik"></canvas>
    </div>
</template>

<script setup>
import Chart from 'chart.js/auto'

const labels = [
    'Januari',
    'Februari',
    'Maret',
    'April',
    'Mei',
    'Juni',
    'Juli',
    'Agustus',
    'September',
    'Oktober',
    'November',
    'Desember'
  ];

  const data = {
    labels: labels,
    datasets: [{
      label: 'Pengunjung',
      data: [1, 5, 7, 4, 10, 6, 3, 2, 8, 9, 0, 0],
      backgroundColor: [
      'rgb(255, 00, 00)',
        'rgb(255, 255, 00)',
        'rgb(00, 255, 00)',
        'rgb(255, 00, 00)',
        'rgb(255,00, 00)',
        'rgb(00,255, 00)'
    ],
    }]
  };

  const config = {
    type: 'bar',
    data: data,
    options: {}
  };


onMounted(() => {
  const myChart = new Chart(
    document.getElementById('statistik'),
    config
  );
})
</script>