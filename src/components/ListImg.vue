<template>
  <section class="list-img">
    <div class="list-img-top">
        <div class="list-img-box">
            <div class="list-img-box-content">
                <h1 class="title-content">Transform your brand</h1>
                <p class="text-content">
                We are a full-service creative agency specializing in helping brands grow fast. 
                Engage your clients through compelling visuals that do most of the marketing for you.</p>
                <button class="btn-img-box Yellow">Learn more</button>
            </div>

            <img src="../assets/images/mobile/image-transform.jpg" alt="image-transform.jpg" loading="lazy" class="img-mobile img-cover">
            <img src="../assets/images/desktop/image-transform.jpg" alt="image-transform.jpg" loading="lazy" class="img-desktop img-cover">
        </div>

        <div class="list-img-box box-2">
            <img src="../assets/images/mobile/image-stand-out.jpg" alt="image-transform.jpg" loading="lazy" class="img-mobile img-cover">
            <img src="../assets/images/desktop/image-stand-out.jpg" alt="image-transform.jpg" loading="lazy" class="img-desktop img-cover">

            <div class="list-img-box-content">
                <h1 class="title-content">Stand out to the right audience</h1>
                <p class="text-content">Using a collaborative formula of designers, researchers, photographers, 
                videographers, and copywriters, we’ll build and extend your brand in digital places.</p>
                <button class="btn-img-box Red">Learn more</button>
            </div>
        </div>
    </div>

    <div class="list-img-bottom">
        <div class="list-img-box-bottom">
            <img src="../assets/images/mobile/image-graphic-design.jpg" alt="image-graphic-design" loading="lazy" class="img-mobile img-cover">
            <img src="../assets/images/desktop/image-graphic-design.jpg" alt="image-graphic-design" loading="lazy" class="img-desktop img-cover">

            <div class="list-img-box-bottom-content">
                <h1 class="title color-1">Graphic design</h1>
                <p class="text color-1">Great design makes you memorable. We deliver artwork that underscores your brand message and captures potential clients’ attention.</p>
            </div>
        </div>
        
        <div class="list-img-box-bottom">
            <img src="../assets/images/mobile/image-photography.jpg" alt="image-photography" loading="lazy" class="img-mobile img-cover">
            <img src="../assets/images/desktop/image-photography.jpg" alt="image-photography" loading="lazy" class="img-desktop img-cover">

            <div class="list-img-box-bottom-content">
                <h1 class="title color-2">Photography</h1>
                <p class="text color-2">Increase your credibility by getting the most stunning, high-quality photos that improve your business image.</p>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: "ListImg",
    data() {
        return {};
    }
}
</script>

<style scoped>
    .list-img .list-img-top {
        display: flex;
        flex-direction: column;
    }
    .list-img .list-img-top .list-img-box {
        display: flex;
        flex-direction: column-reverse;
    }
    .list-img .list-img-top .box-2 { 
        display: flex;
        flex-direction: column; 
    }
    .list-img .list-img-top .list-img-box .img-desktop { display: none; }

    .list-img .list-img-top .list-img-box .list-img-box-content {
        padding: 80px 16px;
        text-align: center;
    }
    .list-img .list-img-top .list-img-box .list-img-box-content .title-content {
        font-family: var(--font-family-fraunces);
        font-size: 2.2rem;
        font-weight: bolder;
        margin-bottom: 30px;
    }
    .list-img .list-img-top .list-img-box .list-img-box-content .text-content {
        color: var(--Dark-grayish-blue);
        font-size: 1.1rem;
        font-weight: 600;
        line-height: 1.8;
        margin-bottom: 35px;
    }    
    .list-img .list-img-top .list-img-box .list-img-box-content .btn-img-box {
        font-family: var(--font-family-fraunces);
        font-size: 1.1rem;
        font-weight: 700;
        text-transform: uppercase;
        margin: 0 auto;
        width: max-content;
        position: relative;
    }
    .list-img .list-img-top .list-img-box .list-img-box-content .btn-img-box::before {
        content: "";
        border-radius: 100px;
        position: absolute;
        height: 12px;
        width: 100%;
        bottom: -6px;
        left: 0;
        right: 0;
        opacity: 0.5;
        transition: .4s;
    }
    .list-img .list-img-top .list-img-box .list-img-box-content .Yellow::before { background-color: var(--Yellow); }

    .list-img .list-img-top .list-img-box .list-img-box-content .Red::before { background-color: var(--Soft-red); }

    .list-img .list-img-top .list-img-box .list-img-box-content .btn-img-box:hover::before {
        content: "";
        opacity: 1; 
        transition: .4s;
    }
    .list-img .list-img-bottom {
        display: flex;
        flex-direction: column;
    }
    .list-img .list-img-bottom .list-img-box-bottom { position: relative; }

    .list-img .list-img-bottom .list-img-box-bottom img { position: relative; }

    .list-img .list-img-bottom .list-img-box-bottom .img-desktop { display: none; }

    .list-img .list-img-bottom .list-img-box-bottom .list-img-box-bottom-content {
        text-align: center;
        display: grid;
        position: absolute;
        bottom: 20px;
        right: 16px;
        left: 16px;
        z-index: 9;
    }
    .list-img .list-img-bottom .list-img-box-bottom .list-img-box-bottom-content .title {
        font-family: var(--font-family-fraunces);
        font-size: 2.2rem;
        font-weight: bolder;
        margin-bottom: 30px;
    }
    .list-img .list-img-bottom .list-img-box-bottom .list-img-box-bottom-content .text {
        color: var(--Dark-grayish-blue);
        font-size: 1.1rem;
        font-weight: 600;
        line-height: 1.5;
        margin-bottom: 35px;
    }  
    .list-img .list-img-bottom .list-img-box-bottom .list-img-box-bottom-content .color-1 { color: var(--Dark-desaturated-cyan); }

    .list-img .list-img-bottom .list-img-box-bottom .list-img-box-bottom-content .color-2 { color: var(--Dark-blue); }

    /*--------------------------------------*\
      #MEDIA
    \*--------------------------------------*/

    /**
     * fit size 992px
     */
    @media screen and (min-width: 992px) {
        .list-img .list-img-top .list-img-box {
            display: grid;
            align-items: center;
            grid-template-columns: repeat(2, 1fr);
        }
        .list-img .list-img-top .list-img-box .img-desktop { display: block; }

        .list-img .list-img-top .list-img-box .img-mobile { display: none; }

        .list-img .list-img-top .list-img-box .list-img-box-content {
            padding: 100px;
            text-align: left;
        }
        .list-img .list-img-top .list-img-box .list-img-box-content .btn-img-box { margin: 0 0; }

        .list-img .list-img-top .list-img-box .list-img-box-content .title-content {
            font-size: 2.5rem;
            max-width: 500px;
            margin-bottom: 50px;
        }
        .list-img .list-img-top .list-img-box .list-img-box-content .text-content { margin-bottom: 55px; }    

        .list-img .list-img-bottom {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
        }
        .list-img .list-img-bottom .list-img-box-bottom .img-desktop { display: flex; }
        
        .list-img .list-img-bottom .list-img-box-bottom .img-mobile { display: none; }

        .list-img .list-img-bottom .list-img-box-bottom .list-img-box-bottom-content {
            max-width: 450px; 
            margin: 0 auto;
        }
    }
</style>