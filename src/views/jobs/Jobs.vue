<template>
  <div>
    <h1>Jobs list</h1>
    <!-- when we use v-for directive we've to give a key property which must be unique -->
    <div v-for="job in jobs" :key="job.id">
      <h2>{{ job.title }}</h2>
    </div>
  </div>
</template>

<script setup>
import { reactive } from "vue";
const jobs = reactive([
  {
    id: 1,
    title: "Frontend Developer",
    salary: 1000,
    details: "0-6 months of experience",
  },
  {
    id: 2,
    title: "Backend Developer",
    salary: 2000,
    details: "1 yr of experience",
  },
  {
    id: 3,
    title: "Fullstack Developer",
    salary: 3000,
    details: "6 months-1 yr of experience",
  },
]);
</script>
