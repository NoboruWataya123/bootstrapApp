<template>
  <main id="main" class="has-sidebar">
    <section class="section dashboard-section">
      <header class="header">
        <h1>Withdraw</h1>
      </header>
      <div class="card withdraw-steps">
        <div class="card-body">
          <ul class="step-nav-list">
            <li class="active"><strong>Withdraw Funds</strong></li>
            <li><strong>Confirm</strong></li>
          </ul>
          <div class="steps">
            <div class="step active">
              <div class="step-body">
                <div class="info-box">
                  <div class="price-info">
                    <strong class="heading">Ledger Balance:</strong>
                    <strong class="price"
                      ><span class="amount">14,429.06</span>Baht</strong
                    >
                  </div>
                  <div class="info-text">
                    <div class="text">
                      <p>
                        Withdrawal money will normally be received in your bank
                        account within 2-3 business days.
                      </p>
                    </div>
                  </div>
                </div>
                <div class="form-group">
                  <label for="bankName">Bank Name:</label>
                  <select id="bankName" class="form-select">
                    <option value="Select Your Bank">Select Your Bank</option>
                    <option
                      value="Bank of Ayudhya Public Company Limited (BAY)"
                    >
                      Bank of Ayudhya Public Company Limited (BAY)
                    </option>
                    <option
                      value="Bank of Ayudhya Public Company Limited (BAY)"
                    >
                      Bank of Ayudhya Public Company Limited (BAY)
                    </option>
                  </select>
                </div>
                <div class="form-group">
                  <label for="amount">Amount</label>
                  <div class="input-holder">
                    <i class="icon-baht"></i>
                    <input id="amount" type="text" class="form-control" />
                  </div>
                  <span class="note"
                    ><span class="text-primary">*</span>if your withdraw amount
                    is between 100 to 29.999.99 you will have a fee 15
                    baht.</span
                  >
                </div>
              </div>
              <div class="step-footer">
                <ul class="buttons-inline-list">
                  <li>
                    <button type="button" class="btn btn-primary btn-next">
                      Next <i class="icon-arrow-right"></i>
                    </button>
                  </li>
                </ul>
              </div>
            </div>
            <div class="step">
              <div class="step-body">
                <ul class="detail-list">
                  <li>
                    <strong class="heading">Withdraw Amount:</strong>
                    <strong class="value"
                      ><span class="amount">220.00</span> baht</strong
                    >
                  </li>
                  <li>
                    <strong class="heading">Withdraw fee:</strong>
                    <strong class="value"
                      ><span class="amount">15.00</span> baht</strong
                    >
                  </li>
                  <li>
                    <strong class="heading">Withdraw fee:</strong>
                    <strong class="value"
                      ><span class="amount">15.00</span> baht</strong
                    >
                  </li>
                </ul>
              </div>
              <div class="step-footer">
                <div class="row align-items-center">
                  <div class="col-12 col-md-6">
                    <strong class="note"
                      >Kindly verify the amount you have entered.</strong
                    >
                  </div>
                  <div class="col-12 col-md-6">
                    <ul class="buttons-inline-list">
                      <li>
                        <button type="button" class="btn popup-close">
                          Cancel
                        </button>
                      </li>
                      <li>
                        <button type="button" class="btn btn-primary">
                          Save
                        </button>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>
