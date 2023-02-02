<script>
export default {

    name: 'HeaderApp',

    data () {
        return{

        }
    }

}
</script>

<template>

    <header>

        <div>

            <img src="../img/dc-logo.png" alt="blue-logo">

            <ul>
                <li><a href="#">
                    CHARACTERS
                </a></li>

                <li class="active"><a href="#">
                    COMICS
                </a></li>

                <li><a href="#">
                    MOVIES
                </a>
                </li>

                <li><a href="#">
                    TV
                </a>
                </li>

                <li><a href="#">
                    GAMES
                </a>
                </li>

                <li><a href="#">
                    COLLECTIBLES
                </a>
                </li>

                <li><a href="#">
                    VIDEOS
                </a>
                </li>

                <li><a href="#">
                    FANS
                </a>
                </li>

                <li><a href="#">
                    NEWS
                </a>
                </li>

                <li><a href="#">
                    SHOP
                </a>
                </li>
            </ul>

        </div>

    </header>
 
</template>

<style lang="scss">

// GENERALI
@mixin container-base{
    max-width: 1000px;
    margin: 0 auto;
}
$flex: flex;

$primary-blue: #0282f9;

    // HEADER
    header{
        background-color: white;

        div{
            height: 60px;
            @include container-base;

            display: $flex;
            justify-content: space-between;
            align-items: center;

            img{
                height: 50px;
            }

            ul{
                height: 100%;
                display: $flex;

                li {
                    font-size: 0.8rem;
                    font-weight: bold;
                    padding: 0 15px;

                    display: $flex;
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
