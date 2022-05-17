<template>
<footer class="footer">
    <div class="container">
        <div class="footer__container">
            <div class="footer__menu">
                <div class="footer__col">
                    <div class="footer__col-up">
                        <h3>DC comics</h3>
                        <ul>
                            <li><a href="">Footer link</a></li>
                            <li><a href="">Footer link</a></li>
                            <li><a href="">Footer link</a></li>
                            <li><a href="">Footer link</a></li>
                            <li><a href="">Footer link</a></li>
                            <li><a href="">Footer link</a></li>
                            <li><a href="">Footer link</a></li>
                        </ul>
                    </div>
                    <div class="footer__col-down">
                        <h3>Shop</h3>
                        <ul>
                            <li><a href="">Footer link</a></li>
                            <li><a href="">Footer link</a></li>
                        </ul>
                    </div>
                </div>
                <div class="footer__col">
                    <h3>DC</h3>
                    <ul>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                    </ul>
                </div>
                <div class="footer__col">
                    <h3>Sites</h3>
                    <ul>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                        <li><a href="">Footer link</a></li>
                    </ul>
                </div>
            </div>
            <div class="brand__logo"></div>
        </div>
    </div>
    <div class="footer__bottom">
        <div class="container">
            <div class="footer-bottom__col-left">
                <a class="footer__register" href="">Sign-up now!</a>
            </div>
            <div class="footer-bottom__col-right">
                <span class="footer-bottom__follow">Follow us</span>
                <div class="footer-bottom__social">
                    <img src="../assets/footer-facebook.png" alt="">
                    <img src="../assets/footer-twitter.png" alt="">
                    <img src="../assets/footer-youtube.png" alt="">
                    <img src="../assets/footer-pinterest.png" alt="">
                    <img src="../assets/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </div>
</footer>
</template>

<script>
export default {
    name: "MyFooter",
};
</script>

<style scoped lang="scss">
@import "../style/variables.scss";
@import "../style/commons.scss";

.footer {
    width: 100%;
    background-image: url(../assets/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    &__container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        height: 450px;

        .footer__menu {
            display: flex;
            padding: 5rem 0;
        }

        .brand__logo {
            width: 60%;
            height: 100%;
            background-image: url(../assets/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-position-y: center;
            background-position-x: right;
        }
    }
}

.footer__col {
    margin-right: 4rem;
        h3 {
            color: white;
            margin: 1rem 0;
            text-transform: uppercase;
            font-size: 1.2rem;
        }
        a {
            color: $footer-text-color;
            font-weight: 300;
        }
}

.footer__bottom {
    background-color: $footer-bottom-color;
    
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}


.footer__register {
    color: white;
    font-size: 1.2rem;
    padding: 1rem;
    text-transform: uppercase;
    border: 3px solid $brand-primary-color;
    display: block;
    margin: 2rem 0;
}

.footer-bottom__follow {
    text-transform: uppercase;
    color: $brand-primary-color;
    font-size: 1.5rem;
    font-weight: bold;
    margin-right: 1rem;
}


.footer-bottom {
    &__col-right {
        display: flex;
        align-items: center;
    }
    
    &__social {
        display: flex;
    
    }    

    &__social img {
        margin: 0 .5rem;
    }
}
</style>