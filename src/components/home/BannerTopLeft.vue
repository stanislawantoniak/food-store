<template>
  <div class="col-sm-6 nopadding banner-left">
    <div class="aspect-ratio aspect-ratio--4to3">
      <BannerPicture :file="'top-left.jpg'"/>
    </div>

    <div class="banner-text">
      <h4 class="banner-title">{{ $t('title') }}</h4>
      <p class="banner-paragraph">{{ $t('subtitle') }}</p>
      <router-link :to="{ name: 'products', params: { categorySlug: 'chocolate-bars' } }"
                   class="btn banner-btn">
        {{ $t('linkLabel') }}
      </router-link>
    </div>
  </div>
</template>

<script>
import BannerPicture from './BannerPicture.vue';

export default {
  components: { BannerPicture },
};
</script>

<i18n>
en:
  title: "Chocolate sweets"
  subtitle: "Not only snickers are here"
  linkLabel: "Get your bar"
de:
  title: "Sommer Fashion"
  subtitle: "Beste Outfits für die Saison"
  linkLabel: "Jetzt bestellen"
</i18n>
