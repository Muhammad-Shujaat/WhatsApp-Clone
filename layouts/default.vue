<template>
    <div class="grid grid-cols-3 bg-white ">
        <div class="col-span-1">
            <div class="flex">
                <LeftSideBar />
                <slot />
            </div>
        </div>
        <div class="col-span-2">
            <Home />
        </div>
    </div>
</template>