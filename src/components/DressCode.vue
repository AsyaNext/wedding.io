<script setup lang="ts">

</script>

<template>
  <div class="dresscode">
    <div class="dresscode__content">
      <div class="dresscode__item">
        <div class="dresscode__title">Дресскод</div>
        <div class="dresscode__text">Мы будем очень рады, если вы поддержите цветовую палитру нашей свадьбы!</div>
        <div class="dresscode__common-colors">
          <div class="dresscode__common-item dresscode__common-item--white"></div>
          <div class="dresscode__common-item dresscode__common-item--beige"></div>
          <div class="dresscode__common-item dresscode__common-item--light-purple"></div>
          <div class="dresscode__common-item dresscode__common-item--purple"></div>
          <div class="dresscode__common-item dresscode__common-item--light-blue"></div>
          <div class="dresscode__common-item dresscode__common-item--blue"></div>
          <div class="dresscode__common-item dresscode__common-item--brown"></div>
          <div class="dresscode__common-item dresscode__common-item--black"></div>
        </div>
      </div>
      <div class="dresscode__item">
        <div class="dresscode__title">Детали</div>
        <div class="dresscode__text">
          <div class="dresscode__text-number">1</div>
          <div>Этот особенный день — только для самых близких, поэтому приглашение предназначено лично вам. Надеемся на понимание! &#129309;</div>
          <div class="dresscode__text-number">2</div>
          <div>Мы будем рады вашим тёплым словам и улыбкам! Чтобы праздник остался нежным и романтичным, пожалуйста, воздержитесь от криков “Горько!” — мы и так знаем, как сладко нам вместе &#128523;</div>
          <div class="dresscode__text-number">3</div>
          <div>Ваше присутствие — уже самый ценный подарок для нас! Мы так долго мечтали об этом дне, что у нас уже есть всё необходимое для счастья. Однако если вы хотите поддержать наше будущее, денежный подарок станет для нас самым практичным и желанным &#128176;</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.dresscode {
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgba(49, 127, 216, 0.3);
  &__content {
    max-width: 1300px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 40px 50px;
    gap: 48px;
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
    margin-bottom: 18px;
    @media (max-width: 500px) {
      font-size: 16px;
    }
    &-number {
      font-weight: 600;
      margin: 16px auto;
      width: 40px;
      height: 40px;
      border: 1px solid #000;
      border-radius: 50%;
    }
  }
  &__common {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 16px;
    &-title {
      font-size: 28px;
    }
    &-colors {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-wrap: wrap;
      gap: 8px;
    }
    &-item {
      border-radius: 50%;
      width: 50px;
      height: 50px;
      box-sizing: content-box;
      box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.1);
      &--black {
        background-color: #2F3234;
      }
      &--brown {
        background-color: #45322e;
      }
      &--blue {
        background-color: #0D2DA2;
      }
      &--light-blue {
        background-color: #327fda;
      }
      &--purple {
        background-color: #bb89ec;
      }
      &--light-purple {
        background-color: rgba(231, 166, 226, 1);
      }
      &--beige {
        background-color: #e9d1af;
      }
      &--white {
        background-color: #E4E5EA;
      }
    }
  }
}
</style>