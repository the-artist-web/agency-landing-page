<template>
    <section class="bg-list-img">
        <img src="../assets/images/mobile/image-gallery-milkbottles.jpg" alt="image-gallery-milkbottles" loading="lazy" class="img-mobile img-cover">
        <img src="../assets/images/desktop/image-gallery-milkbottles.jpg" alt="image-gallery-milkbottles" loading="lazy" class="img-desktop img-cover">

        <img src="../assets/images/mobile/image-gallery-orange.jpg" alt="image-gallery-orange" loading="lazy" class="img-mobile img-cover">
        <img src="../assets/images/desktop/image-gallery-orange.jpg" alt="image-gallery-orange" loading="lazy" class="img-desktop img-cover">

        <img src="../assets/images/mobile/image-gallery-cone.jpg" alt="image-gallery-cone" loading="lazy" class="img-mobile img-cover">
        <img src="../assets/images/desktop/image-gallery-cone.jpg" alt="image-gallery-cone" loading="lazy" class="img-desktop img-cover">

        <img src="../assets/images/mobile/image-gallery-sugar-cubes.jpg" alt="image-gallery-sugar-cubes" loading="lazy" class="img-mobile img-cover">
        <img src="../assets/images/desktop/image-gallery-sugarcubes.jpg" alt="image-gallery-sugar-cubes" loading="lazy" class="img-desktop img-cover">
    </section>
</template>

<script>
export default {
    name: "BgListImg",
    data() {
        return {};
    }
}
</script>

<style scoped>
    .bg-list-img {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
    }
    .bg-list-img .img-desktop { display: none; }

    /*--------------------------------------*\
      #MEDIA
    \*--------------------------------------*/

    /**
     * fit size 992px
     */
    @media screen and (min-width: 992px) {
        .bg-list-img { grid-template-columns: repeat(4, 1fr); }

        .bg-list-img .img-desktop { display: block; }

        .bg-list-img .img-mobile { display: none; }
    }
</style>