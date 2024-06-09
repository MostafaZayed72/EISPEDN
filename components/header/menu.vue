<template>
    <div id="main-menu" class="wsmainfull menu clearfix ">
        <div class="wsmainwp clearfix">
            <!-- HEADER BLACK LOGO -->
            <div class="desktoplogo">
                <NuxtLink to="/" class="logo-black"><img src="/assets/images/EISPEDN-EN-Logo.png" alt="logo" /></NuxtLink>
            </div>
            <!-- HEADER WHITE LOGO -->
            <div class="desktoplogo">
                <NuxtLink to="/" class="logo-white"><img src="/assets/images/EISPEDN-EN-Logo.png" alt="logo" /></NuxtLink>
            </div>
            <!-- MAIN MENU -->
            <nav class="wsmenu clearfix">
                <ul class="wsmenu-list nav-theme">
                    <!-- DROPDOWN SUB MENU -->
                    <li aria-haspopup="true" class="mg_link" :class="{ open: isOpen[0] }">
                        <span class="wsmenu-click 123" @click="toggle(0)"><i class="wsmenu-arrow"></i></span>
                        <NuxtLink to="/" class="h-link hover:bg-blue-700 rounded">Home </NuxtLink>
                        
                    </li>
                    <!-- SIMPLE NAVIGATION LINK -->
                    <li class="nl-simple" aria-haspopup="true"><NuxtLink to="/about" class="h-link hover:bg-blue-700 rounded">Activities</NuxtLink></li>
                    <!-- MEGAMENU -->
                    <li class="nl-simple" aria-haspopup="true"><NuxtLink to="/about" class="h-link hover:bg-blue-700 rounded">Gallery</NuxtLink></li>
                    <li class="nl-simple" aria-haspopup="true"><NuxtLink to="/about" class="h-link hover:bg-blue-700 rounded">Patient Materials</NuxtLink></li>
                    <li class="nl-simple" aria-haspopup="true"><NuxtLink to="/about" class="h-link hover:bg-blue-700 rounded">About Us</NuxtLink></li>
                    <li class="nl-simple" aria-haspopup="true"><NuxtLink to="/about" class="h-link hover:bg-blue-700 rounded">Contact Us</NuxtLink></li>
                   
                   
                </ul>
            </nav>
            <!-- END MAIN MENU -->
        </div>
    </div>
</template>
<script>
import { reactive } from 'vue';
export default {
    setup() {
        const state = reactive({
        isOpen: [false, false]
        });
        const toggle = (index) => {
        state.isOpen[index] = !state.isOpen[index];
        };
        return {
        toggle,
        isOpen: state.isOpen
        };
    },
    mounted() {
        window.addEventListener("scroll", this.handleScroll);
    },
    destroyed() {
        window.removeEventListener("scroll", this.handleScroll);
    },
    methods: {
        handleScroll() {
            const menu = document.getElementById("main-menu");
            const header = document.getElementById("header");
            if (window.pageYOffset > 100) {
                menu.classList.add("scroll");
                header.classList.add("scroll");
            } else {
                menu.classList.remove("scroll");
                header.classList.remove("scroll");
            }
        }
    }
};
</script>
