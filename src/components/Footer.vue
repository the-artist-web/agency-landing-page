<template>
    <footer class="footer section">
        <div class="container">
            <div class="footer-top">
                <img src="../assets/images/logo.svg" alt="logo" class="title-logo">

                <div class="footer-list">
                    <a href="#" class="footer-link">About</a>
                    <a href="#" class="footer-link">Services</a>
                    <a href="#" class="footer-link">Projects</a>
                </div>
            </div>

            <div class="social-list">
                <i class="fa-brands fa-square-facebook social-link"></i>
                <i class="fa-brands fa-instagram social-link"></i>
                <i class="fa-brands fa-twitter social-link"></i>
                <i class="fa-brands fa-pinterest social-link"></i>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer",
    data() {
        return {};
    }
}
</script>

<style scoped>
    .footer { 
        background-color: var(--Dark-moderate-cyan); 
        color: var(--Dark-desaturated-cyan);
    }

    .footer .container .footer-top {
        text-align: center;
        display: grid;
        gap: 40px;
        margin-bottom: 60px;
    }
    .footer .container .footer-top .title-logo {
        margin: 0 auto;
        width: 180px;
    }
    .footer .container .footer-top .footer-list {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 30px;
    }
    .footer .container .footer-top .footer-list .footer-link {
        color: var(--Dark-desaturated-cyan);
        font-size: 1.1rem;
        font-weight: 600;
        transition: .4s;
    }
    .footer .container .footer-top .footer-list .footer-link:hover {
        color: var(--White);
        transition: .4s;
    }
    .footer .container .social-list {
        display: flex;
        align-content: center;
        justify-content: center;
        gap: 20px;
    }
    .footer .container .social-list .social-link {
        color: var(--Dark-desaturated-cyan);
        font-size: 1.3rem;
        font-weight: 600;
        cursor: pointer;
        transition: .4s;
    }
    .footer .container .social-list .social-link:hover {
        color: var(--White);
        transition: .4s;
    }

    /*--------------------------------------*\
      #MEDIA
    \*--------------------------------------*/

    /**
     * fit size 992px
     */
    @media screen and (min-width: 992px) {
        .footer .container .footer-top {
            gap: 50px;
            margin-bottom: 70px;
        }
        .footer .container .footer-top .footer-list { gap: 50px; }

        .footer .container .social-list { gap: 30px; }
    }
</style>