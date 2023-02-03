<script>
export default {

    name: 'HeaderApp',

    data () {
        return{

            links: [
                {
                    name: 'CHARACTERS',
                    url:'#',
                    active: false,
                },
                {
                    name: 'COMICS',
                    url:'#',
                    active: true,
                },
                {
                    name: 'MOVIES',
                    url:'#',
                    active: false,
                },
                {
                    name: 'TV',
                    url:'#',
                    active: false,
                },
                {
                    name: 'GAMES',
                    url:'#',
                    active: false,
                },
                {
                    name: 'COLLECTIBLES',
                    url:'#',
                    active: false,
                },
                {
                    name: 'VIDEOS',
                    url:'#',
                    active: false,
                },
                {
                    name: 'FANS',
                    url:'#',
                    active: false,
                },
                {
                    name: 'NEWS',
                    url:'#',
                    active: false,
                },
                {
                    name: 'SHOP',
                    url:'#',
                    active: false,
                },

            ]

        }
    }

}
</script>

<template>

    <header>

        <div>

            <img src="../img/dc-logo.png" alt="blue-logo">

            <ul>
                <li v-for="link in links"
                :class="{
                    active: link.active == true
                }"
                >
                    <a :href="link.url">
                    {{ link.name }}
                    </a>
                </li>
            </ul>

        </div>

    </header>
 
</template>

<style lang="scss">

    // HEADER
    header{
        background-color: white;

        div{
            height: 60px;
            @include container-base;

            justify-content: space-between;
            align-items: center;

            img{
                height: 50px;
            }

            ul{
                height: 100%;
                display: flex;

                li {
                    font-size: 0.8rem;
                    font-weight: bold;
                    padding: 0 15px;

                    display: flex;
                    align-items: center;

                    a{
                        color: black;
                    }
                    
                    &.active{
                        border-bottom: 2px solid $primary-blue;

                        a{
                            color: $primary-blue; 
                        }
                    }

                }
                li:hover{
                    background-color: lightgray;
                    cursor: pointer;
                }
            }
        }
    }

</style>
