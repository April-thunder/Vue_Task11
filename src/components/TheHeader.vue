<template>
  <header class="header">
    <div class="container">
      <div class="header-wrapper">
        <ul class="menu-list">
          <li class="menu-item">
            <a class="menu-link" href="#">Payment</a>
          </li>
          <li class="menu-item">
            <a class="menu-link" href="#">About Us</a>
          </li>
          <li class="menu-item">
            <a class="menu-link" href="#">Contacts</a>
          </li>
        </ul>
        <img class="logo-image" src="/images/logo.svg" alt="logo" />
        <div class="header-communication">
          <p class="work-time">Daily 11am - 9pm</p>
          <a class="phone-link" href="tel:+0 800 33 08 98">0 800 33 08 98</a>
        </div>
      </div>
    </div>
  </header>
</template>

<style>
.header {
  background: #f0f5fb;
}

.header-wrapper {
  max-width: 1160px;
  padding: 36px 0 0 0;
  margin: 0 auto;
}

.header-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.menu-list {
  display: flex;
  justify-content: space-between;
}

.header-communication {
  display: flex;
  justify-content: space-between;
}

.menu-item:nth-child(2) {
  margin: 0 40px;
}

.menu-link {
  color: #000000;
}

.work-time {
  color: #000000;
  padding: 10px 0px;
}

.phone-link {
  background-image: url("/images/phone.svg");
  background-repeat: no-repeat;
  background-position: middle left;
  padding: 10px 0px 10px 55px;
  margin-left: 35px;
  background-size: 50px;
  font-weight: 700;
  font-size: 18px;
  line-height: 22px;
  color: #000000;
}
</style>