<template>
  <div>
    <div class="container-fluid log-in-bg">
      <div class="container center-div">
        <div class="container logo">
          <div class="row justify-content-center">
            <div class="col-12">
              <img src="../assets/logomiapplogin.svg" class="logo" />
            </div>
          </div>
        </div>
        <div class="row justify-content-center">
          <div class="col-lg-6 col-md-7 col-sm-12 col-xs-12">
            <div class="card">
              <div class="card-body">
                <form>
                  <div class="row justify-content-center">
                    <h1 class="login-title">Login</h1>
                    <div class="col-12">
                      <div class="row justify-contain-center">
                        <div class="col-1">
                          <i class="icon fas fa-user"></i>
                        </div>
                        <div class="col-11">
                          <input class="email" type="email" placeholder="Email" />
                        </div>
                      </div>
                    </div>
                    <div class="col-12">
                      <div class="row justify-contain-center">
                        <div class="col-1">
                          <i class="icon fas fa-lock"></i>
                        </div>
                        <div class="col-11">
                          <input class="password" type="password" placeholder="Password" v-model="password" />
                        </div>
                      </div>
                    </div>
                  </div>
                  <router-link class="forgot-btn" to="#">
                    <h5 style="font-size: 15px; font-weight: 300; text-align: center">Forgot password?</h5>
                  </router-link>
                  <div class="button-position">
                    <router-link to="/Home2">
                      <button type="submit" class="btn submit-btn">Login</button>
                    </router-link>
                  </div>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        key: value
      }
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .log-in-bg {
    height: 100vh;
    background-image: url("../assets/backgroundlogin.jpg");
    background-size: cover;
  }

  .logo {
    width: 300px;
    height: 200px;
    object-fit: contain;
  }

  .card {
    padding-top: 50px;
    padding-bottom: 40px;
    border-radius: 25px;
    background-color: rgba(255, 255, 255, 0.925);
  }

  .login-title {
    text-align: center;
    font-weight: 400;
    font-family: "Montserrat", sans-serif;
    font-size: 25px;
  }

  .center-div {
    padding-top: 50px;
  }

  .icon {
    color: #29abe2;
    font-size: 20px;
  }

  .email,
  .password {
    margin-bottom: 30px;
    width: 100%;
    border: none;
    border-bottom: 1px solid rgb(185, 185, 185);
    font-family: "Montserrat", sans-serif;
    font-weight: 300;
    background-color: transparent;
  }

  .forgot-btn {
    text-decoration: none;
    color: rgb(0, 0, 0);
    font-family: "Montserrat", sans-serif;
    font-weight: 600;
    transition: .5s;
  }

  .forgot-btn:hover {
    text-decoration: none;
    color: #29abe2;
    font-family: "Montserrat", sans-serif;
    font-weight: 600;
  }

  .button-position {
    width: 420px;
    margin: auto;
  }

  .submit-btn {
    background-color: #29abe2;
    border: none;
    padding: 8px;
    color: white;
    font-family: "Montserrat", sans-serif;
    font-weight: 400;
    font-size: 13px;
    letter-spacing: 1px;
    width: 200px;
    -webkit-box-shadow: 0 8px 6px -6px black;
    -moz-box-shadow: 0 8px 6px -6px black;
    box-shadow: 0 8px 6px -6px black;
    margin: 5px;
  }
</style>