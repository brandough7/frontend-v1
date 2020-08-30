<template>
	<div>
		<b-carousel
      id="carousel-1"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
    >
      <b-carousel-slide
        caption="DEMO"
        img-src="https://picsum.photos/1024/480/?image=52"
      ></b-carousel-slide>

      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=54">
        <h1>Hello world!</h1>
      </b-carousel-slide>

      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=58"></b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            src="https://picsum.photos/1024/480/?image=55"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>
    </b-carousel>

    <div class="bg-light">
      <b-container class="py-5">
        <b-row>
          <b-col class="py-3" cols="12" md="4">
              <b-media tag="li">
                <template v-slot:aside>
                  <p class="icons"><b-icon icon="x-diamond-fill"></b-icon></p>
                </template>

                <h5 class="mt-0 mb-1 text-left">Graphic Design</h5>
                <p class="mb-0 text-left text">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt
                  a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.
                </p>
              </b-media>
          </b-col>

          <b-col class="py-3" cols="12" md="4">
            <b-media tag="li">
              <template v-slot:aside>
                <p class="icons"><b-icon class="icons" icon="bounding-box"></b-icon></p>
              </template>

              <h5 class="mt-0 mb-1 text-left">Web Development</h5>
              <p class="mb-0 text-left text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt
                a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.
              </p>
            </b-media>
          </b-col>

          <b-col class="py-3" cols="12" md="4">
            <b-media tag="li">
              <template v-slot:aside>
                <p class="icons"><b-icon class="icons" icon="bar-chart-line-fill"></b-icon></p>
              </template>

              <h5 class="mt-0 mb-1 text-left">Marketing</h5>
              <p class="mb-0 text-left text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt
                a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.
              </p>
            </b-media>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <b-container class="my-5">
      <h1 class="text-left">Our Expertise</h1>


      <b-row>
        <b-col class="p-4 expwrap" cols="12" md="4">
          <p class="text-right text prcnt">93%</p>
          <div class="progress barheight">
            <div class="progress-bar bg-secondary" role="progressbar" style="width: 93%" aria-valuenow="93" aria-valuemin="0" aria-valuemax="100"></div>
          </div>
          <p class="text-left">BRANDING</p>

          <p class="text-right text prcnt">80%</p>
          <div class="progress barheight">
            <div class="progress-bar bg-secondary" role="progressbar" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
          </div>
          <p class="text-left">DESIGN</p>

          <p class="text-right text prcnt">100%</p>
          <div class="progress barheight">
            <div class="progress-bar bg-secondary" role="progressbar" style="width: 100%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
          </div>
          <p class="text-left">DEVELOPMENT</p>
        </b-col>
        <b-col cols="12" md="8">
          <p class="py-3 text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.</p>
        </b-col>

      </b-row>
    </b-container>

    <b-container fluid>
      <b-row>
        <b-col class="p-0" cols="12" md="12" lg="6" order-md="2" order-lg="1">
          <b-img src="https://picsum.photos/1024/700/?image=41" min-height="500" alt="Responsive image" block fluid-grow></b-img>
        </b-col>
        <b-col cols="12" md="12" lg="6" order-md="1" order-lg="2">
              <h1 class="text-left p-3">Our Expertise</h1>
              <p class="p-3 text-left text">"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."</p>
        </b-col>
      </b-row>
    </b-container>
	</div>
</template>
<script>
	export default {

  }
</script>
<style scoped>
  .barheight {
    height: 3px;
  }

  .icons{
    font-size: 30px;
  }

  .prcnt{
    margin: 0 0 5px;
  }

  .expwrap p.text-left {
    margin-bottom: 0px !important
  }
</style>