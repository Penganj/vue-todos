<script setup>
const props = defineProps({
    todo: {
        type: Object,
        required: true,
    }
})
</script>

<template>
    <li>
        <input type="checkbox" :checked="todo.isCompleted" />
        <div class="todo">
            <input type="text" :value="todo.todo" />
            <span>
                {{ todo.todo }}
            </span>
        </div>
    </li>
</template>

<style scoped>

</style>