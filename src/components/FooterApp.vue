<script>
export default {

  name: 'FooterApp',

    data () {
        return{

        }
    }

}
</script>

<template>

    <footer>

        <!-- SEZIONE PRINCIPALE -->
        <section id="main-section">

            <div>

                <ul>
                    <h4>DC COMICS</h4>

                    <li><a href="#">
                        Characters
                    </a></li>

                    <li><a href="#">
                        Comics
                    </a></li>

                    <li><a href="#">
                        Movies
                    </a></li>

                    <li><a href="#">
                        TV
                    </a></li>

                    <li><a href="#">
                        Games
                    </a></li>

                    <li><a href="#">
                        Videos
                    </a></li>

                    <li><a href="#">
                        News
                    </a></li>
                    
                </ul>

                <ul>
                    <h4>DC</h4>

                    <li><a href="#">
                        Terms of Use
                    </a></li>

                    <li><a href="#">
                        Privacy Policy (New)
                    </a></li>

                    <li><a href="#">
                        Ad Choices
                    </a></li>

                    <li><a href="#">
                        Advertising
                    </a></li>

                    <li><a href="#">
                        Jobs
                    </a></li>

                    <li><a href="#">
                        Subscription
                    </a></li>

                    <li><a href="#">
                        Talent Workspace
                    </a></li>

                    <li><a href="#">
                        CPSC Certificates
                    </a></li>

                    <li><a href="#">
                        Ratings
                    </a></li>
                    
                    <li><a href="#">
                        Shop Help
                    </a></li>

                    <li><a href="#">
                        Contact Us
                    </a></li>
                </ul>

                <ul>
                    <h4>SITIES</h4>

                    <li><a href="#">
                        DC
                    </a></li>

                    <li><a href="#">
                        MAD Magazine
                    </a></li>

                    <li><a href="#">
                        DC Kids
                    </a></li>

                    <li><a href="#">
                        DC Universe
                    </a></li>

                    <li><a href="#">
                        DC Power Visa
                    </a></li>
                </ul>

                <img src="../img/dc-logo-bg.png" alt="logo-backgroud-big">

            </div>


        </section>

        <!-- SEZIONE SUBSCRIBE -->
        <section id="subscribe-section">

            <div>

                <button>
                    SIGN-UP NOW!
                </button>

                <ul>
                    <li><a href="#">FOLLOW US</a></li>

                    <li><a href="#">
                        <img src="../img/footer-facebook.png" alt="facebook-footer">
                    </a></li>

                    <li><a href="#">
                        <img src="../img/footer-twitter.png" alt="twitter-footer">
                    </a></li>

                    <li><a href="#">
                        <img src="../img/footer-youtube.png" alt="youtube-footer">
                    </a></li>

                    <li><a href="#">
                        <img src="../img/footer-pinterest.png" alt="pinterest-footer">
                    </a></li>

                    <li><a href="#">
                        <img src="../img/footer-periscope.png" alt="periscope-footer">
                    </a></li>
                    
                </ul>

            </div>

        </section>

    </footer>
 
</template>

<style lang="scss" scoped>

    // FOOTER
    footer{

        #main-section{
            background-image: url(../img/footer-bg.jpg);
            background-size: contain;

            div{
                @include container-base;

                ul{
                    margin-right: 40px;
                    margin-top: 50px;

                    h4{
                        color: white;
                        margin-bottom: 15px;
                    }

                    li{
                        padding: 5px 0;
                        a{
                            color: gray;
                        }
                    }
                }

                img{
                    width: 50%;
                }

            }

        }

        #subscribe-section{
            background-color: #303030;
            padding: 30px 0;

            div{
                @include container-base;
                justify-content: space-between;

                button{
                    padding: 10px;
                    border: 1px solid $primary-blue;
                    background: none;
                    color: white;
                    cursor: pointer;
                }

                ul{
                    display: flex;
                    align-items: center;

                    li{
                        padding: 10px;

                        a{
                            color: $primary-blue;
                            font-weight: bold;

                        }
                    }
                }
            }
        }

    }


        

</style>
