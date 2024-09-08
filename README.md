# Hospital-guide
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hospital Management System</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container" id="login-page">
    <h2>Hospital Management System</h2>
    <input type="text" id="aadhar" placeholder="Enter Aadhar Number" />
    <button onclick="login()">Login</button>
  </div>

  <div class="container" id="user-options" style="display:none;">
    <button onclick="showAdminPage()">Administrator Login</button>
    <button onclick="showDoctorPage()">Doctor Login</button>
    <button onclick="showPatientPage()">Patient Login</button>
    <button onclick="goBack()">Back</button>
  </div>

  <div class="container" id="admin-page" style="display:none;">
    <h3>Administrator Panel</h3>
    <button onclick="showAddEmployee()">Add Employees</button>
    <button onclick="manageMedicines()">Manage Medicines</button>
    <button onclick="manageMachinery()">Manage Machinery</button>
    <button onclick="goBackToOptions()">Back</button>
  </div>

  <div class="container" id="doctor-page" style="display:none;">
    <h3>Doctor Panel</h3>
    <input type="text" id="doctor-username" placeholder="Enter Username">
    <button onclick="viewAppointments()">View Appointments</button>
    <button onclick="viewPatientReports()">View Patient Reports</button>
    <button onclick="contactMedicalShop()">Contact Medical Shop</button>
    <button onclick="goBackToOptions()">Back</button>
  </div>

  <div class="container" id="patient-page" style="display:none;">
    <h3>Patient Panel</h3>
    <button onclick="viewDoctorAppointments()">View Doctor Appointment List</button>
    <button onclick="showEmergencyOptions()">Emergency</button>
    <button onclick="goBackToOptions()">Back</button>
  </div>

  <div class="container" id="emergency-page" style="display:none;">
    <h3>Emergency Options</h3>
    <button onclick="showNearbyHospitals()">Nearby Hospitals</button>
    <button onclick="showAmbulanceNumbers()">Nearby Ambulance Numbers</button>
    <button onclick="showEmergencyTips()">Emergency Tips & Tricks</button>
    <button onclick="goBackToPatient()">Back</button>
  </div>

  <script src="script.js"></script>
</body>

</html>
