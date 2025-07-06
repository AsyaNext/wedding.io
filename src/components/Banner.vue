<script setup lang="ts">

</script>

<template>
  <div class="banner">
    <div class="banner__content">
      <div class="banner__title">
        <span>Анастасия</span>
        <span>&</span>
        <span>Павел</span>
      </div>
      <div class="banner__separator"></div>
      <div class="banner__date">28.08.2025</div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.banner {
  width: 100vw;
  height: 100vh;
  background: -webkit-linear-gradient(130deg, #317fd8,#e7a6e2,#f0efea);/* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(130deg, #317fd8,#e7a6e2,#f0efea);/* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  background-attachment: fixed;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
  @media (max-width: 650px) {
    height: 50vh;
  }
  &__content {
    width: 70%;
    height: 60%;
    background-color: rgba(255, 255, 255, 0.1);
    box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.1);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  &__title {
    font-family: "Mon Amour One", cursive;
    font-size: 80px;
    color: #fff;
    text-align: center;
    display: flex;
    gap: 16px;
    @media (max-width: 1280px) {
      font-size: 60px;
    }
    @media (max-width: 650px) {
      line-height: 40px;
      font-size: 30px;
      flex-direction: column;
      align-items: center;
      gap: 4px;
    }
  }
  &__separator {
    width: 50%;
    height: 1px;
    background-color: #fff;
    margin: 24px 0;
    @media (max-width: 1280px) {
      margin: 12px 0;
    }
  }
  &__date {
    font-family: "Mon Amour One", cursive;
    font-size: 40px;
    color: #fff;
    @media (max-width: 1280px) {
      font-size: 30px;
    }
    @media (max-width: 650px) {
      line-height: 20px;
      font-size: 20px;
    }
  }
}
</style>