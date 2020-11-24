<template>
  <ProjectThumbnail>
    <div class="wrapper has-text-white">
      <div class="decoration">
        <i class="bx bx-git-branch text-icon"></i>
      </div>

      <div
        class="content-wrapper has-text-white is-flex is-align-items-flex-end"
      >
        <div class="py-4 px-2">
          <p class="is-block title is-2 has-text-white is-align-self-baseline">
            the push
          </p>
        </div>
      </div>
    </div>
  </ProjectThumbnail>
</template>

<script>
import ProjectThumbnail from '@/components/ProjectThumbnail'
export default {
  components: {
    ProjectThumbnail,
  },
  extends: ProjectThumbnail,
}
</script>

<style scoped lang="scss">
.wrapper {
  height: 100%;
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  position: relative;
  overflow: hidden !important;

  &:hover {
    .decoration {
      transform: rotateZ(0);
      left: 0;
      opacity: 1;

      .text-icon {
        font-size: 200px;
      }
    }

    .title {
      font-size: 35px;
    }
  }
}

.content-wrapper {
  height: 100%;
}

.decoration {
  position: absolute;

  opacity: 0;
  left: 100%;
  transform: rotateZ(90deg);
}

.text-icon {
  font-size: 160px;
}

.text-icon,
.decoration,
.title {
  transition: all 0.5s;
}
</style>
