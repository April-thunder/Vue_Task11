<template>
  <section class="form-section">
    <div class="container">
      <h2 class="form-section__title">
        Fill out the form and we will call you
      </h2>
    </div>
    <div class="form-section__container">
      <form class="form" action="#">
        <input
          class="form__input"
          type="mail"
          placeholder="Your Name"
          required
        />
        <input
          class="form__input form__input--phone"
          type="phone"
          placeholder="Phone Number"
          required
        />
        <button class="btn__call">Call Back</button>
      </form>
    </div>
    <img class="car" src="../../public/images/car.png" alt="car" />
  </section>
</template>

<style>
  
.form-section__title {
    font-weight: 700;
    font-size: 48px;
    line-height: 67px;
    text-align: center;
    padding-top: 88px;
    margin: 0 auto 48px auto;
    max-width: 500px;
}

.form-section__container {
    margin: 0 auto;
    max-width: 850px;
}

.form__input {
    width: 253px;
    height: 56px;
    border: none;
    border-radius: 57px;
    font-weight: 400;
    font-size: 14px;
    line-height: 140%;
    padding-left: 30px;
}

.form__input--phone {
    margin-left: 42px;
    margin-right: 38px;
}

.btn__call {
    width: 253px;
    height: 56px;
    border: none;
    background: linear-gradient(180deg, #fe5626 0%, #f23f0e 100%), #59aaf1;
    box-shadow: 0px 4px 8px rgba(205, 169, 41, 0.26);
    border-radius: 59px;
    color: #fff;
    font-weight: 700;
    font-size: 18px;
    line-height: 140%;
    cursor: pointer;
}

.car {
    position: absolute;
    bottom: -65px;
    left: 50%;
    margin-left: -342px;
}
</style>