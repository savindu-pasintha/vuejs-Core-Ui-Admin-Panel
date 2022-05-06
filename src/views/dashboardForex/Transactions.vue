<template>
  <div>
    <div>
      <CBadge color="primary" class="p-2 m-2"> Transactions</CBadge>
      <CBadge color="success" class="p-2 m-2"> Complaince</CBadge>
      <CBadge color="warning" class="p-2 m-2"> KYC</CBadge>
      <CBadge color="danger" class="p-2 m-2"> Treasury</CBadge>
    </div>
    <br />
    <div id="forexdiv">
      <div class="forex">
        <h class="Black text-dark"> Daily Forex</h>
      </div>
      <br />
      <div class="dropdown forex">
        <button
          class="btn btn-warning dropdown-toggle"
          type="button"
          id="dropdownMenuButton"
          data-coreui-toggle="dropdown"
          aria-expanded="false"
        >
          Malayasia
        </button>
        <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
          <li><a class="dropdown-item" href="#">Action</a></li>
          <li><a class="dropdown-item" href="#">Another action</a></li>
          <li><a class="dropdown-item" href="#">Something else here</a></li>
        </ul>
      </div>
      <div class="dropdown forex">Add date here</div>
    </div>
  </div>
</template>

<style>
#forexdiv {
  display: flex;
  width: 100%;
  height: auto;
}
.forex {
  width: 150px;
  height: 50px;
}
</style>