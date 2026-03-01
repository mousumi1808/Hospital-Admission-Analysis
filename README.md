
Problem Statement:
Analyze hospital admission data at Novartis to identify factors driving high patient readmission rates and provide insights to improve care quality while reducing unnecessary healthcare costs.

Steps:
- Investigated re-admission patterns and operational metrics.
- Identified trends for better hospital resource planning.
- Tools Used: Python, Data Visualization

Key Insights & Conclusion:
- Readmission rate is high for 70-80 yrs old.
- Pediatrics-Pulmonology,PhysicalMedicineandRehabilitation,OutreachServices,Pathology,Psychiatry-Addictive has longest avg days Pediatrics-EmergencyMedicine, Anesthesiology-Pediatric,
  Anesthesiology, Speech, DCPTEAM has shortest avg days.
- 40% of patients re admitted in 30 days.
- patients having changed their diabetic medication are more prone to re admission.
- Cacausian & AfricanAmerican showing higher admission rate both for male & female indicating poor healthcare facilities or poor health in general due to which either they are not able to    recover or fall sick frequently.
- Patients weighing between 75-100 kg are getting readmitted is more than any other category.
- Encounters involving higher medication counts tend to have longer stays. Additionally, readmitted patients consistently exhibit longer lengths of stay for comparable medication levels, indicating greater clinical complexity. This suggests that medication volume can serve as an important predictor of both prolonged hospitalization and readmission risk.

Challenges Faced :
- Missing values and inconsistent patient records required careful cleaning.
- Medical variables showed skewed distributions, complicating direct statistical interpretation.
- Identifying meaningful drivers of readmission required combining clinical and demographic features.
- Translating analytical results into actionable healthcare recommendations required domain-aware reasoning.

Sql code :
--create database hospitaladmission

create table hospitaladmissionanalysis(patient_id varchar(20),
        index1 varchar(20),
        encounter_id varchar(20),
        race varchar(20),
        gender varchar(20),
        age smallint,
        weight1 varchar(20),
        time_in_hospital smallint,
        medical_specialty varchar(20),
        num_lab_procedures smallint,
        num_procedures smallint,
        num_medications smallint,
        number_outpatient smallint,
        number_emergency smallint,
        number_inpatient smallint,
        
        diag_1 float,
        diag_2 float,
        diag_3 float,
        diag_4 float,
        diag_5 float,
        number_diagnoses smallint,
        X1 varchar(20),
		X2 varchar(20),
		X3 varchar(20),
		X4 varchar(20),
		X5 varchar(20),
       X6 varchar(20),
	   X7 varchar(20),
	   X8 varchar(20),
	   X9 varchar(20),
	   X10 varchar(20),
	   X11 varchar(20),
	   X12 varchar(20),
	   X13 varchar(20),
	   X14 varchar(20),
	   X15 varchar(20),
	   X16 varchar(20),
       X17 varchar(20),
	   X18 varchar(20),
	   X19 varchar(20),
	   X20 varchar(20),
	   X21 varchar(20),
	   X22 varchar(20),
	   X23 varchar(20),
	   X24 varchar(20),
	   X25 varchar(20),
	   change1 varchar(20),
       diabetesMed varchar(20),
	   readmitted smallint,
       comorbidity_score float
)

Detailed analysis in  code attached in the folder.

 Skills Demonstrated

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- Data Visualization
- Business Insight Generation
- power bi Dashboard Development
- sql server
- Problem Solving

Recommendation :
Patient Care Improvement
- Implement post-discharge follow-up programs for high-risk patients.
- Provide personalized care plans for patients with repeated admissions.
- Strengthen discharge readiness assessments.

Operational Strategy :

- Prioritize resources for patients with extended hospital stays.
- Improve coordination between inpatient and outpatient care teams.
- Introduce early intervention programs for vulnerable age groups.

Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
