<script setup lang="ts">
    import ContactIcons from './ContactIcons.vue';
    const scrollToTop = () => {
        document.querySelector('#topbar')?.scrollIntoView({ behavior: 'smooth', block: 'end' })
    }
</script>

<template>
    <div class="mx-8 py-2 relative grid grid-cols-1 sm:grid-cols-3 gap-2 flex">

        <ContactIcons class="order-last sm:order-first flex items-center justify-center sm:justify-start gap-2" size="h-8 w-8" />

        <div class="col-span-1 flex flex-col items-center text-outline-white whitespace-nowrap">
            <p class="font-shrikhand font-normal text-xl">Clube Rainbow</p>
            <p class="text-sm">rainbow.clube.estudantes@gmail.com</p>
        </div>

        <button class="absolute right-0 top-4 flex items-center justify-end hover:brightness-110" @click="scrollToTop()">
            <img src="../assets/icon_up.svg" alt="scroll up" class="h-8 w-8"/>
        </button>
        
    </div>
</template>