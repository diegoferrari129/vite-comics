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
                    url: '#',
                },
                {   
                    label: 'DC MERCHANDISE',
                    img: merchandiseImg,
                    url: '#',
                },
                {   
                    label: 'SUBSCRIPTION',
                    img: subscriptionImg,
                    url: '#',
                },
                {   
                    label: 'COMIC SHOP LOCATOR',
                    img: shopLocatorImg,
                    url: '#',
                },
                {   
                    label: 'DC POWER VISA',
                    img: dcPowerVisaImg,
                    url: '#',
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
                                </div>
                                <a :href="buy.url">{{buy.label}}</a>
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
        min-height: 140px;
    }

    .sales__menu {

        ul {
            list-style-type: none;
            display: flex;
            justify-content: center;
            justify-content: space-around;
            margin-top: 45px;
            
            li {
                padding: 0px 30px;
                color: white;
                display: flex;
                align-items: center;

                .prod {
                    width: 50px;
                    height: 50px;
                    display: flex;
                    margin-right: 5px;
                    
                    img {
                        object-fit: contain;
                    }

                }

                a {
                    text-decoration: none;
                    color: white;
                }
            }
        }
    }

</style>