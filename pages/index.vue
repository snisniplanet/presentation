<template>
  <div>
    <div class="hero is-small banner is-dark">
      <div class="hero-body container has-text-centered">
        <h1 class="title is-1 is-uppercase">snisni</h1>
        <p class="subtitle is-5">
          Projects made with <i class="bx bxs-heart"></i>
        </p>
      </div>
    </div>

    <div class="container section">
      <div class="columns is-vcentered">
        <div class="column">
          <div class="box is-square">
            <div class="content is-centered">
              <p>BIG</p>
            </div>
          </div>
        </div>

        <div class="column">
          <div class="columns is-vcentered">
            <div class="column">
              <div class="notification is-rounded is-square is-success">
                <div class="content is-centered">
                  <p>1</p>
                </div>
              </div>
            </div>

            <div class="column">
              <div class="notification is-rounded is-square is-warning">
                <div class="content is-centered">
                  <p>2</p>
                </div>
              </div>
            </div>
          </div>

          <div class="columns is-vcentered">
            <div class="column">
              <div class="notification is-rounded is-square is-dark">
                <div class="content is-centered">
                  <p>3</p>
                </div>
              </div>
            </div>

            <div class="column">
              <div class="notification is-rounded is-square is-info">
                <div class="content is-centered">
                  <p>4</p>
                </div>
              </div>
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
