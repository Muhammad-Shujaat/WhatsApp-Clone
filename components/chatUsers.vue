<template>
    <div class="w-[86%] bg-white text-center">
        <div class="pl-6 pr-5 py-2 w-full flex justify-between items-center">
            <h1 class="font-bold text-[1.4rem] text-[#111b21] leading-8">Chats</h1>
            <div class="flex text-[#54656f]">
                <div class="p-2 cursor-pointer"><span data-icon="new-chat-outline" class=""><svg viewBox="0 0 24 24"
                            height="24" width="24" preserveAspectRatio="xMidYMid meet" class="" fill="none">
                            <title>new-chat</title>
                            <path
                                d="M9.53277 12.9911H11.5086V14.9671C11.5086 15.3999 11.7634 15.8175 12.1762 15.9488C12.8608 16.1661 13.4909 15.6613 13.4909 15.009V12.9911H15.4672C15.9005 12.9911 16.3181 12.7358 16.449 12.3226C16.6659 11.6381 16.1606 11.0089 15.5086 11.0089H13.4909V9.03332C13.4909 8.60007 13.2361 8.18252 12.8233 8.05119C12.1391 7.83391 11.5086 8.33872 11.5086 8.991V11.0089H9.49088C8.83941 11.0089 8.33411 11.6381 8.55097 12.3226C8.68144 12.7358 9.09947 12.9911 9.53277 12.9911Z"
                                fill="currentColor"></path>
                            <path fill-rule="evenodd" clip-rule="evenodd"
                                d="M0.944298 5.52617L2.99998 8.84848V17.3333C2.99998 18.8061 4.19389 20 5.66665 20H19.3333C20.8061 20 22 18.8061 22 17.3333V6.66667C22 5.19391 20.8061 4 19.3333 4H1.79468C1.01126 4 0.532088 4.85997 0.944298 5.52617ZM4.99998 8.27977V17.3333C4.99998 17.7015 5.29845 18 5.66665 18H19.3333C19.7015 18 20 17.7015 20 17.3333V6.66667C20 6.29848 19.7015 6 19.3333 6H3.58937L4.99998 8.27977Z"
                                fill="currentColor"></path>
                        </svg></span></div>
                <div class="p-2 cursor-pointer">

                    <span data-icon="menu" class=""><svg viewBox="0 0 24 24" height="24" width="24"
                            preserveAspectRatio="xMidYMid meet" class="" version="1.1" x="0px" y="0px"
                            enable-background="new 0 0 24 24">
                            <title>menu</title>
                            <path fill="currentColor"
                                d="M12,7c1.104,0,2-0.896,2-2c0-1.105-0.895-2-2-2c-1.104,0-2,0.894-2,2 C10,6.105,10.895,7,12,7z M12,9c-1.104,0-2,0.894-2,2c0,1.104,0.895,2,2,2c1.104,0,2-0.896,2-2C13.999,9.895,13.104,9,12,9z M12,15 c-1.104,0-2,0.894-2,2c0,1.104,0.895,2,2,2c1.104,0,2-0.896,2-2C13.999,15.894,13.104,15,12,15z">
                            </path>
                        </svg></span>
                </div>
            </div>
        </div>
        <div class="w-full shadow-sm overflow-hidden p-2 text-[#8696a0]">
            <div class="float-right w-[97%] flex">
                <div class="w-full flex bg-[#f0f2f5] p-1 rounded-lg">
                    <div class="mx-3">
                        <div v-if="!searchActive" class="">
                            <span>
                                <svg viewBox="0 0 24 24" height="24" width="24" preserveAspectRatio="xMidYMid meet"
                                    class="" version="1.1" x="0px" y="0px" enable-background="new 0 0 24 24">
                                    <title>search</title>
                                    <path fill="currentColor"
                                        d="M15.009,13.805h-0.636l-0.22-0.219c0.781-0.911,1.256-2.092,1.256-3.386 c0-2.876-2.332-5.207-5.207-5.207c-2.876,0-5.208,2.331-5.208,5.207s2.331,5.208,5.208,5.208c1.293,0,2.474-0.474,3.385-1.255 l0.221,0.22v0.635l4.004,3.999l1.194-1.195L15.009,13.805z M10.201,13.805c-1.991,0-3.605-1.614-3.605-3.605 s1.614-3.605,3.605-3.605s3.605,1.614,3.605,3.605S12.192,13.805,10.201,13.805z">
                                    </path>
                                </svg>
                            </span>
                        </div>
                        <div v-if="searchActive" class="">
                            <span>
                                <svg viewBox="0 0 24 24" height="24" width="24" preserveAspectRatio="xMidYMid meet"
                                    class="" version="1.1" x="0px" y="0px" enable-background="new 0 0 24 24">
                                    <title>search</title>
                                    <path fill="currentColor"
                                        d="M15.009,13.805h-0.636l-0.22-0.219c0.781-0.911,1.256-2.092,1.256-3.386 c0-2.876-2.332-5.207-5.207-5.207c-2.876,0-5.208,2.331-5.208,5.207s2.331,5.208,5.208,5.208c1.293,0,2.474-0.474,3.385-1.255 l0.221,0.22v0.635l4.004,3.999l1.194-1.195L15.009,13.805z M10.201,13.805c-1.991,0-3.605-1.614-3.605-3.605 s1.614-3.605,3.605-3.605s3.605,1.614,3.605,3.605S12.192,13.805,10.201,13.805z">
                                    </path>
                                </svg>
                            </span>
                        </div>
                    </div>
                    <div class="w-full">
                        <input type="text" class="w-full outline-none px-4 bg-[#f0f2f5]"
                            @focus.prevent="searchActive = true" @focusout="searchActive = false" placeholder="Search">
                    </div>
                    <div v-if="searchActive" class="px-1"><span>
                            <svg viewBox="0 0 24 24" height="24" width="24" preserveAspectRatio="xMidYMid meet" class=""
                                version="1.1" x="0px" y="0px" enable-background="new 0 0 24 24">
                                <title>x-alt</title>
                                <path fill="currentColor"
                                    d="M17.25,7.8L16.2,6.75l-4.2,4.2l-4.2-4.2L6.75,7.8l4.2,4.2l-4.2,4.2l1.05,1.05l4.2-4.2l4.2,4.2l1.05-1.05 l-4.2-4.2L17.25,7.8z">
                                </path>
                            </svg>
                        </span></div>
                </div>
                <div class="w-auto">
                    <span class="flex justify-center items-center mt-1 px-2">
                        <svg viewBox="0 0 24 24" height="20" width="20" preserveAspectRatio="xMidYMid meet" class=""
                            fill="none">
                            <title>filter</title>
                            <path
                                d="M11 18C10.7167 18 10.4792 17.9042 10.2875 17.7125C10.0958 17.5208 10 17.2833 10 17C10 16.7167 10.0958 16.4792 10.2875 16.2875C10.4792 16.0958 10.7167 16 11 16H13C13.2833 16 13.5208 16.0958 13.7125 16.2875C13.9042 16.4792 14 16.7167 14 17C14 17.2833 13.9042 17.5208 13.7125 17.7125C13.5208 17.9042 13.2833 18 13 18H11ZM7 13C6.71667 13 6.47917 12.9042 6.2875 12.7125C6.09583 12.5208 6 12.2833 6 12C6 11.7167 6.09583 11.4792 6.2875 11.2875C6.47917 11.0958 6.71667 11 7 11H17C17.2833 11 17.5208 11.0958 17.7125 11.2875C17.9042 11.4792 18 11.7167 18 12C18 12.2833 17.9042 12.5208 17.7125 12.7125C17.5208 12.9042 17.2833 13 17 13H7ZM4 8C3.71667 8 3.47917 7.90417 3.2875 7.7125C3.09583 7.52083 3 7.28333 3 7C3 6.71667 3.09583 6.47917 3.2875 6.2875C3.47917 6.09583 3.71667 6 4 6H20C20.2833 6 20.5208 6.09583 20.7125 6.2875C20.9042 6.47917 21 6.71667 21 7C21 7.28333 20.9042 7.52083 20.7125 7.7125C20.5208 7.90417 20.2833 8 20 8H4Z"
                                fill="currentColor"></path>
                        </svg>
                    </span>
                </div>

            </div>
        </div>
        <div class="w-full min-h-[83vh] overflow-y-scroll">
            <ChatUser v-for="(u, i) in userArray" :key="i" :img="u.img" :number="u.nmber" :name="u.name"
                :time="u.last_msg_time" :last_msg="u.last_msg" />

        </div>
    </div>
</template>
<script setup>
const searchActive = ref(false)
const hour = new Date(Date.now()).getHours()
const minute = new Date(Date.now()).getMinutes()
const userArray = ([
    {
        img: "file.jpg",
        name: "shuju",
        last_msg: "last message",
        last_msg_time: hour + ":" + minute,
        nmber: "03554296593"
    }, {
        img: "file.jpg",
        name: "Arif",
        last_msg: "last message",
        last_msg_time: hour + ":" + minute,
        nmber: "03554296593"
    }, {
        img: "file.jpg",
        name: "sanoo",
        last_msg: "last message",
        last_msg_time: hour + ":" + minute,
        nmber: "03554296593"
    }, {
        img: "file.jpg",
        name: "roqi",
        last_msg: "last message",
        last_msg_time: hour + ":" + minute,
        nmber: "03554296593"
    }
])
</script>