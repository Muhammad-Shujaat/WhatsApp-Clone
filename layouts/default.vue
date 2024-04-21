<template>
    <div class="bg-black">
        <div class="grid grid-cols-3 bg-white ">
            <div class="col-span-1">
                <div class="flex">
                    <div class="w-[14%] p-2 text-center bg-[#f0f2f5] h-[100vh] flex flex-col justify-between ">
                        <LeftSideBar />

                    </div>
                    <div class="w-[86%] bg-white text-center">

                        <slot />
                    </div>
                </div>
            </div>
            <div class="col-span-2">
                <Home />
            </div>
        </div>
    </div>
</template>