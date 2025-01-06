<template>
    <div class="list">
      <ul>
        <li v-for="(task, index) in tasks" :key="tasks.index">
          {{ task.text }}
          <button @click="deleteTask(task.index)">x</button>
        </li>
      </ul>
    </div>
</template>

<script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    tasks:{
    type: Array,
    required: true
  }
});

    const emit = defineEmits('handleDeletion')
    const deleteTask = (index) => {
      emit('handleDeletion', index)
    }
</script>