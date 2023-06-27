<script setup>
import { ref } from 'vue';

const tab = ref('');

const changeTab = (name) => {
    tab.value = tab.value == '' ? name : ''
}
</script>

<template>
    <div class="text-center sticky bottom-0 bg-white">
        <div :class="{'hidden': tab == '','border-2 h-96': true}">
            <card-footer-calendar v-if="tab == 'calendar'" />
            <card-footer-contact v-if="tab == 'contact'" />
            <card-footer-map v-if="tab == 'map'" />
            <card-footer-note v-if="tab == 'note'" />
        </div>
        <div class="grid grid-flow-col grid-cols-4 grid-rows-1 justify-stretch border-2">
            <div class="border-2 cursor-pointer p-6" @click="changeTab('calendar')">Kalendar</div>
            <div class="border-2 cursor-pointer p-6" @click="changeTab('contact')">Hubungi</div>
            <div class="border-2 cursor-pointer p-6" @click="changeTab('map')">Peta</div>
            <div class="border-2 cursor-pointer p-6" @click="changeTab('note')">Nota</div>
        </div>
        <div class="py-1 text-xs">
            Dihasilkan oleh <a href="https://naimsolong.github.io" target="_blank">Amirul Naim</a>
        </div>
    </div>
</template>