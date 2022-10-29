<template>
    <section class="main-section">
        <div class="container container-main">
            <div class="main-descr">
                <h1 class="main-title">Food delivery in Kovel</h1>
                <p class="main-text">
                    If you decide to relax or have unexpected guests, call us.
                    We make sure that your vacation is comfortable, enjoyable
                    and delicious
                </p>
            </div>
            <img
                class="main-image"
                src="/images/main.png"
                alt="pizza-image"
            />
        </div>
    </section>
</template>

<style>
    .main-section {
        background: #f0f5fb;
    }

    .main-descr {
        margin: 0 auto;
        padding-top: 95px;
        padding-bottom: 507px;
        max-width: 630px;
    }

    .main-title {
        text-align: center;
        font-weight: 700;
        font-size: 48px;
        line-height: 59px;
    }

    .main-text {
        text-align: center;
        font-weight: 400;
        font-size: 18px;
        line-height: 140%;
        padding-top: 18px;
    }

    .container-main {
        position: relative;
    }

    .main-image {
        position: absolute;
        top: 210px;
        left: 50%;
        max-width: 860px;
        margin-left: -330px;
    }
</style>