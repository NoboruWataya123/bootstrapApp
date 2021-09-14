<template>
  <main id="main" class="has-sidebar">
    <section class="section">
      <header class="header">
        <h1>Auto Withdraw</h1>
      </header>
      <div class="card graph-box">
        <div class="card-body">
          <form action="#" class="auto-withdraw-form">
            <dl class="info">
              <dt>Auto Withdraw Status:</dt>
              <dd><span class="withdraw-status disable">Disable</span></dd>
              <dt>Description:</dt>
              <dd>Withdraw all day ()</dd>
              <dt>Date and Time Setting:</dt>
              <dd>05-04-2020 10:43</dd>
            </dl>
            <h3>Settings Usage</h3>
            <div class="form-group">
              <strong class="label">Auto Withdraw Status</strong>
              <ul class="radio-buttons">
                <li>
                  <label>
                    <input type="radio" name="withdrawStatus" checked />
                    <span>Disable</span>
                  </label>
                </li>
                <li>
                  <label>
                    <input type="radio" name="withdrawStatus" />
                    <span>Enable</span>
                  </label>
                </li>
              </ul>
            </div>
            <div class="form-group">
              <label for="bankName">Bank Name :</label>
              <input
                id="bankName"
                type="text"
                placeholder="Enter Bank Name"
                value="Bangkok Bank Public Company Limited (BBL)"
                class="form-control"
              />
            </div>
            <div class="form-group">
              <strong class="label">Choose Days</strong>
              <input type="text" class="tagsinput" />
            </div>
            <button type="submit" class="btn btn-primary btn-submit">
              Save
            </button>
          </form>
        </div>
      </div>
    </section>
  </main>
</template>
