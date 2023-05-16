<template>
  <div class="product">
    <a href="#" class="product__link">
      <img
        class="product__img"
        src="../assets/images/product/product1.jpg"
        alt="Товар"
      />
      <span class="tip">-32%</span>
    </a>
    <span class="tip">Акция!</span>
    <h2 class="product__title">Керамический блок Керакам X2 (КПНФ 2)</h2>
    <p class="product__text">
      Двойной кирпич. Имеет теплопроводность, более чем в 2,5 раза ниже, в
      сравнении с полнотелым кирпичом. Используется ..
    </p>
    <div class="product__price-box">
      <div class="product__price product__price-one">
        <span>26</span><span>₽/шт.</span>
      </div>
      <div class="product__price product__price-size">
        <span>5 800</span><span>₽/м3</span>
      </div>
    </div>
    <button class="product__btn">В корзину</button>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
/* COLOR */
$green: #b7c947;
$pistachio: #7f9d87;
$main-text: #1f1f1f;
$orange: #f59127;
$red: #d13324;
$grey: #586067;
$link: #49a9ef;
$footer-bg: #718e79;
$title-modal: #586067;

.product {
  display: flex;
  flex-direction: column;
  width: 235px;
  color: $main-text;
}

.product__link {
  position: relative;

  .tip {
    top: 15px;
    right: 0;
  }
}
.product__img {
  max-width: 100%;
  border: 1px solid rgba(0, 0, 0, 0.08);
  border-radius: 8px;
}
.product__title {
  font-weight: 600;
  font-size: 18px;
  line-height: 23px;
  margin: 18px 0 9px;
}
.product__text {
  font-weight: 400;
  font-size: 16px;
  line-height: 22px;
  color: $grey;
  margin-bottom: 11px;
  flex-grow: 1;
}

.product__price {
  display: flex;
  align-items: baseline;
  gap: 5px;
}
.product__price-box {
  display: flex;
  flex-direction: column;
  gap: 3px;
  margin-bottom: 21px;
}
.product__price-one {
  span:nth-child(1) {
    font-style: normal;
    font-weight: 700;
    font-size: 26px;
    line-height: 32px;
  }
  span:nth-child(2) {
    font-weight: 400;
    font-size: 16px;
    line-height: 21px;
  }
}
.product__price-size {
  span:nth-child(1) {
    font-style: normal;
    font-weight: 700;
    font-size: 26px;
    line-height: 32px;
    color: $title-modal;
  }
  span:nth-child(2) {
    font-weight: 400;
    font-size: 13px;
    line-height: 17px;
    color: $title-modal;
  }
}
.product__btn {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 8px 20px 9px;
  min-width: 114px;
  height: 38px;
  border: 1px solid #7f9d87;
  border-radius: 3px;
  background-color: #ffffff;
  font-weight: 400;
  font-size: 16px;
  line-height: 21px;
  color: $pistachio;
  cursor: pointer;

  &:hover {
    background-color: $pistachio;
    color: #ffffff;
    transition: all 0.5s;
  }
}
</style>