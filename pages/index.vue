<template>
    <div class="relative">
        <div class="absolute w-full h-6 z-10 text-xl text-center align-middle inset-1/2 -translate-x-1/2 -translate-y-1/2">
            <span class="px-8 py-2 bg-white border-2">Walimatul Urus</span>
        </div>
        <div class="w-screen h-screen flex flex-col gap-5 p-5">
            <NuxtLink to="/pengantin-lelaki" class="h-1/2">
                <card>
                    <h1>Majlis Pengantin Lelaki</h1>
                </card>
            </NuxtLink>
            <NuxtLink to="/pengantin-perempuan" class="h-1/2">
                <card>
                    <h1>Majlis Pengantin Perempuan</h1>
                </card>
            </NuxtLink>
        </div>
    </div>
</template>
  