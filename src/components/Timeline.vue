<script setup lang="ts">

</script>

<template>
  <div class="timeline">
    <div class="timeline__content">
      <div class="timeline__title">Свадебный timeline</div>
      <div class="timeline__body">
        <div class="timeline__item">
          <span class="timeline__item-time">15:00</span>
          <span class="timeline__item-text">Welcome</span>
        </div>
        <div class="timeline__item">
          <span class="timeline__item-time">16:00</span>
          <span class="timeline__item-text">Торжественная церемония</span>
        </div>
        <div class="timeline__item">
          <span class="timeline__item-time">16:30</span>
          <span class="timeline__item-text">Начало банкета</span>
        </div>
        <div class="timeline__item">
          <span class="timeline__item-time">20:30</span>
          <span class="timeline__item-text">Завершение официальной части</span>
        </div>
        <div class="timeline__item">
          <span class="timeline__item-time">23:00</span>
          <span class="timeline__item-text">Завершение торжества</span>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.timeline {
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
    padding: 60px 50px;
  }
  &__title {
    font-family: 'PT Serif', serif;
    font-size: 38px;
    font-weight: 500;
    line-height: 100%;
    margin-bottom: 48px;
    text-align: center;
    text-transform: uppercase;
    @media (max-width: 500px) {
      font-size: 24px;
    }
  }
  &__body {
    max-width: 600px;
    width: 100%;
    display: flex;
    flex-direction: column;
  }
  &__item {
    display: flex;
    align-items: center;
    gap: 24px;
    padding: 20px 0;
    &:not(:last-child) {
      border-bottom: 1px solid #000;
    }
    &-text {
      font-family: "Roboto", sans-serif;
      font-size: 20px;
      font-weight: 300;
      @media (max-width: 500px) {
        font-size: 16px;
      }
    }
    &-time {
      font-family: 'PT Serif', serif;
      font-size: 38px;
      font-weight: 500;
      line-height: 100%;
      text-align: center;
      text-transform: uppercase;
      @media (max-width: 500px) {
        font-size: 24px;
      }
    }
  }
}
</style>