<template>
    <div class="blue-nav">
        <div class="container">
            <div class="blue-nav__card">
                <img src="../assets/buy-comics-digital-comics.png" alt="">
                <span>Digital comics</span>
            </div>
            <div class="blue-nav__card">
                <img src="../assets/buy-comics-merchandise.png" alt="">
                <span>DC merchandise</span>
            </div>
            <div class="blue-nav__card">
                <img src="../assets/buy-comics-subscriptions.png" alt="">
                <span>Subscription</span>
            </div>
            <div class="blue-nav__card">
                <img src="../assets/buy-comics-shop-locator.png" alt="">
                <span>Comic shop locator</span>
            </div>
            <div class="blue-nav__card">
                <img src="../assets/buy-dc-power-visa.svg" alt="">
                <span>DC power Visa</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "MyBlueNav",    
}
</script>

<style scoped lang="scss">
@import "../style/variables.scss";

.blue-nav {
    height: 150px;
    background-color: $brand-primary-color;
    
    &__card {
        width: calc(100% / 5);
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;

        span {
            color: white;
            text-transform: uppercase;
        }

        img {
            width: auto;
            height: 33%;
            margin-right: 1rem;
        }
    }
}

.container {
    display: flex;
    height: 100%;
    justify-content: space-around;
}

</style>