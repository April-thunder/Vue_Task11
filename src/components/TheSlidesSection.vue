<template>
    <section class="slides-section">
        <div class="container slides-container">
            <img class="slide" src="../images/slide01.jpg" alt="slide" />
            <img class="slide" src="../images/slide02.jpg" alt="slide" />
            <img class="slide" src="../images/slide03.jpg" alt="slide" />
            <img class="slide" src="../images/slide04.jpg" alt="slide" />
            <img class="slide" src="../images/slide05.jpg" alt="slide" />
            <img class="slide" src="../images/slide06.jpg" alt="slide" />
            <a class="insta-link" href="#">
                <p class="insta-text">
                    Instagram:
                    <span class="insta-text__address">@classic_kovel</span>
                </p>
            </a>
        </div>
    </section>
</template>

<style>
.slides-container {
    margin-top: 90px;
    display: flex;
    justify-content: space-between;
    position: relative;
}

.insta-link {
    position: absolute;
    background: linear-gradient(45.04deg, #fd9924 -51.05%, #f65b16 134.89%);
    box-shadow: 0px 70px 90px rgba(253, 55, 36, 0.2),
        0px 35px 50px rgba(253, 55, 36, 0.2),
        0px 20px 25px rgba(253, 55, 36, 0.2);
    border-radius: 15px;
    width: 480px;
    height: 180px;
    border: none;
    left: 50%;
    margin-left: -240px;
    top: 50%;
    margin-top: -90px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #ffffff;
}

.insta-text {
    border: 2px solid rgba(256, 256, 256, 0.1);
    border-radius: 15px;
    padding: 55px;
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
}

.insta-text__address {
    font-weight: 700;
}

.form-section {
    background: #f0f5fb;
    margin-top: 127px;
    position: relative;
    padding-bottom: 249px;
}

</style>
