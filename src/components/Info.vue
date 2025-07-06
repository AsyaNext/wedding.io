<script setup lang="ts">

</script>

<template>
  <div class="info">
    <div class="info__content">
      <div class="info__image">
        <img src="../assets/info.jpg" />
      </div>
      <div class="info__text">
        <div class="info__text-title">Дорогие гости!</div>
        <div class="info__text-desc">Мы верим, что этот день станет прекрасным началом нашей счастливой семейной жизни. Приглашаем вас на свадьбу, ведь мы будем рады разделить этот чудесный праздник с вами!</div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.info {
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
  &__content {
    max-width: 1300px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 100px 50px;
    @media (max-width: 1280px) {
      flex-direction: column-reverse;
    }
  }
  &__image {
    position: relative;
    max-width: 500px;
    width: 100%;
    &:before {
      content: "";
      position: absolute;
      top: -30px;
      left: -30px;
      max-width: 500px;
      width: 100%;
      max-height: 500px;
      height: 100%;
      background-color: rgba(231, 166, 226, 0.5);
      z-index: -1;
      @media (max-width: 600px) {
        display: none;
      }
    }
    img {
      width: 100%;
    }
  }
  &__text {
    max-width: 600px;
    @media (max-width: 1280px) {
      margin-bottom: 70px;
    }
    &-title {
      font-family: 'PT Serif', serif;
      font-size: 38px;
      font-weight: 400;
      line-height: 100%;
      margin-bottom: 36px;
      text-align: right;
      text-transform: uppercase;
      @media (max-width: 1280px) {
        text-align: center;
      }
      @media (max-width: 500px) {
        font-size: 24px;
      }
    }
    &-desc {
      font-family: "Roboto", sans-serif;
      font-size: 20px;
      line-height: 40px;
      font-weight: 300;
      text-align: right;
      @media (max-width: 1280px) {
        text-align: center;
      }
      @media (max-width: 500px) {
        font-size: 16px;
      }
    }
  }
}
</style>