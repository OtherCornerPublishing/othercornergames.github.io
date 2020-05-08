<template>
  <div class="home container-fluid">
    <div class="bgs" id="bg-keyframes">er</div>
    <ColorSchemeExample />
  </div>
</template>


<script>
import ColorSchemeExample from "../components/ColorSchemeExample";
export default {
  name: "home",
  data() {
    return {};
  },
  computed: {},
  methods: {},
  components: { ColorSchemeExample }
};
</script>


<style lang="scss" scoped>
/* all the background scrolling stuff */
.bgs {
  z-index: -1; /* put it below the text */
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background: url("../assets/backgrounds/forest/ground_3.png") 0 0,
    url("../assets/backgrounds/forest/ground_2.png") 40% 0,
    url("../assets/backgrounds/forest/ground_1.png") 60% 0,
    url("../assets/backgrounds/forest/clouds_2.png") 60% 0,
    url("../assets/backgrounds/forest/rocks.png") 90% 0,
    url("../assets/backgrounds/forest/clouds_1.png") 80%, 0,
    url("../assets/backgrounds/forest/sky.png") 80% 0;
  -webkit-transition: left 300s linear;
  -moz-transition: left 300s linear;
  -o-transition: left 300s linear;
  transition: left 300s linear;
}

#bg-hover:hover,
#bg-target:target {
  left: -9999px;
}

#bg-keyframes {
  -webkit-animation: moving-images 400s linear infinite;
  -moz-animation: moving-images 400s linear infinite;
  -o-animation: moving-images 400s linear infinite;
  animation: moving-images 400s linear infinite;
}

@keyframes moving-images {
  0% {
    left: 0;
  }
  50% {
    left: -9999px;
  }
  100% {
    left: 0;
  }
}

@-moz-keyframes moving-images {
  0% {
    left: 0;
  }
  50% {
    left: -9999px;
  }
  100% {
    left: 0;
  }
}

@-webkit-keyframes moving-images {
  0% {
    left: 0;
  }
  50% {
    left: -9999px;
  }
  100% {
    left: 0;
  }
}

@-o-keyframes moving-images {
  0% {
    left: 0;
  }
  50% {
    left: -9999px;
  }
  100% {
    left: 0;
  }
}
</style>