<template>
  <section class="custom section">
    <div class="container">
        <h1 class="title">Client testimonials</h1>

        <ul class="custom-list">
            <li class="custom-box">
                <img src="../assets/images/image-emily.jpg" alt="image-emily" class="custom-img">

                <p class="text-custom">
                    We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.
                </p>

                <div class="custom-content">
                    <h1 class="title-content">Emily R.</h1>
                    <p class="text-content">Marketing Director</p>
                </div>
            </li>

            <li class="custom-box">
                <img src="../assets/images/image-thomas.jpg" alt="image-thomas" class="custom-img">

                <p class="text-custom">
                    Sunnyside’s enthusiasm coupled with their keen interest in our brand’s success made it a satisfying and enjoyable experience.
                </p>

                <div class="custom-content">
                    <h1 class="title-content">Thomas S.</h1>
                    <p class="text-content">Chief Operating Officer</p>
                </div>
            </li>

            <li class="custom-box">
                <img src="../assets/images/image-jennie.jpg" alt="image-jennie" class="custom-img">

                <p class="text-custom">
                    Incredible end result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!
                </p>

                <div class="custom-content">
                    <h1 class="title-content">Jennie F.</h1>
                    <p class="text-content">Business Owner</p>
                </div>
            </li>
        </ul>
    </div>
  </section>
</template>

<script>
export default {
    name: "CustomList",
    data() {
        return {};
    }
}
</script>

<style scoped>
    .custom .container .title {
        font-family: var(--font-family-fraunces);
        text-align: center;
        margin: 0 0 60px;
        font-size: 1.2rem;
        letter-spacing: 3px;
        font-weight: 700;
        text-transform: uppercase;
        color: var(--Grayish-blue);
    }
    .custom .container .custom-list {
        display: grid;
        grid-template-columns: repeat(1, 1fr);
        gap: 80px;
    }
    .custom .container .custom-list .custom-box {
        text-align: center;
        display: grid;
        gap: 30px;
    }
    .custom .container .custom-list .custom-box .custom-img {
        width: 80px;
        height: 80px;
        margin: 0 auto;
        border-radius: 100px;
    }
    .custom .container .custom-list .custom-box .text-custom {
        color: var(--Very-dark-grayish-blue);
        font-size: 1.1rem;
        font-weight: 600;
        line-height: 1.8;
    }
    .custom .container .custom-list .custom-box .custom-content {
        display: grid;
        gap: 10px;
    }
    .custom .container .custom-list .custom-box .custom-content .title-content {
        font-family: var(--font-family-fraunces);
        font-size: 1.4rem;
        font-weight: bolder;
    }
    .custom .container .custom-list .custom-box .custom-content .text-content {
        color: var(--Grayish-blue);
        font-size: 1rem;
        font-weight: 500;
    }

    /*--------------------------------------*\
      #MEDIA
    \*--------------------------------------*/

    /**
     * fit size 992px
     */
    @media screen and (min-width: 992px) {
        .custom .container .title {
            margin: 0 0 80px;
            font-size: 1.5rem; 
        }
        .custom .container .custom-list {
            grid-template-columns: repeat(3, 1fr);
            max-width: 1300px;
            margin: 0 auto;
            gap: 30px;
        }
        .custom .container .custom-list .custom-box { gap: 60px; }
    }
</style>