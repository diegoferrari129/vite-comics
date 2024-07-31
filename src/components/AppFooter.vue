<script>
export default {

}
</script>

<template>
    <footer>
        <!-- top footer -->
        <div class="container">
            <div class="top__footer">
                <div class="row">
                    <div class="col-4">
                        <div class="row g-3">
                            <div class="col-4">
                                <div class="footer__content">
                                    <h5 class="footer__content__title">DC COMICS</h5>
                                    <ul>
                                        <li>
                                            <a href="#">Characters</a>
                                        </li>
                                        <li>
                                            <a href="#">Comics</a>
                                        </li>
                                        <li>
                                            <a href="#">Movies</a>
                                        </li>
                                        <li>
                                            <a href="#">TV</a>
                                        </li>
                                        <li>
                                            <a href="#">Games</a>
                                        </li>
                                        <li>
                                            <a href="#">Videos</a>
                                        </li>
                                        <li>
                                            <a href="#">News</a>
                                        </li>
                                    </ul>
                                    <div class="pt-3">
                                        <h5 class="footer__content__title">SHOP</h5>
                                        <ul>
                                            <li>
                                                <a href="#">Shop DC</a>
                                            </li>
                                            <li>
                                                <a href="#">Shop DC Collectibles</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                            <div class="col-4">
                                <div class="footer__content">
                                    <h5 class="footer__content__title">DC</h5>
                                    <ul>
                                        <li>
                                            <a href="#">Terms Of Use</a>
                                        </li>
                                        <li>
                                            <a href="#">Privacy Police(New)</a>
                                        </li>
                                        <li>
                                            <a href="#">Ad Choices</a>
                                        </li>
                                        <li>
                                            <a href="#">Advertising</a>
                                        </li>
                                        <li>
                                            <a href="#">Jobs</a>
                                        </li>
                                        <li>
                                            <a href="#">Subscriptions</a>
                                        </li>
                                        <li>
                                            <a href="#">Talent Workshops</a>
                                        </li>
                                        <li>
                                            <a href="#">CPSC Certificate</a>
                                        </li>
                                        <li>
                                            <a href="#">Ratings</a>
                                        </li>
                                        <li>
                                            <a href="#">Shop Help</a>
                                        </li>
                                        <li>
                                            <a href="#">Contact Us</a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="col-4">
                                <div class="footer__content">
                                    <h5 class="footer__content__title">SITES</h5>
                                    <ul>
                                        <li>
                                            <a href="#">DC</a>
                                        </li>
                                        <li>
                                            <a href="#">MAD Magazine</a>
                                        </li>
                                        <li>
                                            <a href="#">DC Kids</a>
                                        </li>
                                        <li>
                                            <a href="#">DC Universe</a>
                                        </li>
                                        <li>
                                            <a href="#">DC Power Visa</a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom__footer">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <div class="d-flex justify-content-between align-items-center">
                            <div class="button__footer">
                                <button>SIGN-UP NOW!</button>
                            </div>
                            <div class="social">
                                <h5>FOLLOW US</h5>
                                <img src="../assets/img/footer-facebook.png" alt="">
                                <img src="../assets/img/footer-twitter.png" alt="">
                                <img src="../assets/img/footer-youtube.png" alt="">
                                <img src="../assets/img/footer-pinterest.png" alt="">
                                <img src="../assets/img/footer-periscope.png" alt="">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
    
</template>


<style lang="scss" scoped>
    footer {
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
    }

    .top__footer {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;

        .footer__content{
            padding: 40px 0px;

            .footer__content__title{
                color: white;
                font-weight: 600;
            }
    
            ul {
                list-style-type: none;
                padding: 0;
                margin: 0;
                
                li{
                    font-size: 14px;
                    padding: 0;
                    margin: 0;
                    
                    a{
                        text-decoration: none;
                        color: #959595;
                    }
                }
            }
        }
    }

    .bottom__footer {
        background-color: #303030;
        display: flex;
        align-items: center;
        min-height: 100px;

        .button__footer {
            
            button {
                background-color: #303030;
                color: white;
                font-weight: 600;
                padding: 10px;
                border: 2px solid #0282f9;
            }
        }

        .social {
            display: flex;
            align-items: center;

            h5 {
                color: #0282f9;
                font-weight: 700;
                margin-right: 10px;
            }

            img {
                margin: 0px 7px;
            }
        }
    }
</style>