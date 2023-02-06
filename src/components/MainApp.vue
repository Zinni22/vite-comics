<script>
import CardElement from './CardElement.vue';

export default {

  name: 'MainApp',

  components: {
    CardElement
  },

    data () {
        return{

            comics: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]

        }
    }

}
</script>

<template>

    <main>

        <!-- SEZIONE CONTENUTI  -->
        <section id="content-section">
            
            <div class="jumbo">
                <!-- <img src="../img/jumbotron.jpg" alt="jumbo"> -->
            </div>

            <div class="card-container">
                <div>


                    <CardElement v-for="comic in comics" 
                        class="card"
                        :src="comic.thumb"
                        :title="comic.series"
                    />
                    
                    <button class="current-button">
                        CURRENT SERIES
                    </button>

                    <button>
                        LOAD MORE
                    </button>

                </div>
            </div>

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

    // MAIN
    main{
        padding-top: 60px;

        #content-section{
            .jumbo{
                height: 350px;
                background-image: url("../img/jumbotron.jpg");
                background-size: cover;
            }

            .card-container{
                background-color: #1c1c1c;
                padding: 50px 0;

                div{
                    @include container-base;
                    justify-content: space-between;
                    flex-wrap: wrap;
                    position: relative;

                    .card{
                        width: calc(100% / 6 - 10px);
                        display: block;
                        cursor: pointer;
                    }

                    button{
                        background-color: $primary-blue;
                        border: none;
                        padding: 10px;
                        color: white;
                        font-weight: bold;
                        margin: 0 auto;
                        cursor: pointer;
                    }

                    .current-button{
                        position: absolute;
                        top: -80px;
                        padding: 20px;
                        font-size: 1.2rem;
                    }
                }
            }
        }

        #blue-section{
            background-color: $primary-blue;
            padding: 40px 0;

            ul{
                @include container-base;

                li{
                    padding: 0 20px;
                    height: 50px;
                    a{
                        height: 100%;
                        color: white;
                        display: flex;
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
