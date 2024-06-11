<script setup>
import BannerContainer from '../components/BannerContainer.vue'
import FAQContainer from '../components/FAQContent.vue'
import FooterComponent from '../components/FooterComponent.vue'
</script>

<template>
  <main>
    <section>
      <BannerContainer />
    </section>
    <section>
      <FAQContainer/>
    </section>
    <footer>
      <FooterComponent/>
    </footer>
  </main>
</template>
