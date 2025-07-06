<script setup lang="ts">

</script>

<template>
  <div class="contacts">
    <div class="contacts__content">
      <div class="contacts__title">Контакты</div>
      <div class="contacts__text">Если у вас есть вопросы по организации праздника, с радостью подскажет наш ведущий Андрей</div>
      <div class="contacts__item">
        <img src="../assets/icon-telegram.png" alt="telegram" />
        <span>+7 (918) 642-88-95</span>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.contacts {
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
  &__content {
    height: 100%;
    max-width: 1300px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 40px;
  }
  &__title {
    font-family: 'PT Serif', serif;
    font-size: 38px;
    font-weight: 500;
    line-height: 100%;
    margin-bottom: 36px;
    text-align: center;
    text-transform: uppercase;
    @media (max-width: 500px) {
      font-size: 24px;
    }
  }
  &__text {
    font-family: "Roboto", sans-serif;
    font-size: 20px;
    line-height: 40px;
    font-weight: 300;
    text-align: center;
    margin-bottom: 16px;
    @media (max-width: 500px) {
      font-size: 16px;
    }
  }
  &__item {
    display: flex;
    align-items: center;
    gap: 8px;
    span {
      font-family: "Roboto", sans-serif;
      font-size: 20px;
      font-weight: 300;
      text-align: center;
    }
    img {
      width: 24px;
      height: 24px;
    }
  }
}
</style>