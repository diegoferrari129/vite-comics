<script>
export default {
    data() {
        return {
            links: [
                {
                    label: 'CHARACTERS',
                    url: '#',
                    current: false,
                },
                {
                    label: 'COMICS',
                    url: '#',
                    current: true,
                },
                {
                    label: 'MOVIES',
                    url: '#',
                    current: false,
                },
                {
                    label: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    label: 'GAMES',
                    url: '#',
                    current: false,
                },
                {
                    label: 'COLLECTIBLES',
                    url: '#',
                    current: false,
                },
                {
                    label: 'VIDEOS',
                    url: '#',
                    current: false,
                },
                {
                    label: 'FANS',
                    url: '#',
                    current: false,
                },
                {
                    label: 'NEWS',
                    url: '#',
                    current: false,
                },
                {
                    label: 'SHOP',
                    url: '#',
                    current: false,
                },
            ]
        }
    },
    
}
</script>

<template>
    <header class="header">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="header__content">
                        <!-- logo -->
                        <div>
                            <img src="../assets/img/dc-logo.png" alt="">
                        </div>

                        <!-- menu -->
                        <div class="header__menu">
                            <ul class="list-unstyled d-flex">
                                <li
                                  v-for="link, index in links"
                                  :key="index">
                                    <a
                                      :href="link.url"
                                      :class="link.current ? 'active' : ''">{{
                                      link.label
                                      }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    .header {
        background-color: white;
        padding: 25px 0px;

        .header__content {
            display: flex;
            justify-content: space-between;
        

            .header__menu {
                display: flex;
                align-items: center;
                
                
                ul {
                    li{
                        padding: 0px 15px;
                        font-weight: 600;
                        
                        &:hover {
                            font-weight: 800;
                        }
                        
                        a {
                            text-decoration: none;
                            color: black;
                        }
                    }
                    
                    .active {
                        color: #0282f9;
                        padding-bottom: 67px;
                        border-bottom: 7px solid #0282f9;
                    }
                }
            }
        }
    }

</style>