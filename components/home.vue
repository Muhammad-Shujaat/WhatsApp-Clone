<template>
    <div class="" v-if="!RuntimeConfig.public.homeDetails.name">
        <DefaultChat />
    </div>

    <div class="w-full text-center bg-[#eae6df] h-[100vh]" v-if="RuntimeConfig.public.homeDetails.name">
        <OpenChat />
    </div>
    <!-- <div class="">
        <Emojipicker />
    </div> -->

</template>
<script setup>

const RuntimeConfig = useRuntimeConfig()
</script>