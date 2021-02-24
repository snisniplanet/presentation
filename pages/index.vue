<template>
  <div>
    <div class="hero is-medium banner">
      <div class="hero-body container has-text-centered">
        <h1 class="title is-1 is-uppercase">SNISNI</h1>
      </div>
    </div>

    <div class="container section">
      <div class="columns is-vcentered">
        <div class="column">
          <div class="box is-square">
            <div class="content is-centered">
              <p class="title is-2">
                Projects made with <i class="bx bxs-heart"></i>
              </p>
            </div>
          </div>
        </div>

        <div class="column">
          <div class="columns is-vcentered">
            <div class="column">
              <div class="notification is-rounded is-square is-success">
                <div class="content is-centered">
                  <i class="bx bxl-vuejs bx-lg subtitle is-1"></i>
                </div>
              </div>
            </div>

            <div class="column">
              <div class="notification is-rounded is-square is-danger">
                <div class="content is-centered">
                  <i class="bx bxl-angular bx-lg subtitle is-1"></i>
                </div>
              </div>
            </div>
          </div>

          <div class="columns is-vcentered">
            <div class="column">
              <div class="notification is-rounded is-square is-dark">
                <div class="content is-centered">
                  <i class="bx bxl-sass bx-lg subtitle is-1"></i>
                </div>
              </div>
            </div>

            <div class="column">
              <div class="notification is-rounded is-square is-info">
                <div class="content is-centered">
                  <i class="bx bxl-react bx-lg subtitle is-1"></i>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="columns is-vcentered">
        <div class="column">
          <div class="notification is-rounded is-square is-warning">
            <div class="content is-centered">
              <i class="bx bxl-javascript bx-lg subtitle is-1"></i>
            </div>
          </div>
        </div>

        <div class="column">
          <div class="notification is-rounded is-square is-link">
            <div class="content is-centered">
              <i class="bx bxl-python bx-lg subtitle is-1"></i>
            </div>
          </div>
        </div>

        <div class="column">
          <div class="notification is-rounded is-square is-dark">
            <div class="content is-centered">
              <i class="bx bxl-dev-to bx-lg subtitle is-1"></i>
            </div>
          </div>
        </div>

        <div class="column">
          <div class="notification is-rounded is-square is-dark">
            <div class="content is-centered">
              <i class="bx bxl-github bx-lg subtitle is-1"></i>
            </div>
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
import ThePush from '@/components/prefabs/cards/ThePush'

export default {
  components: {
    ThePush,
  },
}
</script>

<style scoped lang="scss">
.banner {
  border-radius: 0 0 $radius-large $radius-large;
}
</style>
