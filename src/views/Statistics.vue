<template>
    <div>
        <div class="container-fluid" style="margin: 0;">
            <div class="row">
                <div class="col-3"
                    style="background: #212121 !important; height: 100vh; padding: 0; padding-top: 70px;">
                    <!-- <img src="../assets/logomiapplogin.png" class="logo"> -->
                    <nav class="nav flex-column" style="  overflow: hidden; position: fixed; left: 0;">
                        <router-link class="nav-link" to="/home2"><img src="../assets/home.png" class="home-icon">Home
                        </router-link>
                        <router-link class="nav-link" to="/instructions"><img src="../assets/instruction.png"
                                class="home-icon">Instructions</router-link>
                        <router-link class="nav-link" to="/profile"><img src="../assets/profile.png"
                                class="home-icon">Profile</router-link>
                        <router-link class="nav-link" to="/calendar"><img src="../assets/calendar.png"
                                class="home-icon">Calendar</router-link>
                        <router-link class="nav-link" to="/Statistics" style="color: #29abe2 !important;"><img
                                src="../assets/grafica.png" class="home-icon">Appointment
                            Statistics</router-link>

                        <router-link class="nav-link" to="/waitlist"><img src="../assets/waitlist.png"
                                class="home-icon">Waitlist</router-link>
                        <a class="nav-link" href="#"><img src="../assets/advertasement.png"
                                class="home-icon">Advertising Opportunities</a>
                        <!-- <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a> -->
                    </nav>
                </div>
                <div class="col-9" style="padding: 0;">
                    <nav class="navbar navbar-expand-lg navbar-light bg-light">
                        <img class="logo2" src="../assets/logomiapplogin.png">

                        <p class="text">Medical Intelligent Appointment</p>
                        <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
                            <i class="fas fa-bars"></i>
                        </button> -->

                        <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
                            <!-- <img class="icon-btn" src="../assets/block.png">
                            <img class="icon-btn2" src="../assets/leyend.png">
                            <img class="icon-btn3" src="../assets/plus.png"> -->
                            <img class="icon-btn4" src="../assets/logout.png">
                        </div>

                        <div class="card profile-btn" v-on:click="seen = !seen"
                            style="width: 18rem; borde-radius: 0; background: transparent; border: 0;">
                            <img class="dropdown-img" src="../assets/doc.jpg">
                            <p class="dr-name">John Doe</p>
                        </div>

                        <div class="card dropdown-card" style="width: 18rem;" v-if="seen" id="hide">

                            <!-- first profile -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor2 2.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>


                            <!-- second profile  -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor1.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>

                            <!-- third profile -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor3.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>


                            <!-- third profile -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor4.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>


                            <!-- third profile -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor5.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>


                            <!-- third profile -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor6.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>


                            <!-- third profile -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor7.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>


                            <!-- third profile -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor8.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>


                            <!-- third profile -->

                            <div class="container-fluid doctor-profile" style="margin: 0; padding: 0;">
                                <div class="row justify-content-center" style="margin: 0;">
                                    <div class="col-2">
                                        <img class="profile-pic-small" src="../assets/doctor9.png">
                                    </div>
                                    <div class="col-10">
                                        <p class="dr-name2">John Doe</p>
                                    </div>
                                </div>
                            </div>



                        </div>

                    </nav>

                    <div class="container-fluid" style="overflow: scroll; height: 100vh;">
                        <div class="row justify-content-center" style="padding-top: 80px">
                            <div class="col-md-6 col-sm-12 col-xs-12">
                                <div class="card">
                                    <img src="../assets/check.png" class="card-img-top img-icon" alt="...">
                                    <table class="table table-bordered table-hover table-dark" style="margin: 0;">
                                        <tbody>
                                            <tr>
                                                <th scope="row">Total appointment today:</th>
                                                <td>5</td>
                                            </tr>
                                            <tr>
                                                <th scope="row">Total patients pending confirmation:</th>
                                                <td>5</td>
                                            </tr>
                                            <tr>
                                                <th scope="row">Total patients confirmed:</th>
                                                <td>5</td>
                                            </tr>
                                            <tr>
                                                <th scope="row">Total patients pending check-in:</th>
                                                <td>5</td>
                                            </tr>
                                            <tr>
                                                <th scope="row">Total patients with check-in complete:</th>
                                                <td>5</td>
                                            </tr>
                                            <tr>
                                                <th scope="row">Total patients pending arrival:</th>
                                                <td>5</td>
                                            </tr>
                                            <tr>
                                                <th scope="row">Total patients that have arrived:</th>
                                                <td>5</td>
                                            </tr>
                                        </tbody>
                                    </table>
                                </div>
                            </div>
                            <div class="col-md-6 col-sm-12 col-xs-12">
                                <div class="card">
                                    <img src="../assets/totalpersonas.png" class="card-img-top img-icon" alt="...">
                                    <table class="table table-bordered table-hover table-dark" style="margin: 0;">
                                        <thead>
                                        </thead>
                                        <tbody>
                                            <tr>
                                                <th scope="row">Total patients that have completed their appointment:
                                                </th>
                                                <td>30</td>
                                            </tr>
                                            <tr>
                                                <th scope="row">Total patients remaining for today:</th>
                                                <td>10</td>
                                            </tr>
                                        </tbody>
                                    </table>
                                </div>
                                <div class="card">
                                    <img src="../assets/time.png" class="card-img-top img-icon" alt="...">
                                    <table class="table table-bordered table-hover table-dark" style="margin: 0;">
                                        <thead>
                                        </thead>
                                        <tbody>
                                            <tr>
                                                <th scope="row">Current estimated wait time per patient:
                                                </th>
                                                <td>30 minutes</td>
                                            </tr>
                                        </tbody>
                                    </table>
                                </div>
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
        el: '#hide',
        data() {
            return {
                seen: false
            }
        }
    }
