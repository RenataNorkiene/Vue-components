<template>
  <section>
    <h2>{{ name }}</h2>
    <h3>{{ age }}</h3>
  </section>
</template>

<script>
export default {
  name: "ActiveUser",
  props: {
    name: {
      type: String,
      required: true,
    },
    age: {
      type: Number,
      require: true,
    }
  }
};
</script>
