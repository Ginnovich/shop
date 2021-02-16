<template>
  <footer class="footer">
    <div class="footer-container">
      <img class="logo" src="../../img/logo.svg" alt="logo" />
      <nav class="menu">
        <a href="#" class="menu__link">Каталог</a>
        <a href="#" class="menu__link">Доставка</a>
        <a href="#" class="menu__link">Оплата</a>
        <a href="#" class="menu__link">Контакты</a>
        <a href="#" class="menu__link">О галерее</a>
      </nav>
      <div class="search">
        <div class="tel">+7 (495) 555-55-55</div>
        <div class="adress">г. Москва, ул. Расплетина, 24</div>
      </div>
    </div>
  </footer>
</template>



<script>
export default {
  name: "footer",
  data() {
    return {};
  },
};
</script>


<style lang="scss">
.footer {
  width: 100%;
  height: 112px;
  background-color: #eceaea;
  padding-bottom: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 3px auto;
  min-width: 1200px;
  .footer-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-bottom: 20px;
    width: 90%;
    margin: 3px auto;
    min-width: 1200px;
    background-color: #eceaea;
    .logo {
      cursor: pointer;
      margin-right: 48px;
    }

    .menu {
      background-color: #eceaea;
      margin-right: auto;
      &__link {
        background-color: #eceaea;
        color: #343030;
        padding-right: 44px;
        font-family: "Merriweather", serif;
        line-height: 150%;
        font-size: 14px;
      }
    }
    .tel,
    .adress {
      background-image: url(../../img/Vector.svg);
      background-color: #eceaea;
      background-repeat: no-repeat;
      background-position: left;
      color: #555555;
      font-family: "Merriweather", serif;
      line-height: 150%;
      font-size: 14px;
      font-weight: 400;
      padding-left: 22px;
      padding-right: 52px;
    }
    .adress {
      background-image: url(../../img/Location.svg);
      padding-right: 0;
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