</script>

<style scoped>
    .navbar,
    .navbar-expand-lg,
    .navbar-light,
    .bg-light {
        background: #212121 !important;
        height: 80px;
        top: 0;
        width: 100%;

    }

    .nav-item {
        font-family: 'Montserrat', sans-serif;
    }

    .nav-link {
        color: white !important;
        font-weight: 200;
        font-size: 13px;
        /* letter-spacing: 1px; */
        margin-left: 20px;
        margin-right: 20px;
        transition: .5s;
        text-align: left;
        width: 300px;
        margin-left: 0;
    }

    .nav-link:hover {
        color: #29abe2 !important;
        font-weight: 200;
        /* font-size: 14px; */
        /* letter-spacing: 1px; */
        /* margin-left: 20px; */
        margin-right: 20px;
    }

    .logo-link {
        position: absolute;
        left: 20px;
        top: 10px;
    }

    .navbar-toggler {
        border: 2px solid rgb(184, 184, 184) !important;
    }

    .fa-bars {
        color: rgb(184, 184, 184);
        font-size: 25px;
    }

    .logo {
        height: 90px;
        object-fit: contain;
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 90px;
    }

    .logo2 {
        height: 90px;
        object-fit: contain;
        width: 70px;
    }

    .text {
        color: white;
        margin-left: 20px;
        margin-top: 15px;
        font-weight: 500;
    }

    .icon-btn4 {
        width: 30px;
        height: 30px;
        position: absolute;
        right: 50px;
    }

    .home-icon {
        width: 20px;
        height: 20px;
        margin-right: 10px;
    }

    .profile-pic {
        width: 150px;
        height: 150px;
        border-radius: 50%;
        margin-top: 120px;
        margin-bottom: 40px;
        box-shadow: 0 8px 6px -6px black;
    }

    .day-container {
        margin-bottom: 10px;
        text-align: center;
    }

    .delete-btn {
        width: 100%;
        font-family: "Montserrat", sans-serif;
        font-weight: 300;
        font-size: 13px;
        background: transparent;
        border-radius: none;
        color: grey;
        border-color: #29abe2;
    }

    .delete-btn:hover {
        width: 100%;
        font-family: "Montserrat", sans-serif;
        font-weight: 300;
        font-size: 13px;
        background: #29abe2;
        color: white;
        border-color: #29abe2;
    }



    .card {
        box-shadow: 0 8px 6px -6px black;
        margin-bottom: 20px;
        border-bottom: 0;
    }

    .img-icon {
        width: 130px;
        height: 130px;
        display: block;
        margin-top: 20px;
        margin-bottom: 20px;
        margin-left: auto;
        margin-right: auto;
    }

    /* .table-dark td, .table-dark th, .table-dark thead th {
        background: #29abe2;
    } */

    .profile-btn {
        height: 80px;
        position: absolute;
        right: 90px;
        background: transparent;
        border-radius: 0;
        border: none;
        box-shadow: none;
    }

    .profile-btn:hover {
        background: rgba(255, 255, 255, 0.445);
    }

    .dr-name {
        font-family: "Montserrat", sans-serif;
        text-align: right;
        margin-right: 10px;
        margin-top: 25px;
        font-size: 20px;
        color: white;
    }

    .dropdown-img {
        width: 50px;
        height: 50px;
        border-radius: 50%;
        margin-top: 15px;
        position: absolute;
        left: 10px;
        object-fit: cover;
    }

    .dropdown-card {
        background: #383838;
        border-top-left-radius: 0;
        border-top-right-radius: 0;
        position: absolute;
        top: 80px;
        right: 90px;
        height: 400px;
        overflow: scroll;
        z-index: 100;
        /* display: none; */
        border-radius: 0;
        border: none;
        /* display: none; */
        box-shadow: 0 8px 6px -6px black;
    }

    .doctor-profile {
        height: 60px;
        margin: 0;
        padding: 0;
    }

    .doctor-profile:hover {
        height: 60px;
        margin: 0;
        padding: 0;
        background: rgba(255, 255, 255, 0.329);
    }

    .profile-pic-small {
        width: 40px;
        height: 40px;
        border-radius: 50%;
        margin-top: 10px;
        object-fit: cover;
    }

    .dr-name2 {
        text-align: right;
        color: white;
        font-size: 15px;
        margin-right: 10px;
        margin-top: 20px;
    }
</style>