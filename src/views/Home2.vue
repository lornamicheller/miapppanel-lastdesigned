<template>
    <div>
        <div class="container-fluid" style="margin: 0;">
            <div class="row">
                <!-- <div class="col-3" style="background: #212121; height: 100vh; padding: 0; padding-top: 70px;">
                    <img src="../assets/logomiapplogin.png" class="logo">
                    <nav class="nav flex-column">

                        <router-link class="nav-link" to="/instructions"><img src="../assets/instruction.png"
                                class="home-icon">Instructions</router-link>
                        <router-link class="nav-link" to="/profile"><img src="../assets/profile.png"
                                class="home-icon">Profile</router-link>
                        <router-link class="nav-link" to="/calendar"><img src="../assets/calendar.png"
                                class="home-icon">Calendar</router-link>
                        <a class="nav-link" href="#"><img src="../assets/grafica.png" class="home-icon">Appointment
                            Statistics</a>
                        <router-link class="nav-link" to="/waitlist"><img src="../assets/waitlist.png"
                                class="home-icon">Waitlist</router-link>
                        <a class="nav-link" href="#"><img src="../assets/advertasement.png"
                                class="home-icon">Advertising Opportunities</a>
                    </nav>
                </div> -->
                <div class="col-12" style="padding: 0;">
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
                            <img class="icon-btn4" src="../assets/logout.png">
                        </div>
                    </nav>

                    <div class="container">
                        <div class="row justify-content-center" style="margin-top: 30px; margin-bottom: 20px;">
                            <div class="col-12">
                                <img src="../assets/logo miapp.png"
                                    style="width: 200px; height: 200px; object-fit: contain;">
                            </div>
                        </div>
                        <div class="row justify-content-center">
                            <div class="col-3">
                                <router-link to="/Instructions"><img class="img" src="../assets/instructions.png">
                                </router-link>
                                <p>Instructions</p>
                            </div>
                            <div class="col-3">
                                <router-link to="/Profile"><img class="img" src="../assets/profile boton.png">
                                </router-link>
                                <p>Profile</p>
                            </div>
                            <div class="col-3">
                                <router-link to="/Calendar"><img class="img" src="../assets/calendar botton.png">
                                </router-link>
                                <p>Calendar</p>
                            </div>
                        </div>
                        <div class="row justify-content-center" style="margin-top: 30px;">
                            <div class="col-3">
                                <router-link to="/Statistics"><img class="img" src="../assets/grafica bola 2.png">
                                </router-link>
                                <p>Appointment Statistics</p>
                            </div>
                            <div class="col-3">
                                <router-link to="/Waitlist"><img class="img" src="../assets/waitlist bola.png">
                                </router-link>
                                <p>Waitlist</p>
                            </div>
                            <div class="col-3">
                                <img class="img" src="../assets/advertasing.png">
                                <p>Advertising Opportunities</p>
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
        },
    }
</script>

<style scoped>
    .navbar,
    .navbar-expand-lg,
    .navbar-light,
    .bg-light {
        background: #212121 !important;
        /* padding: 0; */
        height: 80px;
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
        margin-top: 70px;
        margin-bottom: 40px;
    }

    .img {
        transition: .5s;

    }

    .img:hover {
        background: rgb(223, 223, 223);
        height: 100px;
        width: 100px;
        border-radius: 50%;
    }

    .profile-btn {
        height: 80px;
        position: absolute;
        right: 90px;
        background: transparent;
        border-radius: 0;
        border: none;
    }

    .profile-btn:hover {
        background: rgba(255, 255, 255, 0.329);
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