<template>
  <div>
    <div id="searchdiv">
      <div id="searchfilter">
        <div class="dropdown">
          <button
            class="btn btn-dark dropdown-toggle"
            type="button"
            id="dropdownMenuButton"
            data-coreui-toggle="dropdown"
            aria-expanded="false"
          >
            Filter
          </button>
          <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </div>
      </div>
      <input
        class="form-control search"
        type="text"
        placeholder="search for user"
        aria-label=".form-control-lg example"
      />
      <button type="button" class="btn searchbtn">Search</button>
    </div>
  </div>
</template>

<style scoped>
#searchdiv {
  display: flex;
  width: 100%;
  height: auto;
  text-align: center;
  justify-content: center;
}
.search {
  width: 60%;
  height: 50px;
  margin-left: 10px;
  margin-right: 10px;
}
.searchbtn {
  width: 10%;
  height: 50px;
  background-color: orange;
}

.searchfilter {
  width: 10%;
  height: 50px;
  background-color: white;
}
</style>