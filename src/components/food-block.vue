<template>
    <div class="food-block">
        <img class="food-frame" src="/public/images/frame.svg" alt="frame" />
          <div class="food-block__content">
            <img
              class="pizza-image"
              :src="'../../public/images/' + product_data.image"
              alt="pizza-img"
            />
            <div class="pizza__title-block">
              <h3 class="pizza-title">{{product_data.name}}</h3>
              <p class="pizza-size">32cm</p>
            </div>
            <p class="pizza-ingredient">
              Dough, Mozzarella, Cheddar, Blue, Parmesan
            </p>
            <p class="pizza-price">{{product_data.price}}</p>
            <button class="basket" 
                    @click="counter()">
                    <img class="basket-icon" src="../../public/images/pizz-block-icon.svg" alt="basket-icon"/>
            </button>
          </div>
    </div>
  </template>
  
  <script>
    export default {
        name: "food-block",
        props: 
          {
          product_data: {
            type: Object,
            default() {
              return {}
            }
          }},
          counter: {
            type: String,
            default() {
              return {}
            }
          },
        
        data() {
            return{}
        },
        computed: {},
        methods: {
          // counter() {
          //   this.$emit('counter')++
          // }
          
        }
      }
  
  </script>
  
  <style>
    .food-block {
      position: relative;
      width: 260px;
      margin: 0 20px 18px 20px;
    }

    .food-block__content {
      width: 100%;
      position: absolute;
      top: 0;
    }

    .pizza-image {
      margin: 30px auto 0 auto;

      object-fit: contain;
      width: 213px;
      height: 210px;
    }

    .pizza__title-block {
      display: flex;
      justify-content: space-between;
      align-items: center;
      max-width: 230px;
      margin: 0 auto;
    }

    .pizza-title {
      font-weight: 600;
      font-size: 16px;
      line-height: 140%;
    }

    .pizza-size {
      font-weight: 400;
      font-size: 12px;
      line-height: 140%;
    }

    .pizza-ingredient {
      max-width: 230px;
      margin: 0 auto;
      font-weight: 400;
      font-size: 12px;
      line-height: 140%;
      height: 40px;
    }

    .pizza-price {
      text-align: center;
      color: #121146;
      font-weight: 300;
      font-size: 24px;
      line-height: 140%;
      margin-top: 25px;
    }

    .basket {
      margin: 15px auto 0 auto;
      border: 2px solid #eceef6;
      background: transparent;
      width: 33px;
      height: 33px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      transition: 0.3s ease-in-out;
    }

    .basket:hover {
      transform: translateY(-3px);
      transition: 0.3s ease-in-out;
    }
  </style>