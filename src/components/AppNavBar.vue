<script>
import store from '../data/store.js';
import AppCardHeader from "./AppCardHeader.vue";

export default {

    components: {

        AppCardHeader,


    },

    data() {
        return {
            store,

        };
    }
};
</script>

<template>
    <div class="container-fluid">
        <div class="nav">
            <div class="menu-icon">
                <i class="fa-solid fa-bars"></i>
            </div>
            <div class="nav-links">
                <a v-for="link in store.navLinks" :key="link.text" :href="link.href"
                    :class="['nav-link', { active: link.active }]">
                    <i :class="link.icon"></i> {{ link.text }}
                </a>

                <div v-for="dropdown in store.dropdowns" :key="dropdown.text" class="dropdown">
                    <a href="#" class="nav-link">
                        <i :class="dropdown.icon"></i> {{ dropdown.text }}
                        <i class="fa-solid fa-chevron-down"></i>
                    </a>
                    <div class="dropdown-content">
                        <a>
                            <AppCardHeader />
                        </a>
                    </div>
                </div>

                <a v-for="link in store.bottomLinks" :key="link.text" :href="link.href" class="nav-link">
                    <i :class="link.icon"></i> {{ link.text }}
                </a>
            </div>
            <div class="search-icon">
                <i class="fas fa-search"></i>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container-fluid {
    padding: 0;
    display: flex;
    justify-content: center;
    border-bottom: 1px solid #ddd;
}

.nav {
    width: 1440px;
    display: flex;
    justify-content: space-between;
    background-color: white;
    padding: 10px 0px;
}

.menu-icon,
.search-icon {
    font-size: 24px;
    cursor: pointer;
}

.nav-links {
    display: flex;
    align-items: center;
}

.nav-link {

    text-decoration: none;
    color: black;
    font-weight: bold;
    display: flex;
    align-items: center;
}

.nav-link i {
    margin-right: 5px;
}

.i-link a:hover,
.search-icon:hover,
.nav-link:hover,
.menu-icon:hover {
    color: #BF1D2E;
}

.dropdown {
    position: relative;
    display: inline-block;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: white;
    box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
    z-index: 1;
    min-width: 180px;
}

.dropdown:hover .dropdown-content {
    display: block;
}

.dropdown-content a {
    color: black;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
}

.dropdown-content a:hover {
    background-color: #ddd;
}

.i-link {
    color: black;
    font-weight: bold;
    font-size: small;
    align-items: center;
}
</style>