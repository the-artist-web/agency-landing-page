<template>
  <header class="header" data-header>
    <div class="container">
        <a href="#" class="logo">
            <img src="../assets/images/logo.svg" alt="logo">
        </a>

        <nav class="navbar" data-navbar>
            <div class="arrow-top">
                <span></span>
            </div>

            <ul class="navbar-list">
                <li class="navbar-item">
                    <a href="#" class="navbar-link">About</a>
                </li>
                <li class="navbar-item">
                    <a href="#" class="navbar-link">Services</a>
                </li>
                <li class="navbar-item">
                    <a href="#" class="navbar-link">Projects</a>
                </li>
            </ul>

            <button class="btn-primary">Contact</button>
        </nav>

        <img @click="showMenu()" src="../assets/images/icon-hamburger.svg" alt="icon-hamburger" loading="lazy" class="icon-hamburger">
    </div>
  </header>
</template>

<script>
export default {
    name: "Header",
    data() {
        return {};
    },
    methods: {
        showMenu: function () { document.querySelector("[data-navbar]").classList.toggle("active"); }
    }
}
</script>

<style scoped>
    .header .container {
        height: 70px;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        z-index: 10;
    }
    .header .container.active { background-color: var(--Grayish-blue); }
    
    .header .container .navbar {
        position: fixed;
        top: 70px;
        left: 16px;
        right: 16px;
        background-color: var(--White);
        padding: 30px;
        text-align: center;
        display: grid;
        gap: 30px;
        opacity: 0;
        visibility: hidden;
        z-index: 10;
        transition: .4s;
    }
    .header .container .navbar.active {
        top: 110px;
        opacity: 1;
        visibility: visible;
        transition: .4s;
    }
    .header .container .navbar .arrow-top {
        overflow: hidden;
        position: absolute;
        top: -50px;
        right: 0;
        height: 50px;
        width: 50px;
    }
    .header .container .navbar .arrow-top span {
        position: absolute;
        right: -52px;
        top: 25px;
        height: 100px;
        width: 100px;
        transform: rotate(45deg);
        background-color: var(--White);
    }
    .header .container .navbar .navbar-list {
        display: flex;
        flex-direction: column;
        gap: 30px;
    }
    .header .container .navbar .navbar-list .navbar-item .navbar-link {
        color: var(--Dark-grayish-blue);
        font-size: 1.1rem;
        font-weight: 600;
    }

    /*--------------------------------------*\
      #MEDIA
    \*--------------------------------------*/

    /**
     * fit size 992px
     */
    @media screen and (min-width: 992px) {
        .header .container { height: 100px; }

        .header .container .navbar {
            background-color: transparent;
            position: static;
            padding: 0;
            display: flex;
            align-items: center;
            gap: 40px;
            opacity: 1;
            visibility: visible;
        }
        .header .container .navbar .arrow-top { display: none; }

        .header .container .navbar .navbar-list {
            display: flex;
            flex-direction: row;
            align-items: center;
            gap: 40px;
        }
        .header .container .navbar .navbar-list .navbar-item .navbar-link {
            color: var(--White);
            font-size: 1rem;
            font-weight: 500;
        }
        .icon-hamburger { display: none; }
    }
</style>