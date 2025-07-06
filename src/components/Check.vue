<script setup lang="ts">

</script>

<template>
  <div class="check">
    <div class="check__content">
      <div class="check__title">Приглашение</div>
      <div class="check__text">
        Мы будем рады разделить с вами прекрасные воспоминания &#128149;
      </div>
      <div class="check__text">
        &#9200; 28.08.2025 15:00 | &#128205; <a href="https://yandex.ru/maps/?ll=30.525322%2C60.135978&mode=poi&poi%5Bpoint%5D=30.525827%2C60.136079&poi%5Buri%5D=ymapsbm1%3A%2F%2Forg%3Foid%3D1787083279&z=18.39" target="_blank">посёлок Токсово, Разъезжая улица, 15</a>
      </div>
      <button>
        <a href="https://forms.gle/rsnutB51C3a5m4th9" target="_blank">Подтвердить присутствие</a>
      </button>
    </div>
  </div>
</template>

<style scoped lang="scss">
.check {
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
    padding: 40px 50px;
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
    a {
      color: #000;
    }
  }
  button {
    border: 1px solid #000;
    outline: none;
    background-color: transparent;
    color: #000;
    font-family: "Roboto", sans-serif;
    font-size: 16px;
    font-weight: 300;
    border-radius: 5px;
    padding: 16px 24px;
    cursor: pointer;
    transition: all 0.3s;
    a {
      color: #000;
      text-decoration: none;
      &:hover {
        color: #000;
      }
    }
    &:hover {
      background-color: rgba(255, 255, 255, 0.3);
    }
  }
}
</style>