<template>
  <header class="header">
    <img class="logo" src="../../img/logo.svg" alt="logo" />
    <nav class="menu">
      <a href="#" class="menu__link">Каталог</a>
      <a href="#" class="menu__link">Доставка</a>
      <a href="#" class="menu__link">Оплата</a>
      <a href="#" class="menu__link">Контакты</a>
      <a href="#" class="menu__link">О галерее</a>
    </nav>
    <div class="search">
      <form class="search__form" action="index.html" method="POST">
        <input
          type="text"
          class="search__txt"
          name=""
          placeholder="Поиск по названию картины"
        />
        <button v-on:click="method" class="search__btn">Найти</button>
      </form>
    </div>
  </header>
</template>

<script>
export default {
  name: "header",
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-bottom: 20px;
  width: 90%;
  margin: 3px auto;
  min-width: 1200px;
  .logo {
    cursor: pointer;
    margin-right: 48px;
  }
  .menu {
    margin-right: auto;
    &__link {
      color: #343030;
      padding-right: 44px;
      font-family: "Merriweather", serif;
      line-height: 150%;
      font-size: 14px;
    }
  }
  .search {
    display: flex;
    &__txt {
      width: 294px;
      height: 48px;
      padding: 14px;
      border: 1px solid #e1e1e1;
      color: #9f9f9f;
      font-family: "Merriweather", serif;
      line-height: 150%;
      font-size: 14px;
      outline: none;
      &:hover {
        border: 1px solid #b5b5b5;
        color: #343030;
      }
    }
    &__btn {
      height: 48px;
      width: 122px;
      border: none;
      background-color: #403432;
      font-family: "Merriweather", serif;
      line-height: 150%;
      font-size: 14px;
      font-weight: 700;
      float: right;
      color: white;
      cursor: pointer;
    }
  }
}
</style>