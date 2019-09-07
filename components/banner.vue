<template>
  <div class="banner-section">
    <div class="container">
      <div class="row">
 <div class="col-md-offset-1 col-md-11 col-sm-12">
       <form action="">
         <div class="section-tab"> Personal Details </div>
         <section class="form-card ">
           <div class="form-group">
              <label for="firstName" class="control-label col-sm-2">*First Name:</label>
              <input type="text" placeholder="Enter First Name" name="firstName" required>
           </div>
        <div><label for="email"><b>Email</b></label>
            <input type="text" placeholder="Enter Email" name="email" required></div>
            <div>
              <label for="psw"><b>Password</b></label>
            <input type="password" placeholder="Enter Password" name="psw" required>
            </div>
         </section>

    <button type="submit" class="btn">Login</button>
       </form>
      </div>
      </div>

    </div>
  </div>
</template>
<style lang="scss">
.banner-section{
  // position: absolute;
  // right: 0;
  // margin: 20px;
  // max-width: 300px;
  // padding: 16px;
  // color: white;

    .section-tab {
    padding: 8px 25px 8px 30px;
    margin-right: 25px;
    background-color: #0a1a72;
    color: #fff;
    display: inline-block;
    position: relative;
    font-size: 18px;
    font-weight: 700;
    text-transform: capitalize;
}
.section-tab:after {
    content: '';
    position: absolute;
    top: 2px;
    right: -25px;
    border-right: 15px solid transparent;
    border-left: 10px solid #0a1a72;
    border-bottom: 23px solid #0a1a72;
    border-top: 18px solid transparent;
}
.form-card {
    padding: 20px;
    box-shadow: 0 0 10px 5px #e1e1e1;
    margin-bottom: 40px;
}
}
.animated {
  animation-duration: 2.5s;
  animation-fill-mode: both;
  animation-iteration-count: infinite;
}

@keyframes bounce {
  0%, 20%, 50%, 80%, 100% {transform: translateY(0);}
  40% {transform: translateY(-30px);}
  60% {transform: translateY(-15px);}
}
.bounce {
  animation-name: bounce;
}
</style>
