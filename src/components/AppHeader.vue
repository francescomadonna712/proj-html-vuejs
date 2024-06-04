<script>
import AppNavBar from "../components/AppNavBar.vue";


export default {
    components: {
        AppNavBar,
    },

    data() {
        return {

        }
    },
}

</script>

<template>
    <div class="cnt">
        <div class="navbar">
            <div class="nav-row">

                <div class="news-updates">
                    <div class="up">NEWS UPDATES</div>

                    <div class="time">
                        <div>05:33</div>
                        <span>THE</span>
                    </div>

                    <button class="left"><i class="fa-solid fa-chevron-left"></i></button>
                    <button class="right"><i class="fa-solid fa-chevron-right"></i></button>

                </div>

                <div class="social-icons">
                    <i class="fab fa-facebook"></i>
                    <i class="fab fa-twitter"></i>
                    <i class="fab fa-instagram"></i>
                    <i class="fab fa-youtube"></i>
                </div>
            </div>
        </div>

        <div class="banner">
            <div class="row-bnr">
                <img src="../assets/anime-logo.webp" alt="AnimeTech Logo" class="logo" />
                <img src="../assets/header-banner.webp" alt="Banner 1" class="banner-img" />
            </div>
        </div>

        <AppNavBar />

    </div>
</template>

<style scoped>
.navbar {
    justify-content: center;
    display: flex;
    background-color: #BF1D2E;
}

.nav-row {
    display: flex;
    width: 1440px;
    justify-content: space-between;
}

.up {
    padding: 0.5rem;
    margin-right: 1rem;
    background-color: #545454;
}

.news-updates {
    justify-content: center;

    color: white;
    display: flex;
    font-weight: bold;
}

.time {
    display: flex;
    align-items: center;
}

.time span {
    margin-right: 25rem;
}

button {
    color: white;
    padding-right: 1rem;
    border: 0px;
    background-color: #BF1D2E;
}



.social-icons,
i {
    color: white;
    display: flex;
    align-items: center;
    margin: 0 5px;
    font-size: 20px;

}

.social-icons i:hover {
    color: #999;
}

.banner {
    justify-content: center;
    width: 100%;
    border-bottom: 1px solid rgb(228, 222, 222);
    display: flex;
    background-color: white;
    padding: 10px 0px;

}

.row-bnr {
    display: flex;
    justify-content: space-between;
    width: 1440px;
    padding: 10px 0px;
}


.banner .logo {
    max-height: 90px;
}

.banner .banner-img {
    max-height: 90px;
    margin-left: 20px;
}
</style>
