<template>
  <section class="TheDishesSection">
    <div class="container">
      <div class="cart-wrapper">
        <div class="price-block">
          <p class="price-line">
            = <span class="price"> {{ priceCounter }} р</span>
          </p>
        </div>
        <div class="cart-block">
          <img class="cart-image" src="/images/shopping-bag.png" alt="cart" />
          <p class="cart-quantity">{{ counterParent }}</p>
        </div>
      </div>
      <h2 class="dishes-section__title">Popular dishes</h2>
      <div class="tabs-wrapper">
        <button class="tab">All</button>
        <button class="tab">Pizza</button>
        <button class="tab">Sushi</button>
        <button class="tab">Salad</button>
        <button class="tab">Dessert</button>
        <button class="tab">Drinks</button>
      </div>
      <div class="food-wrapper">
        <TheFoodBlock
          v-for="product in products"
          :key="product.article"
          v-bind:product_data="product"
          @counter="counterAdd"
        />
      </div>
      <button class="update-btn">
        <img
          class="update-img"
          src="/images/update-btn.svg"
          alt="update-image"
        />
      </button>
    </div>
  </section>
</template>
<script>
import TheFoodBlock from "./TheFoodBlock.vue";
export default {
  name: "TheDishesSection",
  components: {
    TheFoodBlock,
  },
  props: {},
  data() {
    return {
      products: [
        {
          image: "pizza_quattro.png",
          name: "Quattro formaggie",
          price: 290,
          article: "t1",
          cathegory: "pizza",
        },
        {
          image: "sushi_double-trouble.png",
          name: "Double Trouble Sushi",
          price: 280,
          article: "t2",
          cathegory: "sush",
        },
        {
          image: "dessert_choco.png",
          name: "Cocao Dessert",
          price: 135,
          article: "t3",
          cathegory: "dessert",
        },
        {
          image: "classic_sushi.png",
          name: "Classic Sushi",
          price: 250,
          article: "t4",
          cathegory: "sushi",
        },
        {
          image: "salad_caesar.png",
          name: "Salad Caesar",
          price: 305,
          article: "t5",
          cathegory: "salad",
        },
        {
          image: "sushi_set.png",
          name: "Sushi Set",
          price: 355,
          article: "t6",
          cathegory: "sushi",
        },
        {
          image: "Coca-Cola.png",
          name: "Coca Cola",
          price: 80,
          article: "t7",
          cathegory: "drink",
        },
        {
          image: "pizza_carbonara.png",
          name: "Pizza Carbonara",
          price: 341,
          article: "t8",
          cathegory: "pizza",
        },
        {
          image: "salad_cyliner.png",
          name: "Salad Cylinder",
          price: 288,
          article: "t9",
          cathegory: "pizza",
        },
        {
          image: "dessert_berry.png",
          name: "Berry Desert",
          price: 180,
          article: "t10",
          cathegory: "dessert",
        },
        {
          image: "pizza_dimare.png",
          name: "Pizza DiMare",
          price: 341,
          article: "t11",
          cathegory: "pizza",
        },
        {
          image: "salad_see.png",
          name: "Sea Salad",
          price: 399,
          article: "t12",
          cathegory: "salad",
        },
      ],
      counterParent: 0,
      priceCounter: 0,
    };
  },
  computed: {},
  methods: {
    counterAdd() {
      this.counterParent++;
    },
    priceAdd() {
      this.priceCounter++;
    },
  },
  watch: {},
};
</script>

<style>
.cart-wrapper {
  display: flex;
  justify-content: end;
  align-items: center;
  margin: 0 auto;
  max-width: 1320px;
  padding-top: 70px;
}
.price-block {
  background-image: url("../images/speech-bubble.png");
  background-repeat: no-repeat;
  transform: rotate(180deg);
  background-size: 100%;
  background-position: center;
  width: 130px;
  height: 50px;
  position: relative;
  margin-right: 10px;
}
.price-line {
  color: #fff;
  position: absolute;
  transform: rotate(180deg);
  top: 31%;
  left: 40%;
}
.dishes-section__title {
  font-weight: 700;
  font-size: 48px;
  line-height: 59px;
  text-align: center;
  margin-bottom: 50px;
}
.tabs-wrapper {
  max-width: 830px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}
.tab {
  background: #eceef6;
  border-radius: 45px;
  border: none;
  font-weight: 600;
  font-size: 16px;
  line-height: 140%;
  text-align: center;
  width: 135px;
  padding: 17px;
  cursor: pointer;
  color: #000000;
  transition: 0.5s;
}
.tab:hover {
  background: #59aaf1;
  color: #fff;
  transition: 0.5s;
}
.food-wrapper {
  margin: 47px auto 0 auto;
  max-width: 1200px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.update-btn {
  display: block;
  margin: 40px auto 0 auto;
  background-color: transparent;
  border: none;
  transition: 0.3s ease-in-out;
  display: flex;
  cursor: pointer;
}
.update-btn:hover {
  transform: scale(110%);
  transition: 0.3s ease-in-out;
}

/* cart styles */
.cart-block {
  position: relative;
  width: 70px;
  border-radius: 50%;
  box-shadow: 2px 2px 28px 12px rgba(34, 60, 80, 0.2);
}

.cart-image {
  transform: scale(70%);
}

.cart-quantity {
  position: absolute;
  bottom: -10px;
  right: -14px;
  background-color: tomato;
  border-radius: 50%;
  width: 35px;
  height: 35px;
  color: #fff;
  text-align: center;
  padding-top: 7px;
}
</style>
