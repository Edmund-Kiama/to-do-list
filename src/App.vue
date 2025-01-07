<template>
  <div id="toDoList">
    <Header></Header>
    <task-list :tasks="tasks" @handle-deletion="deleteTask"></task-list>
    <add-list @adding-new-task="handleAddingNewTask" ></add-list>
</div>
</template>

<script setup>
import Header from './components/Header.vue';
import TaskList from './components/TaskList.vue';
import AddList from './components/AddList.vue';

import {ref} from 'vue';


const tasks = ref([]);


//Add task
const handleAddingNewTask = (newList) => {
  tasks.value.push({
    index: generateIndex(),
    text: newList
  })
};

//delete task
const deleteTask = (index) => {
  tasks.value = tasks.value.filter((tasks) => tasks.index !== index)
};

//generate index
const generateIndex = () => {
  return Math.floor(Math.random() * 1000000)
}
</script>