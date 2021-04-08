<template>
  <section id="product" class="portfolio">
      <div class="container">

        <div class="section-title">
          <h2>Our Products</h2>
          <!-- <p>Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam quos quisquam cupiditate. Et nemo qui impedit suscipit alias ea. Quia fugiat sit in iste officiis commodi quidem hic quas.</p> -->
        </div>

        <div class="row">
          <div class="col-lg-12 d-flex justify-content-center">
            <ul id="portfolio-flters">
              <li data-filter="*" class="filter-active">Ready to wear Adire Dresses</li>
              <li data-filter=".filter-app">Adire Travellers Jacket</li>
              <li data-filter=".filter-card">Palazzo Pair</li>
              <li data-filter=".filter-web">Made To Measure</li>
              <li data-filter=".filter-card">Custom Order</li>
              
            </ul>
          </div>
        </div>

        <div class="row portfolio-container">

          <div class="col-lg-4 col-md-6 portfolio-item filter-app" v-for="(obj, key) in projectJSON" :key="key">
            <img src="{{obj.img}}" class="img-fluid" alt="">
            <div class="portfolio-info">
              <h4>{{obj.info}}</h4>
              <p>{{obj.info}}</p>
              <a href="../src/assets/img/portfolio/portfolio-1.jpg" data-gall="portfolioGallery" class="venobox preview-link" title="App 1"><i class="bx bx-plus"></i></a>
              <a href="portfolio-details.html" class="details-link" title="More Details"><i class="bx bx-link"></i></a>
            </div>
          </div>

        </div>

      </div>
    </section>
</template>

<script>
export default {
  data: () =>({
    projectJSON: [
      {
        img: "../assets/img/portfolio/portfolio-1.jpg" ,
        info: "working"
      },
      {
        img: "../assets/img/portfolio/portfolio-1.jpg" ,
        info: "working"
      },
      {
        img: "../assets/img/portfolio/portfolio-1.jpg" ,
        info: "working"
      },
      {
        img: "../assets/img/portfolio/portfolio-1.jpg" ,
        info: "working"
      },
      {
        img: "../assets/img/portfolio/portfolio-1.jpg" ,
        info: "working"
      },
      {
        img: "../assets/img/portfolio/portfolio-1.jpg" ,
        info: "working"
      }
    ]
  })
}
</script>

<style>

</style>