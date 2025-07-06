<script setup lang="ts">

</script>

<template>
  <div class="place">
    <div class="place__content">
      <div class="place__text">
        <div class="place__text-title">Место проведения</div>
        <div class="place__text-desc">
          <span>Панорамный Шатер "Garden Hall"</span>
          <br>
          <span>посёлок Токсово, Разъезжая улица, 15</span>
        </div>
      </div>
      <div class="place__image">
        <img src="../assets/place.jpg" />
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.place {
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
    padding: 0 50px 100px;
    @media (max-width: 1280px) {
      flex-direction: column;
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
      right: -30px;
      max-width: 500px;
      width: 100%;
      max-height: 375px;
      height: 100%;
      background-color: rgba(49, 127, 216, 0.3);
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
      font-weight: 500;
      line-height: 100%;
      margin-bottom: 36px;
      text-align: left;
      text-transform: uppercase;
      @media (max-width: 1280px) {
        text-align: center;
        padding-top: 100px;
        border-top: 1px solid #898989;
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
      text-align: left;
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