<template>
    <div>
        <div class="container-fluid" style="padding: 0; margin: 0; height: 100%; overflow: hidden;">
            <div class="row" style="height: 100%; margin: 0;">
                <div class="col-3" style="background: #212121; height: 100vh; padding: 0; padding-top: 70px;">
                    <!-- <img src="../assets/logomiapplogin.png" class="logo"> -->
                    <nav class="nav flex-column">

                        <router-link to="/home2" class="nav-link"><img src="../assets/home.png" class="home-icon">Home
                        </router-link>
                        <router-link class="nav-link" to="/instructions"><img src="../assets/instruction.png"
                                class="home-icon">Instructions</router-link>
                        <router-link class="nav-link" to="/profile"><img src="../assets/profile.png"
                                class="home-icon">Profile</router-link>
                        <router-link class="nav-link" style="color: #29abe2 !important;" to="/calendar"><img
                                src="../assets/calendar.png" class="home-icon">Calendar</router-link>
                        <router-link class="nav-link" to="/Statistics"><img src="../assets/grafica.png"
                                class="home-icon">Appointment
                            Statistics</router-link>

                        <router-link class="nav-link" to="/waitlist"><img src="../assets/waitlist.png"
                                class="home-icon">Waitlist</router-link>
                        <a class="nav-link" href="#"><img src="../assets/advertasement.png"
                                class="home-icon">Advertising Opportunities</a>
                        <!-- <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a> -->
                    </nav>

                    <div class="card">
                        <table class="table table-bordered table-hover table-dark" style="margin: 0;">
                            <tbody>
                                <tr>
                                    <th scope="row">Total appointments today:</th>
                                    <td>5</td>
                                </tr>
                                <tr>
                                    <th scope="row">Total appointments weekly:</th>
                                    <td>50</td>
                                </tr>
                                <tr>
                                    <th scope="row">Total appointments monthly:</th>
                                    <td>400</td>
                                </tr>
                                <tr>
                                    <th scope="row">Total appointments yearly:</th>
                                    <td>4,800</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
                <div class="col-9" style="padding: 0; height: 100%;">
                    <nav class="navbar navbar-expand-lg navbar-light bg-light">
                        <img class="logo2" src="../assets/logomiapplogin.png">

                        <p class="text">Medical Intelligent Appointment</p>
                        <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
                            <i class="fas fa-bars"></i>
                        </button> -->

                        <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
                            <router-link to="#" data-toggle="modal" data-target="#exampleModalCenter10"><img
                                    class="icon-btn" src="../assets/block.png"></router-link>
                            <img class="icon-btn2" src="../assets/leyend.png">
                            <router-link to="#" data-toggle="modal" data-target="#exampleModalCenter"><img
                                    class="icon-btn3" src="../assets/plus.png"></router-link>
                            <router-link to="/Login"><img class="icon-btn4" src="../assets/logout.png"></router-link>
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
                    <div class="container-fluid" style="height: 100%; overflow: scroll;">

                        <button class="btn btn-primary settings" data-toggle="modal"
                            data-target=".bd-example-modal-lg">waitlist settings</button>
                        <FullCalendar class='demo-app-calendar' ref="fullCalendar" defaultView="dayGridMonth" :header="{
                                left: 'prev,next today',
                                center: 'title',
                                right: 'dayGridMonth,timeGridWeek,timeGridDay,listWeek'}" :plugins="calendarPlugins"
                            :weekends="calendarWeekends" :events="calendarEvents" @dateClick="handleDateClick" />
                    </div>

                    <div class="containr-fluid">
                        <button class="btn" type="button"
                            style="padding: 0; border: none; background: transparent !important; width: 30px; height: 30px; float: right; margin-top: 20px; margin-right: 20px;"
                            data-toggle="modal" data-target="#exampleModal"><img class="icon-4"
                                src="../assets/help.png"></button>
                    </div>

                    <!-- add patient modal -->
                    <div class="modal fade" id="exampleModalCenter" tabindex="-1" role="dialog"
                        aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
                        <div class="modal-dialog modal-dialog-centered" role="document">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <h5 class="modal-title" id="exampleModalLongTitle"
                                        style="font-family: 'Montserrat', sans-serif;">Add Patient Manually</h5>
                                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                                        <span aria-hidden="true">&times;</span>
                                    </button>
                                </div>
                                <div class="modal-body">
                                    <div class="row justify-content-center mt-3">
                                        <div class="col-10">
                                            <div class="input-group mb-2">
                                                <div class="input-group-prepend">
                                                    <div class="input-group-text"
                                                        style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                                        <i class="fas fa-user-circle input-icon"></i>
                                                    </div>
                                                </div>
                                                <input type="text" class="form-control" id="inlineFormInputGroup"
                                                    placeholder="First Name"
                                                    style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            </div>
                                        </div>
                                    </div>
                                    <div class="row justify-content-center mt-3">
                                        <div class="col-10">
                                            <div class="input-group mb-2">
                                                <div class="input-group-prepend">
                                                    <div class="input-group-text"
                                                        style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                                        <i class="fas fa-user-circle input-icon"></i>
                                                    </div>
                                                </div>
                                                <input type="text" class="form-control" id="inlineFormInputGroup"
                                                    placeholder="Last Name"
                                                    style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            </div>
                                        </div>
                                    </div>
                                    <div class="row justify-content-center mt-3">
                                        <div class="col-10">
                                            <div class="input-group mb-2">
                                                <div class="input-group-prepend">
                                                    <div class="input-group-text"
                                                        style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                                        <i class="fas fa-phone"></i>
                                                    </div>
                                                </div>
                                                <input type="text" class="form-control" id="inlineFormInputGroup"
                                                    placeholder="Patient Phone"
                                                    style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            </div>
                                        </div>
                                    </div>
                                    <div class="row justify-content-center mt-3">
                                        <div class="col-10">
                                            <div class="input-group mb-2">
                                                <div class="input-group-prepend">
                                                    <div class="input-group-text"
                                                        style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                                        <i class="fas fa-envelope"></i>
                                                    </div>
                                                </div>
                                                <input type="text" class="form-control" id="inlineFormInputGroup"
                                                    placeholder="Patient Email"
                                                    style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            </div>
                                        </div>
                                    </div>

                                    <div class="row justify-content-center mt-1">
                                        <div class="col-10">
                                            <div class="input-group mb-3">
                                                <div class="input-group-prepend">
                                                    <div class="input-group-text"
                                                        style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                                        <i class="far fa-credit-card input-card"></i>
                                                    </div>
                                                </div>
                                                <select class="custom-select" id="inputGroupSelect01"
                                                    style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                                    <option selected>Patient Health Insurance</option>
                                                    <option></option>
                                                    <option>Medicare:</option>
                                                    <option value="MCS Classicare">MCS Classicare</option>
                                                    <option value="Triple S Advantage">Triple S Advantage</option>
                                                    <option value="MMM">MMM</option>
                                                    <option value="PMC">PMC</option>
                                                    <option value="Humana Gold">Humana Gold</option>
                                                    <option value="First Choice">First Choice</option>
                                                    <option value="Molina">Molina</option>
                                                    <option value="Constellation">Constellation</option>
                                                    <option value="Humana Medicare Advantage">Humana Medicare Advantage
                                                    </option>
                                                    <option></option>
                                                    <option>Private Insurance:</option>
                                                    <option value="Humana">Humana</option>
                                                    <option value="First Medical">First Medical</option>
                                                    <option value="MAPFRE">MAPFRE</option>
                                                    <option value="MCS">MCS</option>
                                                    <option value="Triple Salud (SSS)">Triple Salud (SSS)</option>
                                                    <option value="PALIG">PALIG</option>
                                                    <option value="Plan de Salud Menonita (PSM)">Plan de Salud Menonita
                                                        (PSM)
                                                    </option>
                                                    <option value="Plan de Auxilio Mutuo">Plan de Auxilio Mutuo</option>
                                                    <option></option>
                                                    <option>Public Insurance:</option>
                                                    <option value="SSS Vital">SSS Vital</option>
                                                    <option value="MM Multi-Health Vital">MM Multi-Health Vital</option>
                                                    <option value="Menonita Vital">Menonita Vital</option>
                                                    <option value="First Medical Vital">First Medical Vital</option>
                                                    <option value="Menonita Vital">Menonita Vital</option>
                                                    <option></option>
                                                    <option value="Don't have medical insurance">Don't have medical
                                                        insurance
                                                    </option>

                                                </select>

                                            </div>
                                        </div>
                                    </div>
                                    <div class="row justify-content-center mt-1">
                                        <div class="col-10">
                                            <div class="input-group mb-3">
                                                <div class="input-group-prepend">
                                                    <div class="input-group-text"
                                                        style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                                        <i class="fas fa-history"></i>
                                                    </div>
                                                </div>
                                                <select class="custom-select" id="inputGroupSelect01"
                                                    style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                                    <option selected>Original Appointment</option>
                                                    <option value="6:00 AM">6:00 AM</option>
                                                    <option value="7:00 AM">7:00 AM</option>
                                                    <option value="8:00 AM">8:00 AM</option>
                                                    <option value="9:00 AM">9:00 AM</option>
                                                    <option value="10:00 AM">10:00 AM</option>
                                                    <option value="11:00 AM">11:00 AM</option>
                                                    <option value="12:00 PM">12:00 PM</option>
                                                    <option value="1:00 PM">1:00 PM</option>
                                                    <option value="2:00 PM">2:00 PM</option>
                                                    <option value="3:00 PM">3:00 PM</option>
                                                    <option value="4:00 PM">4:00 PM</option>
                                                    <option value="5:00 PM">5:00 PM</option>
                                                    <option value="6:00 PM">6:00 PM</option>
                                                    <option value="7:00 PM">7:00 PM</option>
                                                    <option value="8:00 PM">8:00 PM</option>
                                                </select>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="modal-footer">
                                    <button type="button" class="btn btn-secondary" data-dismiss="modal"
                                        style="font-family: 'Montserrat', sans-serif; font-size: 13px;">CLOSE</button>
                                    <button type="button" class="btn btn-primary" style=" background: #29abe2 !important;
                            border-color: #29abe2; font-family: 'Montserrat', sans-serif; font-size: 13px;"
                                        data-toggle="modal" data-target="#exampleModalCenter2">ADD PATIENT</button>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- add patient modal -->

                    <!-- block days Modal -->
                    <div class="modal fade" id="exampleModalCenter10" tabindex="-1" role="dialog"
                        aria-labelledby="exampleModalCenterTitle" aria-hidden="true"
                        style="font-family: 'Montserrat', sans-serif;">
                        <div class="modal-dialog modal-dialog-centered" role="document">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <h5 class="modal-title" id="exampleModalLabel">
                                        Choose range of days that your not going to be available</h5>
                                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                                        <span aria-hidden="true">&times;</span>
                                    </button>
                                </div>
                                <div class="modal-body">
                                    <form>
                                        <div class="row">
                                            <div class="col">
                                                <label>Start Day</label>
                                                <input type="date" class="form-control" placeholder="First name">
                                            </div>
                                            <div class="col">
                                                <label>End Day</label>
                                                <input type="date" class="form-control" placeholder="Last name">
                                            </div>
                                        </div>
                                    </form>
                                </div>
                                <div class="modal-footer">
                                    <button type="button" class="btn btn-secondary" data-dismiss="modal"
                                        style="font-family: 'Montserrat', sans-serif; font-size: 13px;">CLOSE</button>
                                    <button data-toggle="modal" data-target="#exampleModalCenter25" type="button"
                                        class="btn btn-primary" style="font-family: 'Montserrat', sans-serif; font-size: 13px; background: #29abe2 !important;
                                    border-color: #29abe2;">SAVE</button>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- block days -->

                    <!-- block days alert -->
                    <div class="modal fade" id="exampleModalCenter25" tabindex="-1" role="dialog"
                        aria-labelledby="exampleModalCenterTitle" aria-hidden="true"
                        style="font-family: 'Montserrat', sans-serif;">
                        <div class="modal-dialog modal-dialog-centered" role="document">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <!-- <h5 class="modal-title" id="exampleModalCenterTitle">Modal title</h5> -->
                                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                                        <span aria-hidden="true">&times;</span>
                                    </button>
                                </div>
                                <div class="modal-body">
                                    <p>Your patients will be notified.</p>
                                </div>
                                <div class="modal-footer">
                                    <button type="button" class="btn btn-secondary" data-dismiss="modal"
                                        style="font-family: 'Montserrat', sans-serif; font-size: 13px;">CLOSE</button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- block days alert -->

                    <!-- modal need help -->
                    <div class="modal fade" id="exampleModal" tabindex="-1" role="dialog"
                        aria-labelledby="exampleModalLabel" aria-hidden="true"
                        style="font-family: 'Montserrat', sans-serif;">
                        <div class="modal-dialog" role="document">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <h5 class="modal-title" id="exampleModalLabel"
                                        style="font-family: 'Montserrat', sans-serif;">Need asistance or training?</h5>
                                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                                        <span aria-hidden="true">&times;</span>
                                    </button>
                                </div>
                                <div class="modal-body">
                                    <p style="font-family: 'Montserrat', sans-serif;">Call 939-277-8068 or write your
                                        request to masmaktech@gmail.com</p>
                                    <p style="font-family: 'Montserrat', sans-serif;">A representative will contact you
                                        as soon as possible. Thank you for using Miapp!</p>

                                </div>
                                <div class="modal-footer">
                                    <button type="button" class="btn btn-secondary" data-dismiss="modal"
                                        style="font-family: 'Montserrat', sans-serif; font-size: 13px;">CLOSE</button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- modal need help -->

                    <!-- miapp promo modal -->

                    <div class="modal fade" id="exampleModalCenter2" tabindex="-1" role="dialog2"
                        aria-labelledby="exampleModalCenterTitle" aria-hidden="true"
                        style="font-family: 'Montserrat', sans-serif;">
                        <div class="modal-dialog modal-dialog-centered" role="document">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <!-- <h5 class="modal-title" id="exampleModalLongTitle"
                            style="font-family: 'Montserrat', sans-serif;">Add Patient Manually</h5> -->
                                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                                        <span aria-hidden="true">&times;</span>
                                    </button>
                                </div>
                                <div class="modal-body">
                                    <p style="font-weight: 500; padding-top: 100px; padding-bottom: 100px;">Would you
                                        like to send
                                        MiApp to patient?</p>
                                </div>
                                <div class="modal-footer">
                                    <button type="button" class="btn btn-secondary" data-dismiss="modal"
                                        style="font-family: 'Montserrat', sans-serif; font-size: 13px;">NO</button>
                                    <button type="button" class="btn btn-primary" style="font-family: 'Montserrat', sans-serif;  background: #29abe2 !important;
                                    border-color: #29abe2; font-size: 13px;" data-toggle="modal"
                                        data-target="#exampleModalCenter2">YES</button>
                                </div>
                            </div>
                        </div>
                    </div>


                    <!-- modal waitlist setting -->
                    <div class="modal fade bd-example-modal-lg" tabindex="-1" role="dialog"
                        aria-labelledby="myLargeModalLabel" aria-hidden="true"
                        style="font-family: 'Montserrat', sans-serif;">
                        <div class="modal-dialog modal-lg">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <h5 class="modal-title" id="exampleModalLabel"
                                        style="font-family: 'Montserrat', sans-serif;">Waitlist setting</h5>
                                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                                        <span aria-hidden="true">&times;</span>
                                    </button>
                                </div>
                                <div class="modal-body">
                                    <div class="form-group">
                                        <select style="font-family: 'Montserrat', sans-serif; font-size: 15px;"
                                            class="form-control" id="exampleFormControlSelect1">
                                            <option>Open Manually / Close Manually</option>
                                            <option>Open Automatically / Close Manually</option>
                                            <option>Open Manually / Close Automatically</option>
                                            <option>Open Automatically / Close Automatically</option>
                                        </select>
                                    </div>

                                    <div class="container">
                                        <p>When open automatically please choose days and time for waitlist to open and
                                            close</p>
                                        <div class="row justify-content-center">
                                            <div class="col-lg-2 col-md-2 col-sm-12">
                                                <h1 class="title-schedule">Days</h1>
                                                <div class="day-container">
                                                    <button type="button"
                                                        class="btn btn-primary delete-btn delete-active">Sunday</button>
                                                </div>
                                                <div class="day-container">
                                                    <button type="button"
                                                        class="btn btn-primary delete-btn">Monday</button>
                                                </div>
                                                <div class="day-container">
                                                    <button type="button"
                                                        class="btn btn-primary delete-btn">Tuesday</button>
                                                </div>
                                                <div class="day-container">
                                                    <button type="button"
                                                        class="btn btn-primary delete-btn">Wednesday</button>
                                                </div>
                                                <div class="day-container">
                                                    <button type="button"
                                                        class="btn btn-primary delete-btn">Thursday</button>
                                                </div>
                                                <div class="day-container">
                                                    <button type="button"
                                                        class="btn btn-primary delete-btn">Friday</button>
                                                </div>
                                                <div class="day-container">
                                                    <button type="button"
                                                        class="btn btn-primary delete-btn">Saturday</button>
                                                </div>
                                            </div>
                                            <div class="col-lg-2 col-md-2 col-sm-12">
                                                <h1 class="title-schedule">Open</h1>

                                                <!-- Sunday Input -->
                                                <select class="form-control start-schedule" placeholder="0:00AM">
                                                    <option value="Manually" class="title-category">Manually</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Monday Input -->
                                                <select class="form-control start-schedule" placeholder="0:00AM">
                                                    <option value="Manually" class="title-category">Manually</option>

                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!--Tuesday Input -->

                                                <select class="form-control start-schedule" placeholder="0:00AM">
                                                    <option value="Manually" class="title-category">Manually</option>

                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Wednesday Input -->

                                                <select class="form-control start-schedule" placeholder="0:00AM">
                                                    <option value="Manually" class="title-category">Manually</option>

                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Thursday Input -->

                                                <select class="form-control start-schedule" placeholder="0:00AM">
                                                    <option value="Manually" class="title-category">Manually</option>

                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Friday Input -->

                                                <select class="form-control start-schedule" placeholder="0:00AM">
                                                    <option value="Manually" class="title-category">Manually</option>

                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Saturday Input -->

                                                <select class="form-control start-schedule" placeholder="0:00AM">
                                                    <option value="Manually" class="title-category">Manually</option>

                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>
                                            </div>
                                            <div class="col-lg-2 col-md-2 col-sm-12">
                                                <h1 class="title-schedule">Close</h1>

                                                <!-- Sunday Input -->
                                                <select class="form-control start-schedule" placeholder="0:00PM">
                                                    <option value="Manually" class="title-category">Manually</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Monday Input -->
                                                <select class="form-control start-schedule" placeholder="0:00PM">
                                                    <option value="Manually" class="title-category">Manually</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!--Tuesday Input -->
                                                <select class="form-control start-schedule" placeholder="0:00PM">
                                                    <option value="Manually" class="title-category">Manually</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Wednesday Input -->

                                                <select class="form-control start-schedule" placeholder="0:00PM">
                                                    <option value="Manually" class="title-category">Manually</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Thursday Input -->

                                                <select class="form-control start-schedule" placeholder="0:00PM">
                                                    <option value="Manually" class="title-category">Manually</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Friday Input -->

                                                <select class="form-control start-schedule" placeholder="0:00PM">
                                                    <option value="Manually" class="title-category">Manually</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>

                                                <!-- Saturday Input -->
                                                <select class="form-control start-schedule" placeholder="0:00PM">
                                                    <option value="Manually" class="title-category">Manually</option>
                                                    <option value="12:00AM" class="title-category">12:00AM</option>
                                                    <option value="12:30AM" class="title-category">12:30AM</option>
                                                    <option value="1:00AM" class="title-category">1:00AM</option>
                                                    <option value="1:30AM" class="title-category">1:30AM</option>
                                                    <option value="2:00AM" class="title-category">2:00AM</option>
                                                    <option value="2:30AM" class="title-category">2:30AM</option>
                                                    <option value="3:00AM" class="title-category">3:00AM</option>
                                                    <option value="3:30AM" class="title-category">3:30AM</option>
                                                    <option value="4:00AM" class="title-category">4:00AM</option>
                                                    <option value="4:30AM" class="title-category">4:30AM</option>
                                                    <option value="5:00AM" class="title-category">5:00AM</option>
                                                    <option value="5:30AM" class="title-category">5:30AM</option>
                                                    <option value="6:00AM" class="title-category">6:00AM</option>
                                                    <option value="6:30AM" class="title-category">6:30AM</option>
                                                    <option value="7:00AM" class="title-category">7:00AM</option>
                                                    <option value="7:30AM" class="title-category">7:30AM</option>
                                                    <option value="8:00AM" class="title-category">8:00AM</option>
                                                    <option value="8:30AM" class="title-category">8:30AM</option>
                                                    <option value="9:00AM" class="title-category">9:00AM</option>
                                                    <option value="9:30AM" class="title-category">9:30AM</option>
                                                    <option value="10:00AM" class="title-category">10:00AM</option>
                                                    <option value="10:30AM" class="title-category">10:30AM</option>
                                                    <option value="11:00AM" class="title-category">11:00AM</option>
                                                    <option value="11:30AM" class="title-category">11:30AM</option>
                                                    <option value="12:00PM" class="title-category">12:00PM</option>
                                                    <option value="12:30PM" class="title-category">12:30PM</option>
                                                    <option value="1:00PM" class="title-category">1:00PM</option>
                                                    <option value="1:30PM" class="title-category">1:30PM</option>
                                                    <option value="2:00PM" class="title-category">2:00PM</option>
                                                    <option value="2:30PM" class="title-category">2:30PM</option>
                                                    <option value="3:00PM" class="title-category">3:00PM</option>
                                                    <option value="3:30PM" class="title-category">3:30PM</option>
                                                    <option value="4:00PM" class="title-category">4:00PM</option>
                                                    <option value="4:30PM" class="title-category">4:30PM</option>
                                                    <option value="5:00PM" class="title-category">5:00PM</option>
                                                    <option value="5:30PM" class="title-category">5:30PM</option>
                                                    <option value="6:00PM" class="title-category">6:00PM</option>
                                                    <option value="6:30PM" class="title-category">6:30PM</option>
                                                    <option value="7:00PM" class="title-category">7:00PM</option>
                                                    <option value="7:30PM" class="title-category">7:30PM</option>
                                                    <option value="8:00PM" class="title-category">8:00PM</option>
                                                    <option value="8:30PM" class="title-category">8:30PM</option>
                                                    <option value="9:00PM" class="title-category">9:00PM</option>
                                                    <option value="9:30PM" class="title-category">9:30PM</option>
                                                    <option value="10:00PM" class="title-category">10:00PM</option>
                                                    <option value="10:30PM" class="title-category">10:30PM</option>
                                                    <option value="11:00PM" class="title-category">11:00PM</option>
                                                    <option value="11:30PM" class="title-category">11:30PM</option>
                                                </select>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="modal-footer">
                                    <button type="button" class="btn btn-secondary" data-dismiss="modal"
                                        style="font-family: 'Montserrat', sans-serif; font-size: 13px;">CLOSE</button>
                                    <button type="button" class="btn btn-primary" style="font-family: 'Montserrat', sans-serif; font-size: 13px; background: #29abe2 !important;
                        border-color: #29abe2;">SAVE</button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- modal waitlist setting -->
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import FullCalendar from '@fullcalendar/vue'
    import dayGridPlugin from '@fullcalendar/daygrid'
    import timeGridPlugin from '@fullcalendar/timegrid'
    import interactionPlugin from '@fullcalendar/interaction'
    import listPlugin from '@fullcalendar/list';

    export default {
        el: '#hide',
        components: {
            FullCalendar // make the <FullCalendar> tag available
        },
        data: function () {
            return {
                seen: false,
                calendarPlugins: [ // plugins must be defined in the JS
                    dayGridPlugin,
                    timeGridPlugin,
                    listPlugin,
                    interactionPlugin // needed for dateClick
                ],
                calendarWeekends: true,
                calendarEvents: [ // initial event data
                    {
                        title: 'Event Now',
                        start: new Date()
                    }
                ]
            }
        },
        methods: {
            toggleWeekends() {
                this.calendarWeekends = !this.calendarWeekends // update a property
            },
            gotoPast() {
                let calendarApi = this.$refs.fullCalendar.getApi() // from the ref="..."
                calendarApi.gotoDate('2000-01-01') // call a method on the Calendar object
            },
            handleDateClick(arg) {
                if (confirm('Would you like to add an event to ' + arg.dateStr + ' ?')) {
                    this.calendarEvents.push({ // add new event data
                        title: 'New Event',
                        start: arg.date,
                        allDay: arg.allDay
                    })
                }
            }
        }
    }
