<script setup>
const props = defineProps({
    calendar: Object
})
</script>

<template>
    <div class="text-white">
        <p class="text-xl mb-9">Kalendar</p>
        {{ props.calendar.day }}
        {{ props.calendar.date.masihih }}
        {{ props.calendar.date.hijrah }}
        {{ props.calendar.time }}
    </div>
</template>