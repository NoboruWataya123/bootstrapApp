<template>
  <main id="main" class="has-sidebar">
    <section class="section dashboard-section">
      <header class="header">
        <h1>Dashboard</h1>
        <strong class="acc-id">Account ID: B2018061028</strong>
      </header>
      <div class="row">
        <div class="col-12 col-md-6 d-md-flex">
          <div class="card w-100">
            <div class="card-body">
              <strong class="heading">Total balance</strong>
              <div class="row align-items-center">
                <div class="col-sm-auto flex-grow-1">
                  <strong class="number-heading h1">10454.29</strong>
                </div>
                <div class="col-sm-auto flex-shrink-0"></div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 d-md-flex">
          <div class="card w-100">
            <div class="card-body">
              <strong class="heading">Withdrawable balance</strong>
              <div class="row align-items-center">
                <div class="col-6 mb-2 mb-md-0">
                  <strong class="number-heading h1">9124.69</strong>
                </div>
                <div class="col-6 text-right">
                  <a href="#" class="btn btn-primary"
                    ><i class="icon-withdraw"></i>Withdraw</a
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="card graph-box">
        <div class="card-body">
          <div class="row mb-3">
            <div class="col-7 col-md-4">
              <strong class="heading">OVERVIEW</strong>
            </div>
            <div class="col-5 col-md-8 d-flex justify-content-end">
              <div class="tab-select jcf-select">
                <a href="#" class="dropdown-toggle" data-bs-toggle="dropdown"
                  >Today</a
                >
                <ul
                  class="dropdown-menu nav nav-tabs"
                  id="myTab"
                  role="tablist"
                >
                  <li class="nav-item">
                    <a
                      class="nav-link active"
                      data-bs-toggle="tab"
                      href="#todayOverview"
                      role="tab"
                      >Today</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      class="nav-link"
                      data-bs-toggle="tab"
                      href="#weeklyOverview"
                      role="tab"
                      >This Week</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      class="nav-link"
                      data-bs-toggle="tab"
                      href="#monthlyOverview"
                      role="tab"
                      >This Month</a
                    >
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <div class="tab-content" id="myTabContent">
            <div
              class="tab-pane fade show active"
              id="todayOverview"
              role="tabpanel"
            >
              <div class="graph-holder">
                <img src="../assets/graph.png" alt="graph" />
              </div>
            </div>
            <div class="tab-pane fade" id="weeklyOverview" role="tabpanel">
              <div class="graph-holder">
                <img src="../assets/graph.png" alt="graph" />
              </div>
            </div>
            <div class="tab-pane fade" id="monthlyOverview" role="tabpanel">
              <div class="graph-holder">
                <img src="../assets/graph.png" alt="graph" />
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="card links-card">
        <div class="row">
          <div class="col-12 col-md-6">
            <h2 class="has-border-top">Create <br />Payment Link</h2>
            <a href="#" class="btn btn-primary"
              ><i class="icon-link"></i>Create Payment Link</a
            >
          </div>
          <div class="col-12 col-md-6">
            <h2 class="has-border-top-secondary">See Link <br />History</h2>
            <a href="#" class="btn btn-secondary"
              ><i class="icon-linkhistory"></i>Link History</a
            >
          </div>
        </div>
      </div>
    </section>
  </main>
</template>
