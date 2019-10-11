<template>
  <div class="container">
    <section class="section">
      <div class="columns is-multiline">
        <div class="column is-4" v-bind.key="product.id" v-for="product in products">
          <div class="card">
            <div class="card-image">
              <figure class="image is-4by3">
                <img :src="product.image" alt />
              </figure>
            </div>
            <div class="card-content">
              <div class="media-content">
                <p class="title is-4">${{product.price}}</p>
                <p class="sub-title is-6">{{product.name}}</p>
                <p>
                  <a class="button add-cart-btn">Add to cart</a>
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          id: 1,
          name: "silvergray",
          image:
            "https://www.kustomkit.com/colours/1200/KK109silvergrey_front.jpg",
          price: 50
        },
        {
          id: 2,
          name: "light blue",
          image:
            "https://www.kustomkit.com/colours/1200/KK109lightblue_front.jpg",
          price: 30
        },
        {
          id: 3,
          name: "leavme",
          image:
            "https://www.freedomdesign.com/wp-content/uploads/2018/03/image-1889.jpeg",
          price: 20
        },
        {
          id: 4,
          name: "midnightnavy",
          image:
            "http://www.kustomkit.com/colours/1200/KK105midnightnavy_front.jpg",
          price: 40
        },
        {
          id: 5,
          name: "carhartt",
          image:
            "https://www.thesportinglodge.co.uk/wp-content/uploads/2017/11/Carhartt-C-collage-Tshirt-white.jpg",
          price: 60
        },
        {
          id: 6,
          name: "Nike blue",
          image:
            "https://www.snkronline.com/media/catalog/product/cache/1/image/1200x1200/9df78eab33525d08d6e5fb8d27136e95/_/4/_40---46_1__2_14.jpg",
          price: 80
        },
        {
          id: 7,
          name: "vestis master",
          image:
            "https://www.ems.com/on/demandware.static/-/Sites-vestis-master-catalog/default/dw1152b8c2/product/images/2023/415/2023415/2023415_004_main.jpg",
          price: 50
        },
        {
          id: 8,
          name: "surplus",
          image:
            "https://armygross.se/images/zoom/surplus_division_black_camo_4b.jpg",
          price: 30
        },
        {
          id: 9,
          name: "jeans",
          image:
            "http://www.shoppersbd.com/media/catalog/product/cache/1/image/9df78eab33525d08d6e5fb8d27136e95/a/1/a1-1000x1000.jpg",
          price: 50
        }
      ]
    };
  }
};
</script>
