<script setup>
import { ref } from 'vue'
const header = ref('List of components')

const items = ref([
  {id: 1, label: "10 simple list items"},
  {id: 2, label: "5 tile list items"},
  {id: 3, label: "3 scroll list items"}
])

const default_items = ref({
  'item-1': {id: 1, label: "RecyclerView"},
  'item-2': {id: 2, label: "ScrollView"},
  'item-3': {id: 3, label: "ListView"}
})

const newItem = ref("")

const newItemPriority = ref("low")

</script>
<template>
  <div class="about">
    <h1>{{ header }}</h1>
    <input v-model.trim="newItem" type="text" placeholder="Add an item">
    newItemPriority
    <select v-model="newItemPriority">
      <option value="low">Low</option>
      <option value="high">High</option>
    </select>
    {{newItem}}
    <br/>
    {{newItemPriority}}
    <ul>
      <li v-for="({id, label}, index) in items" :key="id">
        {{label}}
      </li>
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
