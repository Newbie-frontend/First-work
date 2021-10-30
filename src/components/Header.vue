<template>
  <div>
    <b-navbar toggleable="md" type="dark" variant="success">
      <b-navbar-brand href="#" id="rang2">Question & Answer</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#" disabled
            >Question {{ numTotal }}/10</b-nav-item
          >
           <b-nav-item href="#" disabled
            >Correct Answers : {{ numCorrect }}</b-nav-item
          >
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  props: ["numTotal", "numCorrect"],
};
</script>
<style scoped>
.navbar {
  padding-left: 1rem;
}
.b-narbar-item{
  color: red;
}
</style>
