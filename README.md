

# Hospital CMS System OOP Outline
- [C++ Boilerplate Code](https://github.com/Tarleton-Computer-Society/hospital-cms-cpp-boilerplate)
- [Python BoilerPlate Code](https://github.com/Tarleton-Computer-Society/hospital-cms-python-boilterplate)
- [Java BoilerPlate Code](https://github.com/Tarleton-Computer-Society/hospital-cms-java-boilterplate)
## GUI Client:
The GUI client will be built using a GUI framework such as Java Swing, PyQt, or Tkinter. The client will include the following features:

- Login TAB: A screen where users can enter their login credentials to access the system.
- Dashboard page: A screen where users can view their appointments and medical records. The dashboard will include widgets such as calendars and tables to display data.
- Appointments TAB: A screen where users can view and schedule appointments with doctors. The appointments page will include a calendar widget where users can select a date and time for their appointment. Users can also view their past and upcoming appointments.
- Medical records page: A screen where users can view their medical records and add new ones if necessary. Users can view their medical history, diagnoses, medications, and other relevant information.
- Doctors TAB: A screen where users can view information about doctors in the system. Users can view doctors' profiles, specialties, contact information, and availability.
The GUI client will communicate with the HospitalCMS backend using object-oriented programming (OOP) concepts. The backend will include classes and objects such as Patient, Doctor, Appointment, and MedicalRecord. The GUI client will access these objects and methods directly to retrieve and manipulate data.

For example, to display a list of patients on the dashboard, the GUI client will create an instance of the HospitalCMS class and call the get_patients() method. The method will return a list of Patient objects, which the client can display using a table widget.

To schedule an appointment, the GUI client will create a new Appointment object and pass it to the add_appointment() method of the HospitalCMS class. The method will add the appointment to the backend, which the GUI client can then display on the appointments page.
## Classes and Objects
### Patient
#### Attributes:
- name: string
- age: integer
- gender: string
- contact_info: string
#### Methods:
- get_name(): returns the patient's name
- get_age(): returns the patient's age
- get_gender(): returns the patient's gender
- get_contact_info(): returns the patient's contact information


### Doctor
#### Attributes:
- name: string
- speciality: string
- contact_info: string
#### Methods:
- get_name(): returns the doctor's name
- get_speciality(): returns the doctor's speciality
- get_contact_info(): returns the doctor's contact information

### Appointment
#### Attributes:
- patient: Patient
- doctor: Doctor
- date: date
- time: time
#### Methods:
- get_patient(): returns the patient associated with the appointment
- get_doctor(): returns the doctor associated with the appointment
- get_date(): returns the date of the appointment
- get_time(): returns the time of the appointment


### MedicalRecord
#### Attributes:
- patient: Patient
- doctor: Doctor
- diagnosis: string
- medication: string
#### Methods:
- get_patient(): returns the patient associated with the medical record
- get_doctor(): returns the doctor associated with the medical record
- get_diagnosis(): returns the diagnosis
- get_medication(): returns the medication prescribed

### HospitalCMS
#### Attributes:
- patients: list of Patient
- doctors: list of Doctor
- appointments: list of Appointment
- medical_records: list of MedicalRecord
#### Methods:
- add_patient(patient: Patient): adds a new patient to the system
- add_doctor(doctor: Doctor): adds a new doctor to the system
- add_appointment(appointment: Appointment): adds a new appointment to the system
- add_medical_record(medical_record: MedicalRecord): adds a new medical record to the system
- get_patients(): returns the list of patients in the system
- get_doctors(): returns the list of doctors in the system
- get_appointments(): returns the list of appointments in the system
- get_medical_records(): returns the list of medical records in the system
