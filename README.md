# Hospital CMS System Outline
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
