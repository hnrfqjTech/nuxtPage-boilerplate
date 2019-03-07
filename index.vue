<template>
  <div class="page-index">
    姓名：{{name}}，年龄：{{age}}
  </div>
</template>

<script>
export default {
  name: '',
  mixins: [],
  components: {},
  data() {
    return {
    };
  },
  // middleware: 'test',
  // validate({ params, query, store }) {
  //   return true;
  // },
  async asyncData({ $axios }) {
    return { name: 'demo' }
  },
  async fetch ({ store, params }) {
    // let { data } = await axios.get('http://my-api/stars')
    // store.commit('setStars', data);
  },
  beforeMount() {
  },
  computed: {
    age() {
      return 18;
    }
  },
  mounted() {
  },
  // head () {
  //   return {
  //     title: '标题-demo'
  //   };
  // },
  destroyed() {
  },
  methods: {
  },
};
</script>

<style lang="scss" scoped>
.page-index {

}
</style>
