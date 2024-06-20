**Hospital Management System**

Hospital Management System using MySQL, Php, and Bootstrap

**Need to work on:**

Ability to accept the appointment by the doctor to acknowledge the patient that their appointment has been approved.
The user should not be allowed to register if he/she tries to provide the already registered email ID.
The password should be encrypted and the password field shouldn't be displayed in the admin panel.
Implementation of pagination for all the list views across the application.
Bug fix - Bill payment receipt contains multiple records if the patient has associated with the same doctor multiple times.
Addition of more fields in the prescription statement to make it a more specific one.
Addition of more details on payment - such as date of the payment made, amount paid, etc.
Implementation of export button in admin module to export all details to an excel sheet.
Prerequisites
Install the XAMPP web server
Any Editor (Preferably VS Code or Sublime Text)
Any web browser with the latest version
Languages and Technologies used
HTML5/CSS3
JavaScript (to create dynamically updating content)
Bootstrap (An HTML, CSS, and JS library)
XAMPP (A web server by Apache Friends)
Php
MySQL (An RDBMS that uses SQL)
TCPDF (to generate PDFs)
Steps to run the project in your machine
Download and install XAMPP in your machine
Clone or download the repository
Extract all the files and move it to the 'htdocs' folder of your XAMPP directory.
Start the Apache and Mysql in your XAMPP control panel.
Open your web browser and type 'localhost/phpmyadmin'
In phpmyadmin page, create a new database from the left panel and name it as 'myhmsdb'
Import the file 'myhmsdb.sql' inside your newly created database and click ok.
Open a new tab and type 'localhost/foldername' in the URL of your browser
Hurray! That's it!
**SOFTWARES USED**
XAMPP was installed on the Ubuntu 19.04 machine and APACHE2 Server and MySQL were initialized. And, files were built inside opt/lampp/htdocs/myhmsp
Sublime Text 3.2 was used as a text editor.
Google Chrome Version 77.0.3865.90 was used to run the project (localhost/myhmsp was used as the URL).
Starting Apache And MySQL in XAMPP:
The XAMPP Control Panel allows you to manually start and stop Apache and MySQL. To start Apache or MySQL manually, click the ‘Start’ button under ‘Actions’.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/a1233974-097f-4436-a748-7db642576dc9)

**GETTING INTO THE PROJECT:**
Hospital Management System in PHP and MySql. This system has a ‘Home’ page from where the patient, doctor & administrator can log in into their accounts by toggling the tabs accordingly. Fig 1.1 shows the ‘Home’ page of our project.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/48869076-51bf-40f0-aa7c-34199863c22a)


'About Us' page (Fig 1.2) allows us to get some more information about the quality and the services of the hospital.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/bee1794d-28d2-4ce9-8c59-25840bd257ad)


The ‘Contact’ page allows users to provide feedback or queries about the services of the hospital. Fig 1.3 shows the ‘Contact’ page.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/d6117155-7d91-4d46-8ff1-104c34d27e02)


The ‘Home’ page consists of 3 modules:

Patient Module
Doctor Module
Admin Module
**Patient Module:**
      This module allows patients to create their account, book an appointment to see a doctor, and see their appointment history. The registration page(on the home page itself) asks patients to enter their First Name, Last Name, Email ID, Contact Number, Password, and radio buttons to select their gender.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/ee654eba-aded-4d67-8181-cffbdeb4dc41)


Once the patient has created his/her own account after clicking the ‘Register’ button, then he will be redirected to his/her Dashboard(Fig 1.5).

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/74aebc61-a029-4dcc-b165-43d902988b68)


**The Dashboard page allows patients to perform two operations:**

1. Book his/her appointment:

      Here, the patients can able to book their appointments to see a doctor. The appointment form(Fig 1.6) requires patients to select the doctor that they want to see, Date and Time that they want to meet with the doctor. The consultancy fee will be shown accordingly to the patient as it was already determined by the doctor.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/a333dffc-fca0-4432-a15d-124e3b54eed2)


After clicking on the ‘Create new entry’ button, the patient will receive an alert that acknowledges the successful appointment of the patient.(See Fig 1.7)

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/820837e0-109a-47eb-a3d4-8f094dcf5867)


2. View patients’ Appointment History:

      Here, the patient can see their appointment history which contains Doctor Name, Consultancy Fee, Appointment Date and Time.(See Fig 1.8).

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/d46c7c37-d7d2-40b5-9940-f293533e0c3d)


Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again. Fig 1.9 shows the login page. Clicking on ‘Login’ button will redirect the patient to his dashboard page which we have seen earlier (Fig 1.5)

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/822f30a2-2e03-4fd8-afa4-81fa8568fc2a)


This is how the patient module works. On the whole, this module allows patients to register their account or login their account(if he/she has one), book an appointment and view his/her appointment history.

