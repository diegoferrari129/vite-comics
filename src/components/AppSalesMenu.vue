<script>
    import digitalComicsImg from '../assets/img/buy-comics-digital-comics.png';
    import merchandiseImg from '../assets/img/buy-comics-merchandise.png';
    import subscriptionImg from '../assets/img/buy-comics-subscriptions.png';
    import shopLocatorImg from '../assets/img/buy-comics-shop-locator.png';
    import dcPowerVisaImg from '../assets/img/buy-dc-power-visa.svg';
export default {
    data() {
        return {
            salesMenu: [
                {   
                    label: 'DIGITAL COMICS',
                    img: digitalComicsImg,
                },
                {   
                    label: 'DC MERCHANDISE',
                    img: merchandiseImg,
                },
                {   
                    label: 'SUBSCRIPTION',
                    img: subscriptionImg,
                },
                {   
                    label: 'COMIC SHOP LOCATOR',
                    img: shopLocatorImg,
                },
                {   
                    label: 'DC POWER VISA',
                    img: dcPowerVisaImg,
                },
            ]
        }
    },
}
</script>

<template>
    <div class="sales">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="sales__menu">
                        <ul>
                            <li v-for="buy, index in salesMenu" :key="index"> 
                                <div class="prod">
                                    <img :src="buy.img" :alt="buy.label"> 
                                    <a :href="buy.url">{{buy.label}}</a>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

    .sales {
        background-color: $active__color;
        min-height: 150px;
    }

    .sales__menu {

        ul {
            list-style-type: none;
            display: flex;
            justify-content: center;
            margin-top: 50px;
            
            
            li {
                padding: 0px 30px;
                color: white;

                img {
                    padding-right: 10px;
                    max-width: 50px;
                }
            }
        }
    }

</style>