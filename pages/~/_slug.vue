<template>
  <div>
    <div class="hero is-dark is-medium">
      <div class="hero-body">
        <div class="container">
          <h1 class="title is-1">{{ doc.title }}</h1>
          <p class="subtitle">{{ doc.description }}</p>
        </div>
      </div>
    </div>

    <div class="section container">
      <nuxt-content :document="doc" />
    </div>
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const doc = await $content(params.slug || 'hello').fetch()

    return { doc }
  },
  head() {
    return {
      title: this.doc.title,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: this.doc.description,
        },
      ],
    }
  },
}
</script>
