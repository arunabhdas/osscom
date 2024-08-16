<script setup>
import { ref } from 'vue'
const header = ref('Contact')

const items = ref([
    { id: 1, label: "10 simple list items" },
    { id: 2, label: "5 tile list items" },
    { id: 3, label: "3 scroll list items" }
])

const default_items = ref({
    'item-1': { id: 1, label: "RecyclerView" },
    'item-2': { id: 2, label: "ScrollView" },
    'item-3': { id: 3, label: "ListView" }
})

const newItem = ref("")

const newItemPriority = ref("low")

const newItemDoneState = ref(false)

const newItemHighPriority = ref(false)

</script>
<template>
    <div class="contact">
        <h1>{{ header }}</h1>
        <div class="add-item-form">

            <input v-model.trim="newItem" type="text" placeholder="Add an item">
            newItemPriority
            {{ newItem }}
            <label>
                <input type="checkbox" v-model="newItemHighPriority">
                High Priority
            </label>
            <button 
                v-on:click="items.push({id: items.length + 1, label: newItem})" 
                class="btn btn-primary">
                Save
            </button>
            <br />
        </div>
        <ul>
            <li v-for="({ id, label }, index) in items" :key="id">
                {{ label }}
            </li>
        </ul>
    </div>
</template>

<style>
@media (min-width: 1024px) {
    .contact {
        min-height: 100vh;
        display: flex;
        align-items: center;
    }
}
</style>
