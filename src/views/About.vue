<template>
  <div id="wrapper" class="login-page">
    <!-- header of the page -->
    <header id="header">
      <div class="logo">
        <a href="#"
          ><img
            src="../assets/logo.png"
            width="151"
            height="28"
            alt="Money Space"
        /></a>
      </div>
      <a href="#" class="nav-opener"><span></span></a>
      <div class="nav-holder">
        <nav id="nav">
          <ul class="main-nav">
            <li><a href="#">Pricing &amp; Plans</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
        </nav>
      </div>
    </header>
    <div class="content-wrapper">
      <!-- contain main informative part of the site -->
      <main id="main">
        <section class="login-section">
          <ul class="signup-nav">
            <li><a href="#">Login</a></li>
            <li><a href="#" class="btn btn-primary">Signup</a></li>
          </ul>
          <div class="form-box">
            <form action="#" class="form">
              <h1 class="has-border-bottom">Login</h1>
              <div class="form-group">
                <input type="email" placeholder="Email" class="form-control" />
              </div>
              <div class="form-group">
                <input
                  type="password"
                  placeholder="Password"
                  class="form-control"
                />
              </div>
              <button type="submit" class="btn btn-lg btn-primary w-100">
                Login<i class="icon-arrow-right"></i>
              </button>
              <div class="text-center">
                <a href="#" class="btn-forgot">Forgot your password?</a>
              </div>
            </form>
          </div>
          <div class="info-box">
            <div class="text has-border-top">
              <h2 class="display-1">Better, Faster, Secure</h2>
              <p>Start accepting payments with Money Space</p>
            </div>
          </div>
        </section>
      </main>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.info-box {
  background-image: url(../assets/img01.jpg);
}
</style>
