<template>
  <div id="wrapper" class="" v-bind:class="{ 'nav-active': isActive }">
    <!-- header of the page -->
    <header id="header">
      <div class="brand-info">
        <div class="img-holder">
          <img src="./assets/img02.jpg" alt="image sdescription" />
        </div>
        <strong class="title">Betty Shop</strong>
      </div>
      <a href="#" @click="handleToggle" class="nav-opener"><span></span></a>
      <div class="nav-holder">
        <ul class="buttons-nav d-none d-lg-flex">
          <li><a href="#" class="btn btn-primary">Demo</a></li>
          <li><a href="#" class="btn btn-outline-dark">Sandbox</a></li>
          <li><a href="#" class="btn btn-outline-dark">Live</a></li>
        </ul>
        <ul class="top-nav">
          <li class="d-none d-md-block">
            <a href="#" class="btn btn-outline-primary"
              ><i class="icon-payment-link-add"></i
              ><span>Create Payment Link</span></a
            >
          </li>
          <li class="language jcf-select">
            <a href="#" class="dropdown-toggle" data-bs-toggle="dropdown">EN</a>
            <ul class="dropdown-menu">
              <li><a href="#">EN</a></li>
              <li><a href="#">DE</a></li>
              <li><a href="#">FR</a></li>
              <li><a href="#">JA</a></li>
              <li><a href="#">NL</a></li>
              <li><a href="#">RU</a></li>
            </ul>
          </li>
          <li class="settings">
            <a href="#" class="dropdown-toggle" data-bs-toggle="dropdown"
              ><i class="icon-settings"></i
            ></a>
            <ul class="dropdown-menu">
              <li>
                <a href="#"
                  ><i class="icon-user-circle-o"></i>Confirm Profile</a
                >
              </li>
              <li>
                <a href="#"><i class="icon-lock"></i>Change Password</a>
              </li>
              <li>
                <a href="#"><i class="icon-bank"></i>Bank Account</a>
              </li>
              <li>
                <a href="#"><i class="icon-bank"></i>Personal Account</a>
              </li>
              <li>
                <a href="#"><i class="icon-settings"></i>Webhooks</a>
              </li>
              <li>
                <a href="#"><i class="icon-group"></i>User Management</a>
              </li>
              <li>
                <a href="#"><i class="icon-file-text-o"></i>Tax Invoice</a>
              </li>
              <li>
                <a href="#"><i class="icon-sign-out"></i>Logout</a>
              </li>
            </ul>
          </li>
        </ul>
      </div>
    </header>
    <div class="content-wrapper has-sidebar">
      <!-- side navigation styles -->
      <nav class="side-nav">
        <ul class="nav">
          <li>
            <router-link to="/">
              <a @click="handleToggle"><i class="icon-dash"></i>Dashboard</a>
            </router-link>
          </li>
          <li>
            <router-link to="/activity"
              ><a @click="handleToggle"
                ><i class="icon-activity"></i>Activity</a
              ></router-link
            >
          </li>
          <li>
            <router-link to="/withdrawal">
              <a @click="handleToggle"
                ><i class="icon-wallet"></i>Withdrawal</a
              ></router-link
            >
          </li>
          <li>
            <router-link to="/auto-withdrawal">
              <a @click="handleToggle"
                ><i class="icon-clock"></i>Auto Withdraw</a
              >
            </router-link>
          </li>
        </ul>
        <ul class="buttons-nav d-lg-none">
          <li><a href="#" class="btn btn-primary">Demo</a></li>
          <li><a href="#" class="btn btn-outline-dark">Sandbox</a></li>
          <li><a href="#" class="btn btn-outline-dark">Live</a></li>
        </ul>
        <ul class="bottom-nav">
          <li>
            <a href="#tipInfo" data-bs-toggle="collapse"
              ><i class="icon-tips"></i>Tips</a
            >
            <div class="tip-info collapse" id="tipInfo">
              <a href="#tipInfo" class="btn-close" data-bs-toggle="collapse"
                ><i class="icon-cross"></i
              ></a>
              <strong class="heading">Easy withdrawal as follows</strong>
              <div class="box">
                <div class="icon-holder">
                  <img src="./assets/icon-book.png" alt="Icon" />
                </div>
                <p>
                  The merchant uploads Book Bank into the system, which must be
                  the account that you want to fund.
                </p>
              </div>
              <div class="box">
                <div class="icon-holder">
                  <img src="./assets/icon-box.png" alt="Icon" />
                </div>
                <p>Select the account and the amount you wish to withdraw.</p>
              </div>
              <a href="#" class="btn btn-outline-primary"
                >Next <i class="icon-chevron-right"></i
              ></a>
            </div>
          </li>
        </ul>
      </nav>
      <router-view> </router-view>
      <!-- contain main informative part of the site -->
      <footer id="footer">
        <div class="holder">
          <div class="row">
            <div class="col-12 col-md-6 d-md-flex">
              <div class="credit-cards">
                <img src="./assets/credit-cards.png" alt="credit cards" />
              </div>
              <ul class="fnav">
                <li><a href="#">Privacy policy</a></li>
              </ul>
            </div>
            <div class="col-12 col-md-6">
              <div class="copyright">
                <p>&copy; 2017 Copyright <a href="#">Money Space</a></p>
              </div>
            </div>
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: true,
    };
  },
  methods: {
    handleToggle() {
      this.isActive = !this.isActive;
    },
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
.bi bi-x-lg {
  font-size: 1.5rem;
}
</style>
