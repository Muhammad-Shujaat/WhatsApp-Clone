<template>
    <div class="bg-black">
        <div class="grid grid-cols-3 bg-white ">
            <div class="col-span-1">
                <LeftSideBar />
            </div>
            <div class="col-span-2">
                <slot />
            </div>
        </div>
    </div>
</template>