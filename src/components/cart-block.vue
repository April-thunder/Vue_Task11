<template>
  <div class="cart-block">
    <img class="cart-image" src="../../public/images/shopping-bag.png" alt="cart" />
    <p class="cart-quantity">{{counter}}</p>
  </div>
</template>

<script>
    export default {
        name: "cart-block",
        props: {},
        data() {
            return{
                counter: 0
            }
        },
        computed: {}
}
</script>

<style>
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