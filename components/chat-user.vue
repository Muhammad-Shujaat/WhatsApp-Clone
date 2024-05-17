<template>
    <div class="w-full h-[4.5rem] flex items-center overflow-hidden cursor-pointer hover:bg-[#f5f6f6]">
        <div class=" flex justify-center items-center w-1/5 h-full p-3">
            <NuxtImg class="rounded-full" :src="`/${img}`" />
        </div>
        <div class="w-4/5 flex flex-col" @click.prevent="openChat(img, name, last_msg, number)">
            <div class=" w-full text-start flex justify-between">
                <span class="">{{ `${name}` }}</span>
                <span class="text-xs px-2 flex flex-col">
                    {{ time }}
                </span>

            </div>
            <div class="w-full text-start flex justify-between">
                <span class="">{{ `${last_msg}` }}</span>
                <span class="text-xs px-2 flex flex-col">
                    <span data-icon="down" class="opacity-0 hover:opacity-60"><svg viewBox="0 0 19 20" height="20"
                            width="19" preserveAspectRatio="xMidYMid meet" class="" version="1.1" x="0px" y="0px">
                            <title>down</title>
                            <path fill="currentColor" d="M3.8,6.7l5.7,5.7l5.7-5.7l1.6,1.6l-7.3,7.2L2.2,8.3L3.8,6.7z">
                            </path>
                        </svg></span>
                </span>

            </div>
        </div>
    </div>
</template>
<script setup>



defineProps({
    img: String,
    name: String,
    time: String,
    last_msg: String,
    number: String

})
function openChat(img, name, last_msg, number) {
    console.log("sdkjfljdlf", img, name, last_msg, number);
    const RuntimeConfig = useRuntimeConfig()
    RuntimeConfig.public.homeDetails.name = name;
    RuntimeConfig.public.homeDetails.chatss = last_msg;
    RuntimeConfig.public.homeDetails.userNumber = number;
    RuntimeConfig.public.homeDetails.userPic = img;
    console.log("sdkjfljdlf", img, name, last_msg, number);

}
</script>