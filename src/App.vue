<template>
    <div>
        <navbar-vue />
        <ScrollToTopVue />

        <!-- render vue router -->
        <router-view :key="$route.fullPath"></router-view>
        <!-- <router-view v-slot="{ Component, route }">
            <transition name="fade">
                <component :is="Component" :key="route.path" />
            </transition>
        </router-view> -->
    </div>
</template>

<!-- Test  -->
<script>
import NavbarVue from './components/Navbar.vue'
import ScrollToTopVue from './components/ScrollToTop.vue';

export default {
    name: 'App',
    components: {
        NavbarVue,
        ScrollToTopVue,
    },

}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;1,200;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');

* {
    font-family: 'Plus Jakarta Sans', sans-serif;
}

body {
    background-color: lightgray !important;
}

::-webkit-scrollbar {
    width: 15px;
}

::-webkit-scrollbar-track {
    border-radius: 2px;
    box-shadow: inset 0 0 10px rgb(149, 149, 149);
}

::-webkit-scrollbar-thumb {
    border-radius: 5px;
    background-color: #198754;
}

::-webkit-scrollbar-thumb:hover {
    background-color: #005f33;
}
</style>