</script>

<style scoped>
    @import '~@fullcalendar/core/main.css';
    @import '~@fullcalendar/daygrid/main.css';
    @import '~@fullcalendar/timegrid/main.css';
    @import '~@fullcalendar/list/main.css';

    .demo-app {
        font-family: 'Montserrat', sans-serif;
        /* font-family: Arial, Helvetica Neue, Helvetica, sans-serif; */
        font-size: 14px;
        background: 1e1e1e !important;
    }

    .demo-app-top {
        margin: 0 0 3em;
    }

    .demo-app-calendar {
        margin: 5px;
        max-width: 100%;
        height: 600px;
    }

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

    .icon-btn {
        width: 30px;
        height: 30px;
        position: absolute;
        right: 170px;
        top: 25px;

    }

    .icon-btn2 {
        width: 30px;
        height: 30px;
        position: absolute;
        right: 130px;
    }

    .icon-btn3 {
        width: 30px;
        height: 30px;
        position: absolute;
        top: 25px;
        right: 90px;
    }

    .icon-btn4 {
        width: 30px;
        height: 30px;
        position: absolute;
        right: 50px;
        top: 25px;
    }

    .icon-4 {
        width: 30px;
        height: 30px;
        box-shadow: 0 8px 6px -6px black;
        border-radius: 50%;
    }

    /* switch button */

    .onoffswitch {
        position: relative;
        width: 90px;
        -webkit-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
    }

    .onoffswitch-checkbox {
        display: none;
    }

    .onoffswitch-label {
        display: block;
        overflow: hidden;
        cursor: pointer;
        border: 2px solid #FFFFFF;
        border-radius: 20px;
    }

    .onoffswitch-inner {
        display: block;
        width: 200%;
        margin-left: -100%;
        transition: margin 0.3s ease-in 0s;
    }

    .onoffswitch-inner:before,
    .onoffswitch-inner:after {
        display: block;
        float: left;
        width: 50%;
        height: 30px;
        padding: 0;
        line-height: 30px;
        font-size: 14px;
        color: white;
        font-family: Trebuchet, Arial, sans-serif;
        font-weight: bold;
        box-sizing: border-box;
    }

    .onoffswitch-inner:before {
        content: "OFF";
        padding-left: 10px;
        padding-right: 10px;
        background-color: #FA3754;
        color: #FFFFFF;
    }

    .onoffswitch-inner:after {
        content: "ON";
        padding-right: 10px;
        background-color: #00C7B0;
        color: #FFFFFF;
        text-align: right;
    }

    .onoffswitch-switch {
        display: block;
        width: 22px;
        height: 22px;
        margin: 6px;
        background: #FFFFFF;
        position: absolute;
        top: 0;
        bottom: 0;
        right: 56px;
        border: 2px solid #FFFFFF;
        border-radius: 20px;
        transition: all 0.3s ease-in 0s;
    }

    .onoffswitch-checkbox:checked+.onoffswitch-label .onoffswitch-inner {
        margin-left: 0;
    }

    .onoffswitch-checkbox:checked+.onoffswitch-label .onoffswitch-switch {
        right: 0px;
    }

    /* switch button */


    .close-label {
        font-weight: 500;
        font-size: 13px;
        margin-top: 10px;
        margin-right: 5px;
    }

    .open-label {
        font-weight: 500;
        margin-top: 10px;
        margin-left: 5px;
        font-size: 13px;
    }


    .table-striped tbody tr:nth-of-type(odd) {
        background: #29aae22c;
    }

    .table-head {
        font-size: 13px;
        font-weight: 600;
    }

    .dr-icon {
        width: 40px;
        height: 40px;
    }

    .table-btn {
        font-size: 13px;
        background-image: linear-gradient(to right top, #93278f, #7c55b7, #5976d1, #3392df, #29abe2) !important;
        border: none;
        font-weight: 500;
    }

    .content-table {
        font-size: 13px;
        font-weight: 500;
        padding-top: 20px !important;
    }

    .home-icon {
        width: 20px;
        height: 20px;
        margin-right: 10px;
    }

    .fc-head-container .fc-widget-header {
        height: 60px !important;
        font-family: "Montserrat", sans-serif;
    }

    .fc-day-header {
        padding-top: 16px !important;
    }

    .card {
        margin-top: 100px;
        box-shadow: 0 8px 6px -6px black;
        margin-bottom: 20px;
        border-color: rgb(54, 54, 54);
        border-left: 0;
        border-right: 0;
        border-bottom: 0;
        border-radius: 0;
        background: transparent;
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

    .table-dark td,
    .table-dark th,
    .table-dark thead th {
        background: #212121;
        /* border-color: #212121; */
    }

    .settings {
        float: right;
        margin-left: 20px;
        margin-right: 10px;
        margin-top: 7px;
        border: none;
        background: #2C3E52 !important;
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

    .active {
        width: 100px;
        font-family: "Montserrat", sans-serif;
        font-weight: 300;
        font-size: 13px;
        background: #29abe2;
        color: white;
        border-color: #29abe2;
    }

    .start-schedule {
        margin-bottom: 10px;
        border: 1px solid rgb(199, 199, 199);
        border-radius: 5px;
        margin-top: 3px;
        padding-left: 17px;
        text-align: center;
        font-size: 13px;
    }

    .title-schedule {
        font-family: "Montserrat", sans-serif;
        text-align: center;
        font-size: 17px;
    }

    .profile-btn {
        height: 80px;
        position: absolute;
        right: 220px !important;
        background: transparent;
        border-radius: 0;
        border: none;
        top: -100px;
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
        top: -20px;
        right: 220px !important;
        height: 400px;
        overflow: scroll;
        z-index: 100;
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