<template>
    <!-- <div class="hero-image">
        <img src="../assets/nails-snow.jpg" class="img-fluid" alt="">
        <div class="hero-text">
            <h1>Verdant Nails</h1>
            
        </div>
    </div> -->
    <div class="container-fluid px-0">
        <div class="row px-0 no-gutters">
            <div class="col-12">
                <div class="carousel slide" data-ride="carousel" id="heroImageCarousel">
                    <ol class="carousel-indicators">
                        <li class="active" data-target="#heroImageCarouselCaptions" data-slide-to="0"></li>
                        <li data-target="##heroImageCarouselCaptions" data-slide-to="1"></li>
                        <li data-target="##heroImageCarouselCaptions" data-slide-to="2"></li>
                    </ol>
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                            <img src="../assets/nails-snow.jpg" class="d-block w-100" alt="">
                            <div class="carousel-caption d-none d-md-block">
                                <div class="hero-text">
                                    <h1>Verdan Nails</h1>
                                    <p>Lorem ipsum dolor sit amet.</p>
                                </div>
                            </div>
                        </div>
                        <div class="carousel-item">
                            <img src="../assets/ombre-nails.jpg" class="d-block w-100" alt="">
                            <div class="carousel-caption d-none d-md-block">
                                <div class="hero-text">
                                    <h1>Verdan Nails</h1>
                                    <p>Lorem ipsum dolor sit amet.</p>
                                </div>
                            </div>
                        </div>
                        <div class="carousel-item">
                            <img src="../assets/nails-black.jpg" class="d-block w-100" alt="">
                            <div class="carousel-caption d-none d-md-block">
                                <div class="hero-text">
                                    <h1>Verdan Nails</h1>
                                    <p>Lorem ipsum dolor sit amet.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "HeroImage",
    props: {
        heroImage: String,
    },
    created(){
        
    },
    computed: {
        cssVars(){
            return {
                '--heroImage': this.heroImage,
            }
        }
    }
}
</script>

<style scoped>
    /* .hero-image{
        background-image: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('../assets/nails-snow.jpg');
        height: 50%;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
    } */
    .hero-text{
        background-color: rgba(0, 0, 0, 0.3);
        text-align: center;
        position:absolute;
        top: -500%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white;
        padding: 1rem;
    }
</style>