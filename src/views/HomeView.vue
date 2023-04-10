<template>
<template-view>

    <!-- carousel -->
    <section>
        <carousel-component></carousel-component>
    </section>

    <section>
        
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
