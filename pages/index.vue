<template>
  <div>
    <div class="hero is-medium">
      <div class="hero-body container has-text-centered">
        <h1 class="title is-1 is-uppercase">SNISNI</h1>
      </div>
    </div>

    <div
      class="section is-rounded"
      :style="
        'background-image: url(' +
        require('~/assets/img/backgrounds/white.jpg') +
        ')'
      "
    >
      <div class="container">
        <div class="columns is-vcentered">
          <div class="column">
            <GlassBox>
              <p class="title is-2">
                Projects made with <i class="bx bxs-heart"></i>
              </p>
            </GlassBox>
          </div>

          <div class="column">
            <div class="columns is-vcentered">
              <div class="column">
                <GlassBox
                  icon="bx bxl-vuejs bx-lg subtitle is-1"
                  type="success"
                />
              </div>

              <div class="column">
                <GlassBox
                  icon="bx bxl-angular bx-lg subtitle is-1"
                  type="danger"
                />
              </div>
            </div>

            <div class="columns is-vcentered">
              <div class="column">
                <GlassBox icon="bx bxl-sass bx-lg subtitle is-1" type="dark" />
              </div>

              <div class="column">
                <GlassBox icon="bx bxl-react bx-lg subtitle is-1" type="info" />
              </div>
            </div>
          </div>
        </div>

        <div class="columns is-vcentered">
          <div class="column">
            <GlassBox icon="bx bxl-python bx-lg subtitle is-1" type="link" />
          </div>

          <div class="column">
            <GlassBox
              icon="bx bxl-javascript bx-lg subtitle is-1"
              type="warning"
            />
          </div>

          <div class="column">
            <GlassBox icon="bx bxl-bootstrap bx-lg subtitle is-1" type="dark" />
          </div>

          <div class="column">
            <GlassBox icon="bx bxl-wordpress bx-lg subtitle is-1" type="link" />
          </div>
        </div>
      </div>
    </div>

    <div class="hero">
      <div class="hero-body container section">
        <div class="columns is-vcentered is-2">
          <div class="column is-one-quarter">
            <ThePush />
          </div>

          <div class="column">
            <h3 class="title is-3">Articles from open source developers.</h3>

            <p>
              <strong>The Push</strong> is an independent blog that focuses on
              the many quirks of working as an open source developer.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import GlassBox from '@/components/GlassBox'

import ThePush from '@/components/prefabs/cards/ThePush'

export default {
  components: {
    GlassBox,

    ThePush,
  },
}
</script>

<style scoped lang="scss">
.banner {
  border-radius: 0 0 $radius-large $radius-large;
}
</style>
