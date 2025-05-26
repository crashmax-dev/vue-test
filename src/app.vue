<template>
  <div class="container">
    <div class="tabs">
      <span>Вход</span>
      <span>Регистрация</span>
    </div>
    <span class="title">Введите данные для входа</span>
    <div>
      <input class="input" placeholder="Пароль">
      <input class="input" placeholder="E-mail">
    </div>
    <input id="checkbox" type="checkbox" name="checkbox">
    <label for="checkbox">Запомнить меня</label>
    <button class="buton">
      Войти
    </button>
  </div>
</template>

<script setup lang="ts">
</script>

<style lang="scss">
body {
  background-color: #985ACE;
  padding: 40px;
}

.container {
  margin: 0 auto;
  border-radius: 30px;
  background-color: #fff;
  padding: 20px 25% 45px 2rem;

  span {
    font-size: 12px;
    font-weight: 700;
    line-height: 16px;
    text-transform: uppercase;
    cursor: pointer;
  }

  .title {
    font-size: 24px;
    margin-bottom: 16px;

    .active {
      background-color: #8459aa79;
      border-radius: 4px;
    }
  }

  input[type='email'],
  input[type='password'] {
    background-color: #F8F1FF;
    min-height: 32px;
    border-radius: 7px;
    margin-bottom: 8px;
    display: block;
    width: 100%;
    border: none;
    padding: 8px 16px;
    margin-bottom: 20px;
  }
}

.buton {
  display: block;
  width: 100%;
  border: 1px solid transparent;
  border-radius: 10px;
  color: white;
  background-color: #985ACE;
  height: 40px;
  text-transform: uppercase;
  font-weight: 700;
  font-size: 12px;
  margin-top: 40px;
  border: none;
  &:disabled {
    background-color: gray;
  }
}
</style>
