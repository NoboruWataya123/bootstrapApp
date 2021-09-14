<template>
  <!-- contain main informative part of the site -->
  <main id="main" class="has-sidebar">
    <section class="section">
      <header class="header">
        <h1>Activity</h1>
        <a href="#" class="btn btn-primary"
          ><i class="icon-microsoftexcel"></i> Download Excel File</a
        >
      </header>
      <form action="#" class="filter-form card">
        <div class="holder">
          <div class="datepickers">
            <div class="row">
              <div class="col-6">
                <div class="form-group">
                  <label for="from-date">From</label>
                  <div class="input-holder">
                    <input
                      id="from-date"
                      type="text"
                      class="form-control datepicker"
                      value="20/12/2020"
                      readonly
                    />
                    <i class="icon-calendar"></i>
                  </div>
                </div>
              </div>
              <div class="col-6">
                <div class="form-group">
                  <label for="to-date">To</label>
                  <div class="input-holder">
                    <input
                      id="to-date"
                      type="text"
                      class="form-control datepicker"
                      value="20/12/2020"
                      readonly
                    />
                    <i class="icon-calendar"></i>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="form-group filter-type">
            <strong class="label">Transaction Type</strong>
            <div class="jcf-dropdown">
              <a href="#" class="jcf-opener">Filter</a>
              <div class="jcf-dropdown-menu">
                <ul class="custom-checkbox">
                  <li>
                    <label
                      ><input
                        type="checkbox"
                        id="creditCard"
                        value="Credit Card"
                      /><span>Credit Card</span></label
                    >
                  </li>
                  <li>
                    <label
                      ><input
                        type="checkbox"
                        id="qrCode"
                        value="QR Code"
                      /><span>QR Code</span></label
                    >
                  </li>
                  <li>
                    <label
                      ><input
                        type="checkbox"
                        id="installPayments"
                        value="Install payments"
                      /><span>Install payments</span></label
                    >
                  </li>
                  <li>
                    <label
                      ><input
                        type="checkbox"
                        id="krungthaiBank"
                        value="Krungthai Bank"
                      /><span>Krungthai Bank</span></label
                    >
                  </li>
                  <li>
                    <label
                      ><input
                        type="checkbox"
                        id="krungsriBank"
                        value="Krungsri Bank"
                      /><span>Krungsri Bank</span></label
                    >
                  </li>
                  <li>
                    <label
                      ><input
                        type="checkbox"
                        id="firstChoice"
                        value="First Choice"
                      /><span>First Choice</span></label
                    >
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <div class="form-group transaction-type">
            <strong class="label">Transaction Type</strong>
            <ul class="custom-checkbox">
              <li>
                <label
                  ><input type="checkbox" id="showWithdrawal" /><span
                    >Show Withdrawal</span
                  ></label
                >
              </li>
              <li>
                <label
                  ><input type="checkbox" id="showRefunds" /><span
                    >Show Refunds</span
                  ></label
                >
              </li>
            </ul>
          </div>
        </div>
        <ul class="tags"></ul>
        <div class="btn-holder">
          <button type="submit" class="btn btn-primary btn-search">
            <i class="icon-search"></i> Search
          </button>
        </div>
      </form>
      <div class="card">
        <div class="card-body pb-1">
          <div class="activity-table-holder">
            <table class="table activity-table">
              <thead>
                <tr>
                  <th>Date</th>
                  <th>Transaction ID</th>
                  <th>Status</th>
                  <th>Branch</th>
                  <th>Currency</th>
                  <th class="price-cell">
                    <strong class="theading">Debit</strong>
                    <div class="amount-detail credit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                    </div>
                  </th>
                  <th class="price-cell">
                    <strong class="theading">Credit</strong>
                    <div class="amount-detail credit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                    </div>
                  </th>
                  <th>Action</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td data-title="Date">
                    <span class="tran-id">MSTRF18000000090030</span>
                    <time datetime="2020-12-20">02/02/2020</time>
                    <span class="time">20:30</span>
                  </td>
                  <td data-title="Transaction ID">
                    <span class="tran-id">MSTRF18000000090030</span>
                  </td>
                  <td data-title="Status">
                    <span class="status online"></span>
                  </td>
                  <td data-title="Branch">Branch</td>
                  <td data-title="Currency">THB</td>
                  <td data-title="Debit" class="price-cell">
                    <div class="amount-detail debit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                      <div class="values">
                        <span class="cell">90.3</span>
                        <span class="cell">10.2</span>
                        <span class="cell">30</span>
                        <span class="cell">50</span>
                      </div>
                    </div>
                  </td>
                  <td data-title="Credit" class="price-cell">
                    <div class="amount-detail credit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                      <div class="values">
                        <span class="cell">90.3</span>
                        <span class="cell">10.2</span>
                        <span class="cell">30</span>
                        <span class="cell">50</span>
                      </div>
                    </div>
                  </td>
                  <td class="action">
                    <div class="dropdown">
                      <a
                        href="#"
                        class="dropdown-toggle"
                        data-bs-toggle="dropdown"
                        ><i class="icon-dots"></i
                      ></a>
                      <ul class="dropdown-menu">
                        <li>
                          <a
                            href="#transactionDetails"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Details</a
                          >
                        </li>
                        <li>
                          <a
                            href="#popupVoid"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Void</a
                          >
                        </li>
                        <li>
                          <a
                            href="#popupRefund"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Refund</a
                          >
                        </li>
                      </ul>
                    </div>
                  </td>
                </tr>
                <tr>
                  <td data-title="Date">
                    <span class="tran-id">MSTRF18000000090044</span>
                    <time datetime="2020-12-20">02/02/2020</time>
                    <span class="time">20:30</span>
                  </td>
                  <td data-title="Transaction ID">
                    <span class="tran-id">MSTRF18000000090044</span>
                  </td>
                  <td data-title="Status">
                    <span class="status online"></span>
                  </td>
                  <td data-title="Branch">Branch</td>
                  <td data-title="Currency">THB</td>
                  <td data-title="Debit" class="price-cell">
                    <div class="amount-detail debit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                      <div class="values">
                        <span class="cell">90.3</span>
                        <span class="cell">10.2</span>
                        <span class="cell">30</span>
                        <span class="cell">50</span>
                      </div>
                    </div>
                  </td>
                  <td data-title="Credit" class="price-cell">
                    <div class="amount-detail credit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                      <div class="values">
                        <span class="cell">90.3</span>
                        <span class="cell">10.2</span>
                        <span class="cell">30</span>
                        <span class="cell">50</span>
                      </div>
                    </div>
                  </td>
                  <td class="action">
                    <div class="dropdown">
                      <a
                        href="#"
                        class="dropdown-toggle"
                        data-bs-toggle="dropdown"
                        ><i class="icon-dots"></i
                      ></a>
                      <ul class="dropdown-menu">
                        <li>
                          <a
                            href="#transactionDetails"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Details</a
                          >
                        </li>
                        <li>
                          <a
                            href="#popupVoid"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Void</a
                          >
                        </li>
                        <li>
                          <a
                            href="#popupRefund"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Refund</a
                          >
                        </li>
                      </ul>
                    </div>
                  </td>
                </tr>
                <tr>
                  <td data-title="Date">
                    <span class="tran-id">MSTRF18000000090055</span>
                    <time datetime="2020-12-20">02/02/2020</time>
                    <span class="time">20:30</span>
                  </td>
                  <td data-title="Transaction ID">
                    <span class="tran-id">MSTRF18000000090055</span>
                  </td>
                  <td data-title="Status">
                    <span class="status online"></span>
                  </td>
                  <td data-title="Branch">Branch</td>
                  <td data-title="Currency">THB</td>
                  <td data-title="Debit" class="price-cell">
                    <div class="amount-detail debit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                      <div class="values">
                        <span class="cell">90.3</span>
                        <span class="cell">10.2</span>
                        <span class="cell">30</span>
                        <span class="cell">50</span>
                      </div>
                    </div>
                  </td>
                  <td data-title="Credit" class="price-cell">
                    <div class="amount-detail credit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                      <div class="values">
                        <span class="cell">90.3</span>
                        <span class="cell">10.2</span>
                        <span class="cell">30</span>
                        <span class="cell">50</span>
                      </div>
                    </div>
                  </td>
                  <td class="action">
                    <div class="dropdown">
                      <a
                        href="#"
                        class="dropdown-toggle"
                        data-bs-toggle="dropdown"
                        ><i class="icon-dots"></i
                      ></a>
                      <ul class="dropdown-menu">
                        <li>
                          <a
                            href="#transactionDetails"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Details</a
                          >
                        </li>
                        <li>
                          <a
                            href="#popupVoid"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Void</a
                          >
                        </li>
                        <li>
                          <a
                            href="#popupRefund"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Refund</a
                          >
                        </li>
                      </ul>
                    </div>
                  </td>
                </tr>
                <tr>
                  <td data-title="Date">
                    <span class="tran-id">MSTRF18000000090077</span>
                    <time datetime="2020-12-20">02/02/2020</time>
                    <span class="time">20:30</span>
                  </td>
                  <td data-title="Transaction ID">
                    <span class="tran-id">MSTRF18000000090077</span>
                  </td>
                  <td data-title="Status">
                    <span class="status online"></span>
                  </td>
                  <td data-title="Branch">Branch</td>
                  <td data-title="Currency">THB</td>
                  <td data-title="Debit" class="price-cell">
                    <div class="amount-detail debit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                      <div class="values">
                        <span class="cell">90.3</span>
                        <span class="cell">10.2</span>
                        <span class="cell">30</span>
                        <span class="cell">50</span>
                      </div>
                    </div>
                  </td>
                  <td data-title="Credit" class="price-cell">
                    <div class="amount-detail credit">
                      <div class="haeding-bar">
                        <strong class="cell">Amount</strong>
                        <strong class="cell">Fee</strong>
                        <strong class="cell">Tax</strong>
                        <strong class="cell">Net Amount</strong>
                      </div>
                      <div class="values">
                        <span class="cell">90.3</span>
                        <span class="cell">10.2</span>
                        <span class="cell">30</span>
                        <span class="cell">50</span>
                      </div>
                    </div>
                  </td>
                  <td class="action">
                    <div class="dropdown">
                      <a
                        href="#"
                        class="dropdown-toggle"
                        data-bs-toggle="dropdown"
                        ><i class="icon-dots"></i
                      ></a>
                      <ul class="dropdown-menu">
                        <li>
                          <a
                            href="#transactionDetails"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Details</a
                          >
                        </li>
                        <li>
                          <a
                            href="#popupVoid"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Void</a
                          >
                        </li>
                        <li>
                          <a
                            href="#popupRefund"
                            class="
                              btn btn-sm btn-outline-primary
                              card-popup-opener
                            "
                            >Refund</a
                          >
                        </li>
                      </ul>
                    </div>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </section>
  </main>
  <!-- card popup -->
</template>
