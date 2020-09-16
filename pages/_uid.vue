<template>
  <div class="container">
    {{ $prismic.asText(page.data.title) }}
  </div>
</template>

<script>
export default {
  name: "Home",
  async asyncData({ $prismic, params, error }) {
    try {
      const page = await $prismic.api.getByUID("page", params.uid);
      return { page };
    } catch (e) {
      error({ statsCode: 404, message: "Page not found" });
    }
  }
};
</script>

<style></style>
