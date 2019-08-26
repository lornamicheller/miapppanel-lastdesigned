<template>
    <div>
        <div class="container-fluid" style="padding: 0; margin: 0; height: 100%; overflow: hidden;">
            <div class="row">
                <div class="col-3" style="background: #212121 !important; height: auto; padding: 0; padding-top: 70px;">
                    <!-- <img src="../assets/logomiapplogin.png" class="logo"> -->
                    <nav class="nav flex-column" style="  overflow: hidden; position: fixed; left: 0;">
                        <router-link class="nav-link" to="/home2"><img src="../assets/home.png" class="home-icon">Home
                        </router-link>
                        <router-link class="nav-link" to="/instructions"><img src="../assets/instruction.png"
                                class="home-icon">Instructions</router-link>
                        <router-link class="nav-link" style="color: #29abe2 !important;" to="/profile"><img
                                src="../assets/profile.png" class="home-icon">Profile</router-link>
                        <router-link class="nav-link" to="/calendar"><img src="../assets/calendar.png"
                                class="home-icon">Calendar</router-link>
                        <router-link class="nav-link" to="/Statistics"><img src="../assets/grafica.png"
                                class="home-icon">Appointment
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

                        <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
                            <!-- <img class="icon-btn" src="../assets/block.png">
                            <img class="icon-btn2" src="../assets/leyend.png">
                            <img class="icon-btn3" src="../assets/plus.png"> -->
                            <div class="card profile-btn" style="width: 18rem;">
                                <img class="dropdown-img" src="../assets/doc.jpg">
                                <p class="dr-name">John Doe</p>
                            </div>
                            <router-link to="#"><img class="icon-btn4" src="../assets/logout.png"></router-link>
                        </div>
                    </nav>

                    <div class="container-fluid" style="overflow: scroll; height: auto;">
                        <img src="../assets/doctor2.png" class="profile-pic">

                        <router-link to="#" style="text-decoration: none;">
                            <h1 class="upload">Upload Picture<i class="fas fa-arrow-alt-circle-down"
                                    style="margin-left: 10px; font-size: 20px;"></i></h1>
                        </router-link>

                        <div class="row justify-content-center mt-3">
                            <div class="col-3">
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
                            <div class="col-3">
                                <div class="input-group mb-2">
                                    <input type="text" class="form-control" id="inlineFormInputGroup"
                                        placeholder="Last Name"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                </div>
                            </div>
                        </div>

                        <div class="row justify-content-center mt-1">
                            <div class="col-6">
                                <div class="input-group mb-3">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="fas fa-venus-mars input-icon"></i>
                                        </div>
                                    </div>
                                    <select class="custom-select" id="inputGroupSelect01"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                        <option selected>Gender</option>
                                        <option value="female">Female</option>
                                        <option value="male">Male</option>
                                        <option value="other">Other</option>
                                        <option value="undisclosed">Undisclosed</option>
                                    </select>
                                </div>
                            </div>
                        </div>

                        <div class="row justify-content-center mt-1">
                            <div class="col-6">
                                <div class="input-group mb-3">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="fas fa-comment-medical input-icon"></i>
                                        </div>
                                    </div>
                                    <select class="custom-select" id="inputGroupSelect01"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                        <option selected>Specialty</option>
                                        <option value="Acupuncture">Acupuncture</option>
                                        <option value="Allergy">Allergy</option>
                                        <option value="Allergy and Immunology">Allergy and Immunology</option>
                                        <option value="Anesthesia">Anesthesia</option>
                                        <option value="Audiology">Audiology</option>
                                        <option value="Back Surgery">Back Surgery</option>
                                        <option value="Burns Surgery">Burns Surgery</option>
                                        <option value="Cardiology">Cardiology</option>
                                        <option value="Chiropractic">Chiropractic</option>
                                        <option value="Critical Care Medicine">Critical Care Medicine</option>
                                        <option value="Dentist">Dentist</option>
                                        <option value="Dermatology">Dermatology</option>
                                        <option value="Ear Nose and Throat">Ear Nose and Throat</option>
                                        <option value="Endocrinology">Endocrinology</option>
                                        <option value="Endodontics">Endodontics</option>
                                        <option value="Family Medicine">Family Medicine</option>
                                        <option value="Gastroenterology">Gastroenterology</option>
                                        <option value="General Medicine">General Medicine</option>
                                        <option value="General Practitioner">General Practitioner</option>
                                        <option value="General Surgery">General Surgery</option>
                                        <option value="Geriatric Psychiatrics">Geriatric Psychiatrics</option>
                                        <option value="Geriatrics">Geriatrics</option>
                                        <option value="Glaucoma">Glaucoma</option>
                                        <option value="Gynecology">Gynecology</option>
                                        <option value="Hands Plastic Surgery">Hands Plastic Surgery</option>
                                        <option value="Head and Neck Surgery">Head and Neck Surgery</option>
                                        <option value="Hematology">Hematology</option>
                                        <option value="Internal Medicine">Internal Medicine</option>
                                        <option value="Interventional Cardiology">Interventional Cardiology</option>
                                        <option value="Laboratories">Laboratories</option>
                                        <option value="Maxilofacial">Maxilofacial</option>
                                        <option value="Mohs Micrographic Surgery">Mohs Micrographic Surgery</option>
                                        <option value="Neonatal and Perinatal Medicine">Neonatal and Perinatal Medicine
                                        </option>
                                        <option value="Nephrology">Nephrology</option>
                                        <option value="Neurology">Neurology</option>
                                        <option value="Neuroophthamology">Neuroophthamology</option>
                                        <option value="Neurophysiology">Neurophysiology</option>
                                        <option value="Neurosurgery">Neurosurgery</option>
                                        <option value="Nuclear Medicine">Nuclear Medicine</option>
                                        <option value="Obstetric and gynecology">Obstetric and Gynecology</option>
                                        <option value="Occupational Medicine">Occupational Medicine</option>
                                        <option value="Oncologic Gynecology">Oncologic Gynecology</option>
                                        <option value="Oncological Surgery">Oncological Surgery</option>
                                        <option value="Oncology">Oncology</option>
                                        <option value="Oncology Hematology">Oncology Hematology</option>
                                        <option value="Ophthalmology">Ophthalmology</option>
                                        <option value="Optometry">Optometry</option>
                                        <option value="Orthodontics">Orthodontics</option>
                                        <option value="Orthopedic Surgery">Orthopedic Surgery</option>
                                        <option value="Orthopedics">Orthopedics</option>
                                        <option value="Pain Management">Pain Management</option>
                                        <option value="Pediatric Allergy and Immunology">Pediatric Allergy and
                                            Immunology</option>
                                        <option value="Pediatric Cardiology">Pediatric Cardiology</option>
                                        <option value="Pediatric Critical Care">Pediatric Critical Care</option>
                                        <option value="Pediatric Dentist">Pediatric Dentist</option>
                                        <option value="Pediatric Endocrinology">Pediatric Endocrinology</option>
                                        <option value="Pediatric Gastroenterology">Pediatric Gastroenterology</option>
                                        <option value="Pediatric Hematology and Oncology">Pediatric Hematology and
                                            Oncology</option>
                                        <option value="Pediatric Neurology">Pediatric Neurology</option>
                                        <option value="Pediatric Odontology">Pediatric Odontology</option>
                                        <option value="Pediatric Orthopedics">Pediatric Orthopedics</option>
                                        <option value="Pediatric Physiatry">Pediatric Physiatry</option>
                                        <option value="Pediatric Pneumology">Pediatric Pneumology</option>
                                        <option value="Pediatric Psychiatrics">Pediatric Psychiatrics</option>
                                        <option value="Pediatric Surgery">Pediatric Surgery</option>
                                        <option value="Pediatric Urology">Pediatric Urology</option>
                                        <option value="Pediatry">Pediatry</option>
                                        <option value="Periodontics">Periodontics</option>
                                        <option value="Physiatry">Physiatry</option>
                                        <option value="Physical Therapy">Physical Therapy</option>
                                        <option value="Plastic Surgery">Plastic Surgery</option>
                                        <option value="Pneumology">Pneumology</option>
                                        <option value="Podiatrics">Podiatrics</option>
                                        <option value="Proctology">Proctology</option>
                                        <option value="Prosthodontics">Prosthodontics</option>
                                        <option value="Psychiatricn">Psychiatric</option>
                                        <option value="Psychology">Psychology</option>
                                        <option value="Radiology">Radiology</option>
                                        <option value="Retinology">Retinology</option>
                                        <option value="Spinal Cord Psychiatry and Rehabilitation">Spinal Cord Psychiatry
                                            and Rehabilitation</option>
                                        <option value="Sports Medicine">Sports Medicine</option>
                                        <option value="Surgery or Peripheral Vascular Illness">Surgery or Peripheral
                                            Vascular Illness</option>
                                        <option value="Thoracic Surgery">Thoracic Surgery</option>
                                        <option value="Urology">Urology</option>
                                    </select>
                                </div>
                            </div>
                        </div>
                        <div class="row justify-content-center mt3">
                            <div class="col-6">
                                <div class="input-group mb-2">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="fas fa-map-marker-alt"></i>
                                        </div>
                                    </div>
                                    <input type="text" class="form-control" id="inlineFormInputGroup"
                                        placeholder="Office Address"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                </div>
                            </div>
                        </div>
                        <div class="row justify-content-center mt-3">
                            <div class="col-6">
                                <div class="input-group mb-2">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="fas fa-phone"></i>
                                        </div>
                                    </div>
                                    <input type="tel" class="form-control" id="inlineFormInputGroup"
                                        placeholder="Office Phone"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                </div>
                            </div>
                        </div>
                        <div class="row justify-content-center mt-3">
                            <div class="col-6">
                                <div class="input-group mb-2">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="fas fa-fax"></i>
                                        </div>
                                    </div>
                                    <input type="tel" class="form-control" id="inlineFormInputGroup"
                                        placeholder="Office Fax"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                </div>
                            </div>
                        </div>
                        <div class="row justify-content-center mt-3">
                            <div class="col-6">
                                <div class="input-group mb-2">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="fas fa-envelope"></i>
                                        </div>
                                    </div>
                                    <input type="tel" class="form-control" id="inlineFormInputGroup"
                                        placeholder="Office Email"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                </div>
                            </div>
                        </div>

                        <div class="row justify-content-center mt-1">
                            <div class="col-6">
                                <div class="input-group mb-3">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="far fa-credit-card input-card"></i>
                                        </div>
                                    </div>
                                    <select class="custom-select" id="inputGroupSelect01"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                        <option selected>Accepted Insurance Providers</option>
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
                            <div class="col-6">
                                <div class="input-group mb-3">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="fas fa-calendar-check"></i>
                                        </div>
                                    </div>
                                    <select class="custom-select" id="inputGroupSelect01"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                        <option selected>Appointment Method</option>
                                        <option value="No Appointments (Patients are seen in the order of arrival.)">No
                                            Appointments (Patients are seen in the order of arrival.)</option>
                                        <option
                                            value="Block Appointments (Patients are seen in the order of arrival within their designated time block.)">
                                            Block Appointments (Patients are seen in the order of arrival within their
                                            designated time block.)</option>
                                        <option
                                            value="Individual Appointments (Patients are seen at the time of their scheduled appointment regardless of earlier arrival of other patients.)">
                                            Individual Appointments (Patients are seen at the time of their scheduled
                                            appointment regardless of earlier arrival of other patients.)</option>
                                    </select>
                                </div>
                            </div>
                        </div>

                        <div class="container">
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
                                        <option selected>0:00AM</option>
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
                                    </select>

                                    <!-- Monday Input -->
                                    <select class="form-control start-schedule" placeholder="0:00AM">
                                        <option selected>0:00AM</option>
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
                                    </select>

                                    <!--Tuesday Input -->

                                    <select class="form-control start-schedule" placeholder="0:00AM">
                                        <option selected>0:00AM</option>
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
                                    </select>

                                    <!-- Wednesday Input -->

                                    <select class="form-control start-schedule" placeholder="0:00AM">
                                        <option selected>0:00AM</option>
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
                                    </select>

                                    <!-- Thursday Input -->

                                    <select class="form-control start-schedule" placeholder="0:00AM">
                                        <option selected>0:00AM</option>
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
                                    </select>

                                    <!-- Friday Input -->

                                    <select class="form-control start-schedule" placeholder="0:00AM">
                                        <option selected>0:00AM</option>
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
                                    </select>

                                    <!-- Saturday Input -->

                                    <select class="form-control start-schedule" placeholder="0:00AM">
                                        <option selected>0:00AM</option>
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
                                    </select>
                                </div>
                                <div class="col-lg-2 col-md-2 col-sm-12">
                                    <h1 class="title-schedule">Close</h1>

                                    <!-- Sunday Input -->
                                    <select class="form-control start-schedule" placeholder="0:00PM">
                                        <option selected>0:00AM</option>
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
                                        <option selected>0:00AM</option>
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
                                        <option selected>0:00AM</option>
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
                                        <option selected>0:00AM</option>
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
                                        <option selected>0:00AM</option>
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
                                        <option selected>0:00AM</option>
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
                                        <option selected>0:00AM</option>
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

                        <div class="row justify-content-center mt-1">
                            <div class="col-6">
                                <div class="input-group mb-3">
                                    <div class="input-group-prepend">
                                        <div class="input-group-text"
                                            style="background: transparent; border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                            <i class="fas fa-history input-card"></i>
                                        </div>
                                    </div>
                                    <select class="custom-select" id="inputGroupSelect01"
                                        style="border: 0; border-radius: 0; border-bottom: 1px solid grey;">
                                        <option selected>Estimated Time Per Patient</option>
                                        <option value="5 Minutes">5 Minutes</option>
                                        <option value="10 Minutes">10 Minutes</option>
                                        <option value="15 Minutes">15 Minutes</option>
                                        <option value="20 Minutes">20 Minutes</option>
                                        <option value="25 Minutes">25 Minutes</option>
                                        <option value="30 Minutes">30 Minutes</option>
                                        <option value="45 Minutes">45 Minutes</option>
                                        <option value="1 Hour">1 Hour</option>
                                        <option value="1 Hour 15 Minutes">1 Hour 15 Minutes</option>
                                        <option value="1 Hour 30 Minutes">1 Hour 30 Minutes</option>
                                        <option value="1 Hour 45 Minutes">1 Hour 45 Minutes</option>
                                        <option value="2 Hour">2 Hour</option>
                                        <option value="2 Hour 15 Minutes">2 Hour 15 Minutes</option>
                                        <option value="2 Hour 30 Minutes">2 Hour 30 Minutes</option>
                                        <option value="2 Hour 45 Minutes">2 Hour 45 Minutes</option>
                                        <option value="3 Hour">3 Hour</option>
                                        <option value="3 Hour 15 Minutes">3 Hour 15 Minutes</option>
                                        <option value="3 Hour 30 Minutes">3 Hour 30 Minutes</option>
                                        <option value="3 Hour 45 Minutes">3 Hour 45 Minutes</option>
                                        <option value="4 Hour">4 Hour</option>
                                        <option value="4 Hour 15 Minutes">4 Hour 15 Minutes</option>
                                        <option value="4 Hour 30 Minutes">4 Hour 30 Minutes</option>
                                        <option value="4 Hour 45 Minutes">4 Hour 45 Minutes</option>
                                        <option value="5 Hour">5 Hour</option>

                                    </select>
                                </div>
                            </div>
                        </div>

                        <button type="button" class="btn btn-primary save-btn">SAVE</button>


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

<style scoped>
    .navbar,
    .navbar-expand-lg,
    .navbar-light,
    .bg-light {
        background: #1e1e1e !important;
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
        top: 25px;
        position: absolute;
        right: 50px;
        transition: .5s;

    }

    .icon-btn4:hover {
        background: rgba(255, 255, 255, 0.103);
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


    .icon-btn4 {
        width: 30px;
        height: 30px;
        position: absolute;
        right: 50px;
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

    .save-btn {
        background-color: #29abe2 !important;
        border: none;
        margin-top: 30px;
        margin-bottom: 100px;
        width: 200px;
        font-size: 13px;
        font-weight: 500;
        padding: 10px;
        box-shadow: 0 8px 6px -6px black;
    }

    .upload {
        font-size: 15px;
        font-family: "Montserrat", sans-serif;
        font-weight: 600;
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
    }
</style>