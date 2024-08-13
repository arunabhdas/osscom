<script setup>
import { ref } from 'vue'
const header = ref('List of components')

const items = ref([
  {id: 1, label: "10 simple list items"},
  {id: 2, label: "5 tile list items"},
  {id: 3, label: "3 scroll list items"}
])

</script>
<template>
  <div class="about">
    <h1>List of components</h1>
    <ul>
      <li v-for="item in items" :key="item.id">{{item.label}}</li>
    </ul>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
