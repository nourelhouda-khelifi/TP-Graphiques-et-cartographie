<script setup>
 import apexchart from "vue3-apexcharts";
 const series = [
 {
 name: "Ventes",
 data: [ { x: "Jan", y: 10 }, { x: "Fév", y: 20 },{ x: "Mar", y: 15 },
 { x: "Avr", y: 25 }, { x: "Mai", y: 30 }, { x: "Juin", y: 40 }
 ]
 },
 {
 name: "Achats",
 data: [ { x: "Jan", y: 60 }, { x: "Fév", y: 20 },{ x: "Mar", y: 30 },
 { x: "Avr", y: 10 }, { x: "Mai", y: 50 }, { x: "Juin", y: 10 }
 ]
 }
 ];
 // -- les options du graphique
 const options = {
 chart: {
 type : "line", // type de graphique
 },
 stroke: {
 curve: 'smooth', // type de ligne
 },
 markers: {
 size: 5, // taille des marqueurs à chaque point
 },
 }
</script>
<template>
 <div>
 <apexchart width="500" :options="options" :series="series"></apexchart>
 </div>
</template>