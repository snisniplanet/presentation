<template>
  <div>
    <div class="hero is-large is-info">
      <div class="hero-body container">
        <h1 class="title is-1 is-uppercase">snisni</h1>
      </div>
    </div>

    <div>
      <div class="container section">
        <ProjectThumbnail />
      </div>
    </div>
  </div>
</template>

<script>
import ProjectThumbnail from '@/components/ProjectThumbnail'

export default {
  components: {
    ProjectThumbnail,
  },
}
</script>
