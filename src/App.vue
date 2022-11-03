<template>
  <div>
    <div class="bg_container">
      <section class="top">
        <TopSection/>
        <LinkTree/>
      </section>
    </div>
    <AboutInfo/>
  </div>
</template>

<script setup>
  import TopSection from '@/components/TopSection.vue'
  import LinkTree from '@/components/LinkTree.vue'
  import AboutInfo from '@/components/AboutInfo.vue'
</script>

<style>
  .bg_container{  
      background-image: url(../src/imgs/BG_MicBlackAndWhite.jpg);
      background-size: 100%;
      text-align: center;
      padding-bottom: 4em;
  }
  @media (min-width: 667px) {
    section {
        margin: 0 4em;
    }
  }
</style>
