<template>
  <div class="container">
    <div class="column">
      <div class="text-left main-form-section mx-5">
        <b-form name="form">
          <!-- Personal Details -->
          <div class="card inception">
            <div class="tab-heading inception">
              <h3 class="text">Personal Details</h3>
            </div>
                 <!-- first name -->
            <b-form-group label="First Name:" label-for="firstName">
              <b-form-input
                id="firstName"
                type="text"
                required
                placeholder="Enter First Name"
              ></b-form-input>
              <!-- <div
                v-if="$v.form.firstName.$error && !$v.form.firstName.required"
                class="error-txt"
              >
                first name is required
              </div> -->
            </b-form-group>
          </div>
          <!-- Personal Details End-->
          <!-- School Details -->
          <div class="card inception">
            <div class="tab-heading inception">
              <h3 class="text">School Details</h3>
            </div>
                 <!-- first name -->
            <b-form-group label="First Name:" label-for="firstName">
              <b-form-input
                id="firstName"
                type="text"
                required
                placeholder="Enter First Name"
              ></b-form-input>
              <!-- <div
                v-if="$v.form.firstName.$error && !$v.form.firstName.required"
                class="error-txt"
              >
                first name is required
              </div> -->
            </b-form-group>
          </div>
          <!-- School Details End-->
        </b-form>
      </div>
    </div>
  </div>
</template>
<script>
export default {

}
</script>

<style lang="scss">
@import '~assets/scss/main.scss';
.error-txt {
  color: red;
}

.main-form-section {
  color: black !important;
}
.column{
  .main-form-section{
    .card {
      font-size: 1.1rem;
      font-weight: 400;
      margin: 7rem 0;
      padding: 0 0 1rem 0;
      width: 100%;
      box-shadow: 0.3rem 1.3rem 2rem 2px rgba(56, 65, 56, 0.41);
      background-color: $light-white;
      p {
        margin: 0 1rem 1rem 1rem;
        color: #333;
        font-size: 1.2rem;
        font-weight: 300;
        &:last-child {
          margin-bottom: 0;
        }
      }
      .tab-heading {
        font-family: "Open Sans";
        font-weight: 600;
        border-top: 0.3rem solid #03a9f4;
        margin: 0 0 1rem 0;
        color: $fg-color;
        background-color: transparent;
        display: flex;
        justify-content: flex-start;
        position: relative;
        &:before,
        &:after {
          content: "";
          display: block;
          width: 1rem;
          height: 1rem;
          background-color: transparent;
          background-image: $inverted-corner;
          background-size: contain;
          background-repeat: no-repeat;
          margin-top: -1px;
        }
        &:before {
          margin: 0 0 0 1rem;
        }
        &:after {
          transform: rotateZ(270deg);
        }
        .text {
          display: block;
          background-color: $heading-bg-color;
          padding: 0.2rem 1rem 0.5rem;
          border-color: $heading-bg-color;
          border-bottom-right-radius: 1rem;
          border-bottom-left-radius: 1rem;
          position: relative;
          box-shadow: 0.1rem 0.4rem 0.5rem -3px rgba(0, 0, 0, 0.56);
          margin-top: -1px;
          &:before,
          &:after {
            content: "";
            display: block;
            position: absolute;
            z-index: -1;
          }
          &:before {
            bottom: 0.4rem;
            right: 0.9rem;
            width: 75%;
            height: 1.6rem;
            box-shadow: 0.8rem 0.4rem 1rem -0.9px rgba(0, 0, 0, 0.76);
            transform: rotate(6deg);
            border-bottom-right-radius: 1rem;
          }
          &:after {
            top: -0.7rem;
            right: 0.65rem;
            transform: rotate(20deg);
            content: "(";
            color: transparent;
            font-size: 1.7rem;
            font-weight: 900;
            text-shadow: 1rem 0 0.4rem black;
          }
        }
      }
    }
  }
}
</style>

