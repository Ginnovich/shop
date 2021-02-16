<template>
  <section class="shop">
    <hr />
    <h1>Картины эпохи Возрождения</h1>
    <div class="card-container">
      <form action="index.html" method="get" class="card">
        <img src="../../img/painting-63186_1280 1.png" alt="painting" />
        <h3 class="article">«Рождение Венеры» Сандро Боттичелли</h3>
        <div class="shop__buy">
          <div class="shop__price">
            <h4>2 000 000 $</h4>
            <h2>1 000 000 $</h2>
          </div>
          <button class="shop__btn">Купить</button>
        </div>
      </form>
      <form action="index.html" method="get" class="card">
        <img
          src="../../img/ae973f6678e037cd297053384aa7dca0 1.png"
          alt="painting"
        />
        <h3 class="article">«Тайная вечеря» Леонардо да Винчи</h3>
        <div class="shop__buy">
          <div class="shop__price">
            <h2>3 000 000 $</h2>
          </div>
          <button class="shop__btn">Купить</button>
        </div>
      </form>
      <form action="index.html" method="get" class="card">
        <img src="../../img/image-19 1.png" alt="painting" />
        <h3 class="article">«Сотворение Адама» Микеланджело</h3>
        <div class="shop__buy">
          <div class="shop__price">
            <h4>6 000 000 $</h4>
            <h2>5 000 000 $</h2>
          </div>
          <button class="shop__btn">Купить</button>
        </div>
      </form>
      <form action="index.html" method="get" class="card card-disabled">
        <img src="../../img/20152310142330 1.png" alt="painting" />
        <h3 class="article">«Урок анатомии» Рембрандт</h3>
        <div class="shop__buy">
          <div class="shop__price">
            <h2 class="sold">Продана на аукционе</h2>
          </div>
        </div>
      </form>
    </div>
  </section>
</template>


<script>
export default {
  name: "shop",
  data() {
    return {};
  },
};
</script>


<style lang="scss">
.shop {
  min-height: 768px;
  border-top: 1px solid #e1e1e1;
  margin: 0 auto;
  width: 90%;
  min-width: 1200px;
  h1 {
    margin-top: 45px;
    font-family: "Merriweather", serif;
    font-weight: 700;
    font-size: 24px;
    line-height: 150%;
  }
  .card-container {
    display: flex;
    justify-content: space-between;
  }
  .card {
    margin-top: 39px;
    width: 280px;
    height: 328px;
    border: 1px solid #e1e1e1;
  }
  .card-disabled {
    opacity: 0.5;
  }
  .article {
    padding: 16px 0 23px 24px;
    font-size: 18px;
    line-height: 150%;
    color: #343030;
    font-weight: 400;
  }
  &__buy {
    display: flex;
    align-items: center;
  }
  &__price {
    padding-left: 24px;
    padding-right: 26px;
  }
  h4 {
    font-family: "Merriweather", serif;
    font-weight: 300;
    font-size: 14px;
    line-height: 150%;
    text-decoration-line: line-through;
    color: #a0a0a0;
  }
  h2 {
    font-family: "Merriweather", serif;
    font-weight: 700;
    font-size: 15px;
    line-height: 150%;
    color: #343030;
  }
  .sold {
    padding-top: 12px;
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
</style>