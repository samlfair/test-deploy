<template>
  <div>
    <prismic-link :field="slice.primary.link">{{
      slice.primary.link.slug
    }}</prismic-link>
  </div>
</template>

<script>
export default {
  name: "Link",
  props: {
    slice: Object
  }
};
</script>
