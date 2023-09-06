<template>
    <figure>
      <img :src="img"
           :alt="alt">
      <figcaption>{{text}}</figcaption>
    </figure>
</template>

<script lang="ts">
export default {
  props: ["text","alt", "img"]
}
</script>

<style>
figure {
  float: right;
  width: 30%;
  text-align: center;
  font-style: italic;
  font-size: smaller;
  text-indent: 0;
  border: thin silver solid;
  margin: 0.5em;
  padding: 0.5em;
  overflow: hidden;
}
img {
  width: 100%;
  margin: 0;
}

@media (min-width: 320px) and (max-width: 500px) {
  figure {
    width: 40%;
  }
}
</style>