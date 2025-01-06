<template>
    <div class="title">
    <h1>To-do-List</h1>
  </div>
  <div class="for-the-day">
    <h2>For the Day</h2>
    <h4>{{ day }}</h4>
  </div>
</template>

<script setup>
    const day = new Date()
</script>