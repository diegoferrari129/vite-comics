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
    <div>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="d-flex justify-content-between">
                        <!-- logo -->
                        <div>
                            <img src="" alt="">
                        </div>

                        <!-- menu -->
                        <div>
                            <ul class="list-unstyled d-flex">
                                <li v-for="link, index in links" :key="index">
                                    <a :href="link.url" :class="link.current ? 'active' : ''">{{ link.label }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
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
            padding-bottom: 30px;
            border-bottom: 5px solid #0282f9;
        }
    }
</style>