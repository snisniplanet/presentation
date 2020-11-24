<template>
  <div>
    <div class="box">
      <div :style="boxStyling" class="image"></div>

      <div class="overlay">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<style scoped>
.box {
  width: 200px;
  height: 300px;
  position: relative;
}

.image {
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}

.overlay,
.image {
  position: absolute;
  inset: 0;
}

.box,
.image,
.overlay {
  border-radius: 10px;
}
</style>

<script>
export default {
  props: {
    image: {
      type: String,
      default: require('~/assets/img/thumbnails/lines.jpg'),
    },
  },
  data() {
    return {
      boxStyling: `background-image: url(${this.image})`,
    }
  },
}
</script>
