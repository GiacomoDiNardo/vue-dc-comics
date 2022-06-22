<template>
  <div class="bg-banner-sign-up">
    <div class="container py-4">
      <div class="d-flex justify-content-between">
        <button class="btn btn-outline-primary">SIGN-UP NOW</button>

        <div class="socials d-flex gap-3 align-items-center">
          <span class="follow-text">FOLLOW US</span>
          <img
            v-for="(icon, i) in socialIcons"
            :key="i"
            :src="icon.src"
            :alt="`immagine di ${icon}`"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BannerSignUp",

  data() {
    return {
      socialIcons: [
        {
          src: "img/footer-facebook.png",
        },
        {
          src: "img/footer-twitter.png",
        },
        {
          src: "img/footer-youtube.png",
        },
        {
          src: "img/footer-pinterest.png",
        },
        {
          src: "img/footer-periscope.png",
        },
      ],
    };
  },
};
</script>

<style scoped>
.bg-banner-sign-up {
    background-color: #303030;
}

.btn.btn-outline-primary {
    color: white;
}

.follow-text {
    color: var(--bs-primary);
}
</style>