**Doctor Module:**
      The doctors can log in to their account which can be done by toggling the tab from ‘Patient’ to ‘Doctor’. Fig 1.10 shows the login form for a doctor. Registration of a doctor account can be done only by admin. We will discuss more about this in the Admin Module.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/e8753dae-3867-484b-b6a9-f8bf26f1652f)


Once the doctor clicks the ‘Login’ button, they will be redirected to their own dashboard which is shown in Fig 1.11

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/182eb4a8-b206-4089-8200-b0ecd3c7512b)


In this page, doctor can able to see their appointments which has been booked by the patients. Fig 1.12 shows the appointment of the doctor ‘Ganesh’ which has been booked by the patient ‘Kenny Sebastian’ (Fig 1.6). This means that the doctor ‘Ganesh’ will have an appointment with the patient ‘Kenny Sebastian’ on 10-10-2019 10 AM.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/7ee586c2-0ab0-4dd1-8783-14b3f3cad2fc)


In real-time, the doctors will have thousands of appointments. It will be easier for a doctor to search for appointments in the case of more appointments. To make it easier, I have a ‘Search’ box in the navigation bar (See Fig 1.12) which allows doctors to search for a patient by their contact number.       Once everything is done, the doctor can log out of their account. Thus, in general, a doctor can log in to his/her account, view their appointments, and search for a patient. This is all about Doctor Module.

**Admin Module:**
      This module is the heart of our project where an admin can see the list of all patients. Doctors and appointments and the feedback/queries received from the ‘Contact’ page. Also, admin can add a doctor too.       Login into the admin account can be done by toggling into the admin tab of the Home page. Fig 1.13 shows the login page for admin.       username: admin, password: admin123

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/9d1b692b-8cff-4e86-9462-045d0b983340)


On clicking the ‘Login’ button, the admin will be redirected to his/her dashboard as shown in Fig 1.14.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/8e4d13a1-33ee-40ec-aca1-5fd799984109)


This module allows the admin to perform five major operations:

**1. View the list of all patients registered:**

      Admin can able to view all the patients registered. This includes the patients’ First Name, Last Name, Email ID, Contact Number and Password. (See Fig 1.15).As like in doctor module, admin can also search for a patient by their contact number in the search box.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/f9e9185f-1844-4c0a-bc1e-45f144155b30)


**2. View the list of all doctors registered:**

      Details of the doctors can also be viewed by the admin. This details include the Name of the doctor, Password, Email and Consultancy fees, shown in Fig 1.16. Searching for a doctor can be done by using the doctor’s Email ID in the search box.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/9543e536-35de-4cfe-9740-9db992390edb)


**3. View the Appointment lists:**

      Admin can also able to see the entire details of the appointment that shows the appointment details of the patients with their respective doctors. This includes the First Name, Last Name, Email and Contact Number of patients, doctor’s name, Appointment Date, Time and the Consultancy Fees. (See Fig 1.17).

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/f4b874c7-8cea-4395-9c33-eb28e62346e2)


**4. Add Doctor:**

      Admin alone can add a new doctor since anyone can register as a doctor if we put this section on the home page. This form asks Doctor’s Name, Email ID, Password and his/her Consultancy Fees.(See Fig 1.18)

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/5d3f6d24-61fa-4c0c-8da5-18fa70675e03)


After adding a new doctor, if we check the doctor’s list, we will see the details of new doctor is added to the list as shown in the Fig 1.19

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/8f583c25-4026-49c1-8609-f8f043a3be83)


**5. View User’s feedback/Queries**:

      Admin is allowed to view the feedback/Query that has been given by the user in the ‘Contact’ page (Refer Fig 1.3). This includes User’s Name, Email Id, Contact Number and the message(Feedback/ Query) as shown in the Fig 1.20.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/53acc7d2-69ea-4da7-a229-dfb50a6c900a)


      Taking everything into consideration, the admin can able to view the details of patients and doctors, appointment details, Feedback by the user and can add a new doctor. Once everything is done, the admin can logout from his account.

**Updates
1. Cancel Appointments**
      Patients and doctors can able to delete their appointments.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/22b2a07b-fe6e-4415-b080-cbd764d20c5b)


If the patient deletes the last record (for doctor Ganesh), then a label "deleted by you" will be displayed in the column 'Current Status' and the action will change to cancel state.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/7617cdb1-456b-445e-950b-c3034db3a928)


Now if we login to the doctor Ganesh's account and view his appointment details, then it will look like this:

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/875e02b1-c6f8-444e-83c7-38fc27cebd7b)


Similarly, doctors can also delete their appointments and patients can view their updated appointment details.

**2. Remove Doctors by Admin**
      Admin can also delete the doctors from the system. This lets the admin to have more control over the system.

![image](https://github.com/Yovi1717/Upskillcampus/assets/128585091/8376b5bc-9829-4c0c-9725-42e2ed0dab81)

