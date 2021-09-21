# Medical_Analytics_Group_Operational_Data_Challenge

Operational data challenge
We would like to invite all interested in machine learning and operational research to explore our operational dataset. You can download it from here:

Data only (zipped Excel file, 53MB)
Code and data (zipped code and Excel file, 63MB)
This data, describing patient waits in a hospital, was built for the following challenges (see our recent publication here: https://rdcu.be/b4ffC):

Predict patient wait times from the other operational features, as accurately as possible
Identify the smallest subset of features, sufficient for accurate wait time prediction across all four facilities in the dataset. The smallest model MAE should be at most 1-2 minutes worse compared to the best full model MAE
Invent (engineer) new features significantly improving model prediction quality
Overall, reducing MAE by more than 70% in comparison with the simple intercept model (predicting wait from its overall average) would be a significant step forward.

Data description
Our dataset represents operational features, captured in four different hospital facilities, processing walk-in (F4) or scheduled (F1, F2, F3) patients. Approximately 600 to 1000 days of full  patient flow data were extracted from each facility. The target variable to be predicted is Wait. The other variables represent different features of the patient flow, captured at the time of patient arrivals and departure (one line per each patient visit event). Data Excel file contains the exact definitions of all features used (see Contents sheet).

This data was extracted from the real hospital information system. Therefore it was anonymized and aggregated to remove any confidential information. In particular, x_ArrivalDTTM, x_ScheduledDTTM, and x_BeginDTTM timestamps were anonymized, and set to the fictitious future dates (to make you aware of this modification). Only their relative timing was preserved. As a result, these timestamps can be used only for sorting, to reflect the correct order of feature events, but nothing else.

Code
We include our Matlab code used to process this data here – feel free to download and experiment.
