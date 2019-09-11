<template>
  <div>
    <div class="main-background">
      <!--  -->
      <Header></Header>
      <AllForms></AllForms>
      <!--  -->
    </div>
  </div>
</template>
<script>
import Header from "~/components/header.vue";
import AllForms from "~/components/form.vue";
export default {
  components: {
    Header,
    AllForms
  }
};
</script>
<style lang="scss">
.main-background {
      background-image: linear-gradient(90deg,rgba(48,172,177,.8),rgba(115,173,39,.8)),
    url("~@/assets/Images/office-space.jpg");
/*
    background-image: linear-gradient(90deg,rgba(48,172,177,.8),rgba(115,173,39,.8)),
    url("~@/assets/Images/girl.jpg"); */
  height: 100vh;
  position: fixed;
  width: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  overflow-y: scroll;
}
</style>
