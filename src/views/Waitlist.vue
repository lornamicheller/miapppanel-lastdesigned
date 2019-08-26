<template>
    <div>
        <div class="container-fluid" style="padding: 0; margin: 0; height: 100%; overflow: hidden;">
            <div class="row" style="height: 100%; margin: 0;">
                <div class="col-3" style="background: #212121; height: 100%; padding: 0; padding-top: 70px;">
                    <!-- <img src="../assets/logomiapplogin.png" class="logo"> -->
                    <nav class="nav flex-column" style="height: 100vh;">

                        <router-link class="nav-link" to="/home2"><img src="../assets/home.png" class="home-icon">Home
                        </router-link>
                        <router-link class="nav-link" to="/instructions"><img src="../assets/instruction.png"
                                class="home-icon">Instructions</router-link>
                        <router-link class="nav-link" to="/profile"><img src="../assets/profile.png"
                                class="home-icon">Profile</router-link>
                        <router-link class="nav-link" to="/calendar"><img src="../assets/calendar.png"
                                class="home-icon">Calendar</router-link>
                        <router-link class="nav-link" to="/Statistics"><img src="../assets/grafica.png"
                                class="home-icon">Appointment
                            Statistics</router-link>
                        <!-- <router-link class="nav-link" to="/Patients"><i class="fas fa-bars"
                                style="color: white; margin-right: 9px;"></i>Patients' Information</router-link> -->
                        <router-link class="nav-link" style="color: #29abe2 !important;" to="/waitlist"><img
                                src="../assets/waitlist.png" class="home-icon">Waitlist</router-link>
                        <a class="nav-link" href="#"><img src="../assets/advertasement.png"
                                class="home-icon">Advertising Opportunities</a>
                        <!-- <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a> -->
                    </nav>

                    <div class="container-fluid" style="position: absolute; top: 400px;">
                        <div>
                            <p style="text-align: left; color: white;"><i class="fas fa-circle"
                                    style="color: white; margin-right: 10px;"></i>Patient is in the waitlist.</p>
                        </div>
                        <div>
                            <p style="text-align: left; color: white;"><i class="fas fa-circle"
                                    style="color: grey; margin-right: 10px;"></i>Patient completed or canceled
                                appointment.</p>
                        </div>
                        <div>
                            <p style="text-align: left; color: white;"><i class="fas fa-circle"
                                    style="color: #29abe2; margin-right: 10px;"></i>Health or Wellness provider is
                                currently attending to this
                                patient.</p>
                        </div>
                    </div>
                </div>
                <div class="col-9" style="padding: 0; height: 100vh;">
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
                            <router-link to="/login"><img class="icon-btn4" src="../assets/logout.png"></router-link>
                        </div>
                    </nav>

                    <div class="container-fluid" style="padding-top: 10px; display: flex; width: 100%;">
                        <p class="close-label">Close Waitlist</p>
                        <div class="onoffswitch">
                            <input type="checkbox" name="onoffswitch" class="onoffswitch-checkbox" id="myonoffswitch"
                                checked>
                            <label class="onoffswitch-label" for="myonoffswitch">
                                <span class="onoffswitch-inner"></span>
                                <span class="onoffswitch-switch"></span>
                            </label>
                        </div>
                        <p class="open-label">Open Waitlist</p>

                        <button class="btn btn-primary settings" data-toggle="modal"
                            data-target=".bd-example-modal-lg">waitlist settings</button>

                        <button type="button" class="btn btn-primary add-btn" data-toggle="modal"
                            data-target="#exampleModalCenter"><i class="fas fa-plus"></i></button>
                    </div>

                    <div class="container-fluid" style="padding: 0; height: 100%; overflow: scroll;">

                        <table class="table table-striped table-borderless table-hover table-dark" style="margin: 0;">
                            <thead>
                                <tr>
                                    <th class="table-head" scope="col">Order</th>
                                    <th class="table-head" scope="col">Name</th>
                                    <th class="table-head" scope="col">Original Appointment Time</th>
                                    <th class="table-head" scope="col">Estimated Actual Appointment Time</th>
                                    <th class="table-head" scope="col">Status of Patient</th>
                                    <th class="table-head" scope="col">Click "Begin Turn" When Patient Begins
                                        Appointment"
                                    </th>
                                    <!-- <th class="table-head" scope="col">Click "Complete Turn" When Patient Finishes Appointment"</th> -->
                                    <th class="table-head" scope="col">Move Patient's Turn</th>
                                    <th class="table-head" scope="col">Cancel Patient's Turn</th>
                                    <!-- <th class="table-head" scope="col">Click "Complete" When Patient Finishes Appointent
                                </th> -->

                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td class="content-table">1</td>
                                    <td class="content-table">Jane Doe
                                        <router-link to="#" data-toggle="modal" data-target="#exampleModalCenter30">View More</router-link>
                                    </td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter7">Complete Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">2</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Booked and pending confirmation
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>

                                <tr>
                                    <td class="content-table">3</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Confirmed
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">4</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Pending Check-in
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">5</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Arrived at Office
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">6</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Canceled Appointment
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">7</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Delayed
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">8</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">9</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">10</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">11</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">12</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">13</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">14</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">15</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">16</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">17</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">18</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">19</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">20</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">21</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">22</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">23</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">24</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">25</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">26</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>
                                <tr>
                                    <td class="content-table">27</td>
                                    <td class="content-table">Jane Doe</td>
                                    <td class="content-table">8:00am</td>
                                    <td class="content-table">8:45am</td>
                                    <td class="content-table">Check-in Complete
                                        <!-- Different status of patients are
                                    - Booked and pending confirmation
                                    - Confirmed
                                    - Pending Check-in
                                    - Checked-in
                                    - Arrived at Office
                                    - Canceled Appointment
                                    - Delayed (Amount of time 15mins, 30mins, 1 hour )
                                    -->
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn">Begin Turn</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter3">Move</button>
                                    </td>
                                    <td>
                                        <button type="button" class="btn btn-primary table-btn" data-toggle="modal"
                                            data-target="#exampleModalCenter6">Cancel</button>
                                    </td>
                                    <!-- <td>
                                    <button type="button" class="btn btn-primary table-btn">Complete</button>
                                </td> -->
                                </tr>

                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
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
                                        <option value="Humana Medicare Advantage">Humana Medicare Advantage</option>
                                        <option></option>
                                        <option>Private Insurance:</option>
                                        <option value="Humana">Humana</option>
                                        <option value="First Medical">First Medical</option>
                                        <option value="MAPFRE">MAPFRE</option>
                                        <option value="MCS">MCS</option>
                                        <option value="Triple Salud (SSS)">Triple Salud (SSS)</option>
                                        <option value="PALIG">PALIG</option>
                                        <option value="Plan de Salud Menonita (PSM)">Plan de Salud Menonita (PSM)
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
                                        <option value="Don't have medical insurance">Don't have medical insurance
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

        <!-- miapp promo modal -->

        <div class="modal fade" id="exampleModalCenter2" tabindex="-1" role="dialog2"
            aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
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
                        <p style="font-weight: 500; padding-top: 100px; padding-bottom: 100px;">Would you like to send
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

        <!-- miapp promo modal -->

        <div class="modal fade" id="exampleModalCenter30" tabindex="-1" role="dialog"
            aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
            <div class="modal-dialog modal-dialog-centered" role="document">
                <div class="modal-content">
                    <div class="modal-header">
                        <h5 class="modal-title" id="exampleModalLongTitle">Modal title</h5>
                        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                            <span aria-hidden="true">&times;</span>
                        </button>
                    </div>
                    <div class="modal-body">
                        ...
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
                        <button type="button" class="btn btn-primary">Save changes</button>
                    </div>
                </div>
            </div>
        </div>

        <!-- move btn modal -->
        <div class="modal fade" id="exampleModalCenter3" tabindex="-1" role="dialog3"
            aria-labelledby="exampleModalCenterTitle" aria-hidden="true" style="font-family: 'Montserrat', sans-serif;">
            <div class="modal-dialog modal-dialog-centered" role="document">
                <div class="modal-content">
                    <div class="modal-header">
                        <!-- <h5 class="modal-title" id="exampleModalLongTitle"
                            style="font-family: 'Montserrat', sans-serif;">Move Patient turn</h5> -->
                        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                            <span aria-hidden="true">&times;</span>
                        </button>
                    </div>
                    <div class="modal-body">
                        <button type="button" class="btn btn-primary move-btn">Next Slot</button>
                        <button type="button" class="btn btn-primary move-btn">End of List</button>
                        <button type="button" class="btn btn-primary move-btn" data-toggle="modal"
                            data-target="#exampleModalCenter4">Manual Entry</button>

                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-dismiss="modal"
                            style="font-family: 'Montserrat', sans-serif; font-size: 13px;">NO</button>
                        <button type="button" class="btn btn-primary" style="font-family: 'Montserrat', sans-serif; font-size: 13px; background: #29abe2 !important;
                        border-color: #29abe2;" data-toggle="modal" data-target="#exampleModalCenter2">YES</button>
                    </div>
                </div>
            </div>
        </div>
        <!-- move btn modal -->

        <!-- move manually modal -->
        <div class="modal fade" id="exampleModalCenter4" tabindex="-1" role="dialog4"
            aria-labelledby="exampleModalCenterTitle" aria-hidden="true" style="font-family: 'Montserrat', sans-serif;">
            <div class="modal-dialog modal-dialog-centered" role="document">
                <div class="modal-content">
                    <div class="modal-header">
                        <!-- <h5 class="modal-title" id="exampleModalLongTitle"
                            style="font-family: 'Montserrat', sans-serif;">Move Patient turn</h5> -->
                        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                            <span aria-hidden="true">&times;</span>
                        </button>
                    </div>
                    <div class="modal-body" style="padding-top: 20px;">
                        <div class="form-row justify-content-center">
                            <div class="form-group col-md-5">
                                <label for="inputCity"
                                    style="margin-top: 8px; font-family: 'Montserrat', sans-serif;">Move Jane Doe to
                                    slot #</label>
                            </div>
                            <div class="form-group col-md-3">
                                <select id="inputState" class="form-control">
                                    <option selected value="1">1</option>
                                    <option value="2">2</option>
                                    <option value="3">3</option>
                                    <option value="4">4</option>
                                    <option value="5">5</option>
                                    <option value="6">6</option>
                                    <option value="7">7</option>
                                    <option value="8">8</option>
                                    <option value="9">9</option>
                                    <option value="10">10</option>
                                    <option value="11">11</option>
                                    <option value="12">12</option>
                                    <option value="13">13</option>
                                    <option value="14">14</option>
                                    <option value="15">15</option>
                                    <option value="16">16</option>
                                    <option value="17">17</option>
                                    <option value="18">18</option>
                                    <option value="19">19</option>
                                    <option value="20">20</option>
                                </select>
                            </div>
                        </div>
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-dismiss="modal"
                            style="font-family: 'Montserrat', sans-serif; font-size: 13px;">NO</button>
                        <button type="button" class="btn btn-primary" style="font-family: 'Montserrat', sans-serif; font-size: 13px; background: #29abe2 !important;
                        border-color: #29abe2;" data-toggle="modal" data-target="#exampleModalCenter5">YES</button>
                    </div>
                </div>
            </div>
        </div>
        <!-- move manually modal -->

        <!-- move manually modal -->
        <div class="modal fade" id="exampleModalCenter5" tabindex="-1" role="dialog5"
            aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
            <div class="modal-dialog modal-dialog-centered" role="document">
                <div class="modal-content">
                    <div class="modal-header">
                        <!-- <h5 class="modal-title" id="exampleModalLongTitle"
                            style="font-family: 'Montserrat', sans-serif;">Move Patient turn</h5> -->
                        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                            <span aria-hidden="true">&times;</span>
                        </button>
                    </div>
                    <div class="modal-body" style="padding-top: 20px;">
                        Are you sure you want to move Jane doe to slot #15?
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-dismiss="modal"
                            style="font-family: 'Montserrat', sans-serif; font-size: 13px;">NO</button>
                        <button type="button" class="btn btn-primary" style="font-family: 'Montserrat', sans-serif; font-size: 13px; background: #29abe2 !important;
                        border-color: #29abe2;" data-toggle="modal" data-target="#exampleModalCenter5">YES,
                            MOVE</button>
                    </div>
                </div>
            </div>
        </div>
        <!-- move manually modal -->

        <!-- cancel btn modal -->
        <div class="modal fade" id="exampleModalCenter6" tabindex="-1" role="dialog6"
            aria-labelledby="exampleModalCenterTitle" aria-hidden="true" style="font-family: 'Montserrat', sans-serif;">
            <div class="modal-dialog modal-dialog-centered" role="document">
                <div class="modal-content">
                    <div class="modal-header">
                        <!-- <h5 class="modal-title" id="exampleModalLongTitle"
                            style="font-family: 'Montserrat', sans-serif;">Move Patient turn</h5> -->
                        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                            <span aria-hidden="true">&times;</span>
                        </button>
                    </div>
                    <div class="modal-body" style="padding-top: 20px;">
                        Are you sure you would like to cancel Jane Doe's appointment?
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-dismiss="modal"
                            style="font-family: 'Montserrat', sans-serif; font-size: 13px;">NO</button>
                        <button type="button" class="btn btn-primary" style="font-family: 'Montserrat', sans-serif; font-size: 13px; background: #29abe2 !important;
                        border-color: #29abe2;">YES,
                            CANCEL</button>
                    </div>
                </div>
            </div>
        </div>
        <!-- cancel btn modal -->


        <!-- complet turn btn modal -->
        <div class="modal fade" id="exampleModalCenter7" tabindex="-1" role="dialog7"
            aria-labelledby="exampleModalCenterTitle" aria-hidden="true" style="font-family: 'Montserrat', sans-serif;">
            <div class="modal-dialog modal-dialog-centered" role="document">
                <div class="modal-content">
                    <div class="modal-header">
                        <!-- <h5 class="modal-title" id="exampleModalLongTitle"
                            style="font-family: 'Montserrat', sans-serif;">Move Patient turn</h5> -->
                        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                            <span aria-hidden="true">&times;</span>
                        </button>
                    </div>
                    <div class="modal-body" style="padding-top: 20px;">
                        Jane Doe's appointment has been completed. Thank you!</div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-dismiss="modal"
                            style="font-family: 'Montserrat', sans-serif; font-size: 13px;">CLOSE</button>
                    </div>
                </div>
            </div>
        </div>
        <!-- complet turn btn modal -->

        <!-- modal waitlist setting -->
        <div class="modal fade bd-example-modal-lg" tabindex="-1" role="dialog" aria-labelledby="myLargeModalLabel"
            aria-hidden="true" style="font-family: 'Montserrat', sans-serif;">
            <div class="modal-dialog modal-lg">
                <div class="modal-content">
                    <div class="modal-header">
                        <h5 class="modal-title" id="exampleModalLabel" style="font-family: 'Montserrat', sans-serif;">
                            Waitlist setting</h5>
                        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                            <span aria-hidden="true">&times;</span>
                        </button>
                    </div>
                    <div class="modal-body">
                        <div class="form-group">
                            <select style="font-family: 'Montserrat', sans-serif; font-size: 15px;" class="form-control"
                                id="exampleFormControlSelect1">
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
                                        <button type="button" class="btn btn-primary delete-btn">Monday</button>
                                    </div>
                                    <div class="day-container">
                                        <button type="button" class="btn btn-primary delete-btn">Tuesday</button>
                                    </div>
                                    <div class="day-container">
                                        <button type="button" class="btn btn-primary delete-btn">Wednesday</button>
                                    </div>
                                    <div class="day-container">
                                        <button type="button" class="btn btn-primary delete-btn">Thursday</button>
                                    </div>
                                    <div class="day-container">
                                        <button type="button" class="btn btn-primary delete-btn">Friday</button>
                                    </div>
                                    <div class="day-container">
                                        <button type="button" class="btn btn-primary delete-btn">Saturday</button>
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

    .icon-btn {
        width: 30px;
        height: 30px;
        position: absolute;
        right: 170px;
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
        right: 90px;
    }

    .icon-btn4 {
        width: 30px;
        height: 30px;
        position: absolute;
        right: 50px;
        top: 25px;
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
        font-weight: 500;
        font-family: 'Montserrat', sans-serif;

    }

    .dr-icon {
        width: 40px;
        height: 40px;
    }

    .table-btn {
        font-size: 13px;
        /* background-image: linear-gradient(to right top, #93278f, #7c55b7, #5976d1, #3392df, #29abe2) !important; */
        border: none;
        padding: 10px;
        font-weight: 500;
        background: #29abe2 !important;
    }

    .content-table {
        font-size: 13px;
        font-weight: 500;
        padding-top: 20px !important;
        font-family: 'Montserrat', sans-serif;
    }

    .home-icon {
        width: 20px;
        height: 20px;
        margin-right: 10px;
    }

    .add-btn {
        position: absolute;
        right: 25px;
        height: 40px;
        width: 40px;
        border-radius: 50%;
        box-shadow: 0 8px 6px -6px black;
    }

    .move-btn {
        margin: 10px;
        width: 120px;
        font-size: 14px;
        font-family: 'Montserrat', sans-serif;
        background: #29abe2 !important;
        border-color: #29abe2;
        transition: .5s;
    }

    .move-btn:hover {
        background: #2492c2 !important;
        border-color: #2492c2;
    }

    .spot-dropdown {
        width: 60px;
        border: none;
        border-radius: 0;
        border-bottom: 1px solid grey;
    }

    .modal {
        font-family: 'Montserrat', sans-serif !important;
    }

    .settings {
        position: absolute;
        right: 80px;
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
</style>