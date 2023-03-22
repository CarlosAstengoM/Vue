<!-- Copyright(c) 2023, Carlos Astengo, All Rights Reserved -->

<script setup>
    import BarChart from "../components/chartTypes/BarChart.vue"
    import BubbleChart from "../components/chartTypes/BubbleChart.vue"
    import LineChart from "../components/chartTypes/LineChart.vue"
    import PieChart from "../components/chartTypes/PieChart.vue"
    import TrendlineChart from "../components/chartTypes/TrendlinesChart.vue"
</script>

<template>
    <div class="chart-grid">        
        <BarChart />
        <BubbleChart />
        <LineChart />
        <PieChart />
        <TrendlineChart />
    </div>
</template>

<style>
    .chart-grid
    {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-between;
    }
</style>
