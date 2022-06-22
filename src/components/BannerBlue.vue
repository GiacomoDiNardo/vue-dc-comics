<template>
  <div class="bg-banner-blue">
    <div class="container py-5">
      <div class="row">
        <div class="col d-flex justify-content-center align-items-center gap-3" v-for="page in pages" :key="page.title">
          <img :src="page.logo" :alt="`immagine di ${page.title}`" />
          <span class="shop-name">{{ page.title }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BannerBlue",

  data() {
    return {
      pages: [
        {
          logo: "/img/buy-comics-digital-comics.png",
          title: "digital comics",
        },
        {
          logo: "/img/buy-comics-merchandise.png",
          title: "DC merchandise",
        },
        {
          logo: "/img/buy-comics-subscriptions.png",
          title: "subscription",
        },
        {
          logo: "/img/buy-comics-shop-locator.png",
          title: "comic shop locator",
        },
        {
          logo: "/img/buy-dc-power-visa.svg",
          title: "Dc power visa",
        },
      ],
    };
  },
};
</script>

<style scoped>
.bg-banner-blue {
  background-color: #2c7df5;
  color: white;
}

.col img {
    width: 50px;
    aspect-ratio: 1/1;
    object-fit: contain;
}

.col span {
    text-transform: uppercase;
    font-size: 14px;
}
</style>