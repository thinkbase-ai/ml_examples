
# The Cleveland Heart disease dataset

Much Coronary heart disease (CHD) involves the reduction of blood flow to the heart muscle due to build-up of plaque in the arteries of the heart. It is the most common form of cardiovascular disease. Currently, invasive coronary angiography represents the gold standard for establishing the presence, location, and severity of CAD, however this diagnostic method is costly and associated with morbidity and mortality in CAD patients. Therefore, it would be beneficial to develop a non-invasive alternative to replace the current gold standard.

Other less invasive diagnostics methods have been proposed in the scientific literature including exercise electrocardiogram, thallium scintigraphy and fluoroscopy of coronary calcification. However the diagnostic accuracy of these tests only ranges between 35%-75%. Therefore, it would be beneficial to develop a computer aided diagnostic tool that could utilize the combined results of these non-invasive tests in conjunction with other patient attributes to boost the diagnostic power of these non-invasive methods with the aim ultimately replacing the current invasive gold standard.

IThe included dataset comprises 303 observations, 13 features and 1 target attribute. The 13 features include the results of the aforementioned non-invasive diagnostic tests along with other relevant patient information. The target variable includes the result of the invasive coronary angiogram which represents the presence or absence of coronary artery disease in the patient with 0 representing absence of CHD and labels 1-4 representing presence of CHD. Most research using this dataset have concentrated on simply attempting to distinguish presence (values 1,2,3,4) from absence (value
0).

The data was collected by Robert Detrano, M.D., Ph.D of the Cleveland Clinic Foundation. 

## Attribute information: 
1. age: age in years
2. sex: 1 = male; 0 = female
3. cp: chest pain type
- Value 1: typical angina
- Value 2: atypical angina
- Value 3: non-anginal pain
- Value 4: asymptomatic
4. trestbps: resting blood pressure (in mm Hg on admission to the hospital)
5. chol: serum cholesterols in mg/dl
6. fbs: fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
7. restecg: resting electrocardiographic results
- Value 0: normal
- Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
- Value 2: showing probable or definite left ventricular hypertrophy by Estes’ criteria
8. thalach: maximum heart rate achieved
9. exang: exercise induced angina (1 = yes; 0 = no)
10. oldpeak: ST depression induced by exercise relative to rest
11. slope: the slope of the peak exercise ST segment
- Value 1: upsloping
- Value 2: flat
- Value 3: Downsloping
12. ca: number of major vessels (0–3) colored by fluoroscopy
13. thal: 3 = normal; 6 = fixed defect; 7 = reversible defect

## The target
The target variable, labelled in this data set as _outcome_ has the results of this invasive procedure to determine arterial narrowing.
0 is no narrowing, and 1,2,3 are various degrees of narrowing.


__Note__: "age" is a reserved word in darl, so the name of the input has been changed to "_age".
