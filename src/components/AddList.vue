<template>
    <form class="add-new-task" @submit.prevent="addNewTask">
      <label class="label" for="newTask">New Task</label>
      <input id="newTask" type="text" placeholder="Add a new task" class="input-new-task" v-model="text">
      <button type="submit">Add</button>
    </form>
</template>

<script setup>
  import {ref} from 'vue';

  const text = ref('');

  const emit = defineEmits('addingNewTask');
  const addNewTask = () => {
    if (!text.value){
      alert('Please add task')
      return;
    }
    const newList = text.value;
    emit('addingNewTask',newList)    

    text.value=''
  };
</script>