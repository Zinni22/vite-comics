<script>
export default {

  name: 'MainApp',

    data () {
        return{

        }
    }

}
</script>

<template>

    <main>

        <!-- SEZIONE CONTENUTI  -->
        <section id="content-section">
            <h2>
                --> Content goes here &lt;--
            </h2>
        </section>

        <!-- SEZIONE AZZURRA -->
        <section id="blue-section">

            <ul>
                <li><a href="#">
                    <img src="../img/buy-comics-digital-comics.png" alt="digital-comics">
                    DIGITAL COMICS
                </a></li>

                <li><a href="#">
                    <img src="../img/buy-comics-merchandise.png" alt="merchandise-comics">
                    DC MERCHANDISE
                </a></li>

                <li><a href="#">
                    <img src="../img/buy-comics-subscriptions.png" alt="subscription-comics">
                    SUBSCRIPTION
                </a></li>

                <li><a href="#">
                    <img src="../img/buy-comics-shop-locator.png" alt="shop-locator-comics">
                    COMIC SHOP LOCATOR
                </a></li>

                <li><a href="#">
                    <img src="../img/buy-dc-power-visa.svg" alt="power-visa-comics" class="small-picture">
                    DS POWER VISA
                </a></li>
            </ul>

        </section>

        
    </main>
 
</template>

<style lang="scss" scoped>

//GENERALI
@mixin container-base{
    max-width: 1000px;
    margin: 0 auto;
}

$flex: flex;

$primary-blue: #0282f9;

    // MAIN
    main{
        background-color: black;

        #content-section{
            @include container-base;
            padding: 50px 0;

            h2{
                color: white;
            }
        }

        #blue-section{
            background-color: $primary-blue;
            padding: 40px 0;

            ul{
                @include container-base;
                display: $flex;

                li{
                    padding: 0 20px;
                    height: 50px;
                    a{
                        height: 100%;
                        color: white;
                        display: $flex;
                        align-items: center;
                        font-size: 0.8rem;
                        img{
                            height: 100%;
                            margin-right: 10px;

                            &.small-picture{
                                width: 50px;
                            }
                        }
                        
                    }
                    
                }
            }
        }
        
    }



</style>
