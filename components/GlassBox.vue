<template>
  <div class="box is-glass is-rounded is-square" :class="'is-' + type">
    <div class="content is-centered">
      <i :class="[icon, 'has-text-' + type]"></i>

      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    icon: {
      type: String,
    },
    type: {
      type: String,
      default: '',
    },
  },
}
</script>

<style></style>
