<template>
<template-view>

    <!-- carousel -->
    <section>
        <carousel-component></carousel-component>
    </section>

    <section class="py-5">
        <div class="container">
            <div class="row">
                <div class="col-md-8">
                      <h1>REDEFINES THE <span class="heading">LUXURY</span><br>
                         <span class="heading">HOSPITALITY</span>EXPERIENCE</h1>
                   
                    <div>
                        <p>Dharan Kitchen is prestigious name since 2062 BS (2005 AD)
                            for serving healthy and tasty foods in reasonable price.
                            Your fun destination for food and beverages. We care about
                            your taste and health. We promise in intimate and relaxed dining
                            experience that offers something different to local and foreign dishes and
                            ensures you enjoy a memoriable food experiencene every time.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <img src="https://www.dharankitchen.com/img/slide2.jpg" alt="" class="rounded-4 " style="width:350px">
                </div>
            </div>
        </div>
    </section>

    <!-- Our Branches -->
    <section class="branches py-5">
        <div class="container">
            <div class="row">
                <div class="col-md-12">

                </div>
            </div>
        </div>
    </section>
</template-view>
</template>

<script>
// @ is an alias to /src
import TemplateView from '@/views/TemplateView'
import CarouselComponent from '@/components/CarouselComponent'
export default {
    name: 'HomeView',
    components: {
        TemplateView,
        CarouselComponent
    }
}
</script>

<style scoped>
.heading {
    color: var(--kPrimary)
}
.branches{
    content: '';
    position: absolute;
    background-image: url(https://verandah-hotel.com/wp-content/uploads/2019/11/Lobby2.jpg);
    height: 100%;
    width: 100%;
    z-index: 0;
    background-repeat: no-repeat;
    background-position: center;
}
</style>
