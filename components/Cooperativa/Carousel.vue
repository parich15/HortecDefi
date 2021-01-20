<template>
  <div id="containerCarousel" @contextmenu="noclick()">
    <b-carousel
      id="CarCoop"
      style="text-shadow: 0px 0px 10px #000"
      fade
      indicators
      img-width="1400"
      img-height="700"
    >
      <b-carousel-slide
        :caption="$t('Slider.txt1')"
        img-src="/img/carousel2.jpg"
      />
      <b-carousel-slide
        :caption="$t('Slider.txt2')"
        img-src="/img/carousel1.jpg"
      />
      <b-carousel-slide
        :caption="$t('Slider.txt3')"
        img-src="/img/carousel3.jpg"
      />
      <b-carousel-slide
        :caption="$t('Slider.txt4')"
        img-src="/img/carousel4.jpg"
      />
    </b-carousel>
  </div>
</template>

<script>
export default {
  name: 'Carousel',
  data () {
    return {
      nombre: 'Carousel'
    }
  },
  methods: {
    noclick () {
      document.getElementById('containerCarousel').addEventListener('contextmenu', function (e) {
        e.preventDefault()
      }, false)
    }
  }
}
</script>

<style>

</style>
