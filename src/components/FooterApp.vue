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

    </footer>
 
</template>

<style lang="scss" scoped>
// GENRALI
@mixin container-base{
    max-width: 1000px;
    margin: 0 auto;
}

$flex: flex;

$primary-blue: #0282f9;

    // FOOTER
    footer{

        #main-section{
            background-image: url(../img/footer-bg.jpg);
            padding: 50px 0;

            div{
                @include container-base;
                display: $flex;

                ul{
                    margin-right: 40px;

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
                }
            }

        }

    }


        

</style>
