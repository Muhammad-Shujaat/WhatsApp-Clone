<template>
        <div class="w-full grid grid-rows-11 h-[100vh] ">
                <!-- head area -->
                <div class="w-full row-start-1 bg-[#f0f2f5] p-3 h-[3.5rem] flex justify-between items-center">
                        <div class="flex items-center gap-3 cursor-pointer">
                                <NuxtImg class="rounded-full w-10" :src="RuntimeConfig.public.homeDetails.userPic" />
                                <div class="flex flex-col items-start">
                                        <span class="text-[1rem] leading-4">{{ RuntimeConfig.public.homeDetails.name
                                                }}</span>
                                        <p class="text-xs text-[#3b4a54] ">{{
                                                RuntimeConfig.public.homeDetails.userNumber }}</p>
                                </div>
                        </div>

                        <div class="flex items-center gap-6 px-6 text-[#3b4a54]">
                                <div class="">
                                        <button class="" tabindex="0" data-tab="6" title="Get the app for calling"
                                                type="button" aria-label="Get the app for calling">
                                                <div class="flex flex-col justify-center items-center">
                                                        <span data-icon="video-call" class="">
                                                                <svg viewBox="0 0 24 24" height="22" width="22"
                                                                        preserveAspectRatio="xMidYMid meet" class=""
                                                                        fill="none">
                                                                        <title>video-call</title>
                                                                        <path d="M3.27096 7.31042C3 7.82381 3 8.49587 3 9.84V14.16C3 15.5041 3 16.1762 3.27096 16.6896C3.5093 17.1412 3.88961 17.5083 4.35738 17.7384C4.88916 18 5.58531 18 6.9776 18H13.1097C14.502 18 15.1982 18 15.7299 17.7384C16.1977 17.5083 16.578 17.1412 16.8164 16.6896C17.0873 16.1762 17.0873 15.5041 17.0873 14.16V9.84C17.0873 8.49587 17.0873 7.82381 16.8164 7.31042C16.578 6.85883 16.1977 6.49168 15.7299 6.26158C15.1982 6 14.502 6 13.1097 6H6.9776C5.58531 6 4.88916 6 4.35738 6.26158C3.88961 6.49168 3.5093 6.85883 3.27096 7.31042Z"
                                                                                fill="currentColor"></path>
                                                                        <path d="M18.7308 9.60844C18.5601 9.75994 18.4629 9.97355 18.4629 10.1974V13.8026C18.4629 14.0264 18.5601 14.2401 18.7308 14.3916L20.9567 16.3669C21.4879 16.8384 22.3462 16.4746 22.3462 15.778V8.22203C22.3462 7.52542 21.4879 7.16163 20.9567 7.63306L18.7308 9.60844Z"
                                                                                fill="currentColor"></path>
                                                                </svg>
                                                        </span>
                                                        <span data-icon="chevron-down-alt" class="">
                                                                <svg viewBox="0 0 17 13" height="8"
                                                                        preserveAspectRatio="xMidYMid meet" class=""
                                                                        version="1.1" x="0px" y="0px"
                                                                        enable-background="new 0 0 17 13">
                                                                        <title>chevron-down-alt</title>
                                                                        <path fill="currentColor"
                                                                                d="M3.202,2.5l5.2,5.2l5.2-5.2l1.5,1.5l-6.7,6.5l-6.6-6.6L3.202,2.5z">
                                                                        </path>
                                                                </svg>
                                                        </span>
                                                </div>
                                        </button>
                                </div>
                                <div class="">
                                        <div aria-disabled="false" role="button" tabindex="0" class="" data-tab="6"
                                                title="Search…" aria-label="Search…"><span data-icon="search-alt"
                                                        class=""><svg viewBox="0 0 26 26" height="24" width="24"
                                                                preserveAspectRatio="xMidYMid meet" class=""
                                                                version="1.1" x="0px" y="0px"
                                                                enable-background="new 0 0 24 24">
                                                                <title>search-alt</title>
                                                                <path fill="currentColor"
                                                                        d="M15.9,14.3H15L14.7,14c1-1.1,1.6-2.7,1.6-4.3c0-3.7-3-6.7-6.7-6.7S3,6,3,9.7 s3,6.7,6.7,6.7c1.6,0,3.2-0.6,4.3-1.6l0.3,0.3v0.8l5.1,5.1l1.5-1.5L15.9,14.3z M9.7,14.3c-2.6,0-4.6-2.1-4.6-4.6s2.1-4.6,4.6-4.6 s4.6,2.1,4.6,4.6S12.3,14.3,9.7,14.3z">
                                                                </path>
                                                        </svg></span></div><span class=""></span>
                                </div>
                                <div class="">
                                        <div class="">
                                                <div aria-disabled="false" role="button" tabindex="0" class=""
                                                        data-tab="6" title="Menu" aria-label="Menu">
                                                        <span data-icon="menu" class=""><svg viewBox="0 0 24 24"
                                                                        height="24" width="24"
                                                                        preserveAspectRatio="xMidYMid meet" class=""
                                                                        version="1.1" x="0px" y="0px"
                                                                        enable-background="new 0 0 24 24">
                                                                        <title>menu</title>
                                                                        <path fill="currentColor"
                                                                                d="M12,7c1.104,0,2-0.896,2-2c0-1.105-0.895-2-2-2c-1.104,0-2,0.894-2,2 C10,6.105,10.895,7,12,7z M12,9c-1.104,0-2,0.894-2,2c0,1.104,0.895,2,2,2c1.104,0,2-0.896,2-2C13.999,9.895,13.104,9,12,9z M12,15 c-1.104,0-2,0.894-2,2c0,1.104,0.895,2,2,2c1.104,0,2-0.896,2-2C13.999,15.894,13.104,15,12,15z">
                                                                        </path>
                                                                </svg>
                                                        </span>
                                                </div>
                                        </div>
                                </div>
                        </div>

                </div>

                <!-- messges area -->
                <div class="w-full row-start-2 row-end-11 overflow-y-scroll scroll-smooth p-4 flex flex-col gap-2">
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjjldsfldfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdlskdjflkfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjs;dflkjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjlksdjflfkljdldfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdsdjfkahsjkfksjdfklsdaflfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdsjkdhflhaffhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-right"><span
                                        class=" rounded-lg text-xs leading-4 py-1.5 bg-[#d9fdd3] px-2.5">ksjdfhjdf</span>
                        </div>
                        <div class="w-full text-left"><span
                                        class="bg-white rounded-lg text-xs leading-4 py-1.5 px-2.5">ksjdfhjdf</span>
                        </div>
                </div>

                <!-- msg sending area -->
                <div class="w-full row-start-11 bg-[#f0f2f5] h-[3.5rem] flex items-center gap-4 px-6 py-1">
                        <div class="">
                                <span data-icon="smiley" class="text-[#869690] cursor-pointer"><svg viewBox="0 0 24 24"
                                                height="24" width="24" preserveAspectRatio="xMidYMid meet"
                                                class="x23j0i4 xd7y6wv" version="1.1" x="0px" y="0px"
                                                enable-background="new 0 0 24 24">
                                                <title>Emoji</title>
                                                <path fill="currentColor"
                                                        d="M9.153,11.603c0.795,0,1.439-0.879,1.439-1.962S9.948,7.679,9.153,7.679 S7.714,8.558,7.714,9.641S8.358,11.603,9.153,11.603z M5.949,12.965c-0.026-0.307-0.131,5.218,6.063,5.551 c6.066-0.25,6.066-5.551,6.066-5.551C12,14.381,5.949,12.965,5.949,12.965z M17.312,14.073c0,0-0.669,1.959-5.051,1.959 c-3.505,0-5.388-1.164-5.607-1.959C6.654,14.073,12.566,15.128,17.312,14.073z M11.804,1.011c-6.195,0-10.826,5.022-10.826,11.217 s4.826,10.761,11.021,10.761S23.02,18.423,23.02,12.228C23.021,6.033,17.999,1.011,11.804,1.011z M12,21.354 c-5.273,0-9.381-3.886-9.381-9.159s3.942-9.548,9.215-9.548s9.548,4.275,9.548,9.548C21.381,17.467,17.273,21.354,12,21.354z  M15.108,11.603c0.795,0,1.439-0.879,1.439-1.962s-0.644-1.962-1.439-1.962s-1.439,0.879-1.439,1.962S14.313,11.603,15.108,11.603z">
                                                </path>
                                        </svg></span>
                        </div>
                        <div class="w-full">
                                <input class="w-full h-10 outline-none px-4 text-[#3b4a54] py-1 rounded-lg text-sm leading-4 bg-white"
                                        type="text" placeholder=" Type a message">

                        </div>
                        <div class="">
                                <span data-icon="send" class="text-[#869690] cursor-pointer"><svg viewBox="0 0 24 24"
                                                height="24" width="24" preserveAspectRatio="xMidYMid meet" class=""
                                                version="1.1" x="0px" y="0px" enable-background="new 0 0 24 24">
                                                <title>send</title>
                                                <path fill="currentColor"
                                                        d="M1.101,21.757L23.8,12.028L1.101,2.3l0.011,7.912l13.623,1.816L1.112,13.845 L1.101,21.757z">
                                                </path>
                                        </svg></span>
                        </div>

                </div>
        </div>
</template>
<script setup>
const RuntimeConfig = useRuntimeConfig()


</script>