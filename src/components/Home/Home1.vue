<template>
  <div style="padding: 0!important;">
    <!-- <svg
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 1440 320"
      class="top-background"
    >
      <path
        fill="#0099ff"
        fill-opacity="1"
        d="M0,192L80,186.7C160,181,320,171,480,181.3C640,192,800,224,960,229.3C1120,235,1280,213,1360,202.7L1440,192L1440,0L1360,0C1280,0,1120,0,960,0C800,0,640,0,480,0C320,0,160,0,80,0L0,0Z"
      ></path>
    </svg> -->

      <v-row class="d-flex justify-center align-center">
      <v-col 
      xl="6"
      lg="6"
      md="12"
      data-aos="fade" 
      class="pot-rel d-flex flex-column justify-md-center justify-sm-center ">
        <img
          src="../../../public/Home/Robots/left/left.png"
          data-aos="fade-right"
          data-aos-duration="3000"
          class="img-fluid"
        >
      </v-col>

      <v-col 
      xl="6"
      lg="6"
      md="12"
      class="d-flex flex-column justify-md-center justify-sm-center container-fluid"
      id="right-content">
          <iframe
            src="https://www.youtube.com/embed/b6oTI_k6TFU"
            title="YouTube video player"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
            class="iframe-yt"
            data-aos="fade-left"
            data-aos-duration="3000"
          ></iframe>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      robots: [
        {
          id: 1,
          text: "roboBack",
          src: require("../../../public/Home/Robots/left/Asset4.png"),
          class: "roboBack",
          d_aos: "fade",
        },
        {
          id: 2,
          text: "roboFront",
          src: require("../../../public/Home/Robots/left/Asset3.png"),
          class: "roboFront",
          d_aos: "fade-right",
        },
        {
          id: 3,
          text: "Vector1",
          src: require("../../../public/Home/Robots/left/Vector.png"),
          class: "Vector1",
          d_aos: "fade",
        },
        {
          id: 4,
          text: "Vector2",
          src: require("../../../public/Home/Robots/left/Vector.png"),
          class: "Vector2",
          d_aos: "fade",
        },
        {
          id: 5,
          text: "Star",
          src: require("../../../public/Home/Robots/left/star.png"),
          class: "Star",
          d_aos: "fade",
        },
        {
          id: 6,
          text: "Wheel",
          src: require("../../../public/Home/Robots/left/Wheel.png"),
          class: "Wheel",
          d_aos: "fade",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>

.top-background {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 0;
  opacity: 0.5;
}

.bottom-background {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  z-index: 0;
  opacity: 0.5;
}

.pot-rel{
    position: relative;
}
.roboFront,
.roboBack,
.Vector1,
.Vector2,
.Star,
.Wheel {
  position: absolute;
}
.roboBack {
  left: 141px;
  top: 10px;
  z-index: 1;
}
.roboFront {
  left: 326px;
  top: 2px;
  z-index: 5;
}
.Vector1 {
  left: 220px;
  top: 226px;
  z-index: 6;
}
.Vector2 {
  left: 133px;
  top: 170px;
  z-index: 3;
}
.Star {
  left: 452px;
  top: -100px;
  z-index: 6;
}
.Wheel {
  left: 40px;
  top: 180px;
  z-index: 6;
}
.iframe-yt {
  width: 560px;
  height: 315px;
  // position: absolute;
  // top: 281px;
  border-radius: 2%;
}

#right-content{
  @media(max-width: 1260px)
  {
    padding: 0 250px;
  }
  @media(max-width: 631px){
    margin-top: 100px
  }  

  @media(max-width: 631px){
    margin-top: 80px;
  }
}
</style>