<template>
  <nav class="navbar navbar-expand-lg navbar-light nav-main">
    <a class="navbar-brand" href="#">SGCP</a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto topnav">
        <li class="nav-item active">
          <a class="nav-link" href="#"
            >Inicio <span class="sr-only">(current)</span></a
          >
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Productos</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Clientes</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Salir</a>
        </li>
      
      </ul>
    </div>

    <!-- The Modal -->
    <div class="modal" id="myModal">
      <div class="modal-dialog">
        <div class="modal-content">
          <!-- Modal Header -->
          <div class="modal-header">
            <h4 class="modal-title">Customer Sign In</h4>
            <button type="button" class="close" data-dismiss="modal">×</button>
          </div>

          <!-- Modal body -->
          <div class="modal-body">
            <form>
              <label class="sr-only" for="usrname">Username</label>
              <div class="input-group mb-3">
                <div class="input-group-prepend">
                  <span class="input-group-text" id="basic-addon1"
                    ><i class="fa fa-user"></i
                  ></span>
                </div>
                <input
                  type="text"
                  class="form-control"
                  placeholder="Username"
                  aria-label="Username"
                  aria-describedby="basic-addon1"
                />
              </div>

              <label class="sr-only" for="Password">Name</label>
              <div class="input-group mb-2">
                <div class="input-group-prepend">
                  <span class="input-group-text" id="basic-addon2"
                    ><i class="fa fa-key"></i
                  ></span>
                </div>
                <input
                  id="Password"
                  type="password"
                  class="form-control"
                  placeholder="Password"
                  aria-label="Password"
                  aria-describedby="basic-addon2"
                />
              </div>
            </form>
          </div>

    
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
  .topnav a {
    border-bottom: 2px solid transparent;
  }
  .topnav a:hover {
    border-bottom: 2px solid #fe6b47;;
  }
  .nav-main{ 
    background-color: #3c8dbc;
    color:white;
    padding: 2px 20px;
  }
  .navbar-light .navbar-nav .nav-link{
    color:whitesmoke;
  }
  .navbar-light .navbar-brand {
    color:whitesmoke;
  }

</style>

