<template>
  <section class="container">
    <div>
      <Counter></Counter>
      <hr />
      <Counter></Counter>
      <hr />
      <Counter></Counter>
      <hr />
    </div>
  </section>
</template>

<script>
// Counter.vueコンポーネントを使えるようにする記述
import Counter from "~/components/Counter.vue";
export default {
  components: {
    Counter
  }
};
</script>
