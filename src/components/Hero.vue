<template>
  <div class="hero">
    <div class="container">
        <h1 class="title-hero">We are creatives</h1>
        <img src="../assets/images/icon-arrow-down.svg" alt="icon-arrow-down" loading="lazy" class="icon-arrow-down">
    </div>
  </div>
</template>

<script>
export default {
    name: "Hero",
    data() {
        return {};
    }
}
</script>

<style scoped>
    .hero {
        background-image: url(../assets/images/mobile/image-header.jpg);
        width: 100%;
        height: 100vh;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center center;
    }
    .hero .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        height: 100vh;
        width: 100%;
        gap: 50px;
    } 
    .hero .container .title-hero {
        font-size: 3rem;
        text-align: center;
        color: var(--White);
        text-transform: uppercase;
        font-family: var(--font-family-fraunces);
        letter-spacing: 5px;
    }
    .hero .container .icon-arrow-down {
        width: 50px;
    }

    /*--------------------------------------*\
      #MEDIA
    \*--------------------------------------*/

    /**
     * fit size 992px
     */
    @media screen and (min-width: 992px) {
        .hero { background-image: url(../assets/images/desktop/image-header.jpg); }

        .hero .container { gap: 80px; } 

        .hero .container .title-hero {
            font-size: 4rem;
            font-weight: bold;
            letter-spacing: 10px;
        }
        /* .hero .container .icon-arrow-down { width: 80px; } */
    }
</style>