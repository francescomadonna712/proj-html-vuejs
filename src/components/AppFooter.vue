<script>

</script>

<template>
    <div class="container-fluid">
        <div class="footer-row">

            <ul>
                <li>
                    <h5>GET STARTED</h5>
                </li>
                <li><a href="">Resources</a></li>
                <li><a href="">Tutorials</a></li>
                <li><a href="">Examples</a></li>
                <li><a href="">Docs</a></li>
            </ul>
            <ul>
                <li>
                    <h5>ABOUT</h5>
                </li>
                <li><a href="">Stories</a></li>
                <li><a href="">Community</a></li>
                <li><a href="">Blog</a></li>
                <li><a href="">Brand Assets</a></li>
            </ul>
            <ul>
                <li>
                    <h5>FEATURES</h5>
                </li>
                <li><a href="">Overview</a></li>
                <li><a href="">Design</a></li>
                <li><a href="">Code</a></li>
                <li><a href="">Collaborate</a></li>
            </ul>
            <ul>
                <li>
                    <h5>QUICK LINKS</h5>
                </li>
                <li><a href="">Stories</a></li>
                <li><a href="">Community</a></li>
                <li><a href="">Blog</a></li>
                <li><a href="">Brand Assets</a></li>
            </ul>
            <ul>
                <li>
                    <h5>SUBSCRIBE TO NEWSLETTER</h5>
                </li>
                <li><input class="email" type="text" placeholder="Email"></li>
                <li><button>SUBSCRIBE</button></li>

            </ul>
        </div>
    </div>
    <div class="banner">
        <div class="row-bnr">
            <img src="../assets/anime-logo-white-300x89.png" alt="AnimeTech Logo" class="logo" />
            <span>© Anime Tech, Theme by HasnainDEV</span>

        </div>
    </div>

</template>

<style scoped>
.container-fluid {
    padding: 0;
    background-color: #BF1D2E;
    display: flex;
    justify-content: center;


}

.footer-row {
    display: flex;
    flex-direction: row;
    padding-top: 3rem;

    color: white;
    width: 1440px;

}

ul {
    padding: 0;
    border-bottom: 1PX solid white;
    padding-bottom: 3rem;
}

li {
    padding: 0.2rem;
    padding-right: 8rem;
    list-style: none;
}

a {
    color: white;
}

a:link {
    color: white;
    text-decoration: none;
    font-weight: 500;
}

A:HOVER {
    color: grey;
}

.email {
    width: 20rem;
    padding: 0.6rem;
    border-radius: 5px;
    border: none;
}

button {
    width: 20rem;
    padding: 0.6rem;
    border-radius: 5px;
    border: none;
    background-color: #545454;
    color: white;
    font-weight: 600;
}

.banner {

    width: 100%;
    justify-content: center;
    display: flex;
    background-color: #BF1D2E;
    padding: 10px 0px;

}

.row-bnr {
    display: flex;
    justify-content: space-between;
    width: 1440px;
    padding: 10px 0px;
}

.row-bnr span {
    display: flex;
    align-items: center;
    font-size: larger;
    color: white;
    margin-right: 30px;
}
</style>