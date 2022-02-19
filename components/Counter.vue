<template>
  <section>
    <h2>{{ title }}</h2>
    <!-- モジュールのcounter.jsから参照 -->
    counter: {{ $store.state.counter.counter }}
    <!-- ボタンがクリックされたとき、counter.jsのmutationsのcountUpを呼び出す -->
    <button v-on:click="$store.commit('counter/countUp')">+1</button>
    <button v-on:click="$store.commit('counter/reset')">reset</button>
  </section>
</template>

<script>
export default {
  data: function() {
    return {
      title: "Counter"
    };
  }
};
</script>
