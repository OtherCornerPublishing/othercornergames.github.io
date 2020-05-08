<template>
  <div class="color-scheme-example">
    <h1>To change your color scheme go to _variables.scss to change your color variables. You can edit the look of your default bootstrap classes by editing the class definitions in _overrides.scss. You can find these in assets inside of src.</h1>
    <button type="button" name id class="btn btn-primary btn-lg btn-block">primary</button>
    <button type="button" name id class="btn btn-secondary btn-lg btn-block">secondary</button>
    <button type="button" name id class="btn btn-success btn-lg btn-block">success</button>
    <button type="button" name id class="btn btn-danger btn-lg btn-block">danger</button>
    <button type="button" name id class="btn btn-warning btn-lg btn-block">warning</button>
    <button type="button" name id class="btn btn-info btn-lg btn-block">info</button>
    <button type="button" name id class="btn btn-dark btn-lg btn-block">dark</button>
    <button type="button" name id class="btn btn-light btn-lg btn-block">light</button>
  </div>
</template>


<script>
export default {
  name: "color-scheme-example",
  data() {
    return {};
  },
  computed: {},
  methods: {},
  components: {}
};
</script>


<style lang="scss" scoped>
</style>