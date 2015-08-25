## Data sets produced in this project ##
1. **ACAPreventiveServicesProc:** itemized list of all procedure codes that correspond to preventive services that qualify as covered with no patient cost sharing under ACA. File includes the following attributes:
	1. **Group:** overarching category of service (e.g., all, children, immunization, conception)
	2.  **Service:** type of service (e.g., wellness examination, cervical cancer, depression)
	3.  **Procedure Code:**  procedure code associated with the service
	4.  **Effective Date:** date that service is eligible for coverage with no patient cost sharing
	5.  **Restrictions:** criteria that define the circumstances under which the service qualifies (e.g. pregnant, age range)    
2.  **ACAPreventiveServicesICD9:** itemized list of all diagnosis codes that define circumstances under which services that qualify as covered with no patient cost sharing under ACA. File includes the following attributes:
	1.  **Group:** overarching category of service (e.g., all, children, immunization, conception)
	2.  **Service:** type of service (e.g., wellness examination, cervical cancer, depression)
	3.  **ICD-9 Code:**  diagnosis code that defines circumstances under which the service that qualifies 
	4.  **Code Description:** description of the diagnosis code

These two files must be used in combination to fully evaluate a service rendered.  For a given service to qualify, both a procedure code and a diagnosis code must be present.  For example, a patient that receives a gestational diabetes screening must meet the following criteria for the service to qualify:  

1. procedure code is included in the list of codes  defined for diabetes screening   


1. patient must be pregnant (gestation >24 weeks), indicated through use of a diagnosis code

## Data used on this project ##
1. List of diagnosis and procedure codes, published by the [CDC](http://www.cdc.gov/prevention/billingcodes.html). 
2. Reference list of ICD-9 and CPT codes to convert ranges to itemized list.

## Limitations and Caveats##
1. Files produced only includes ICD-9 codes. ICD-10 are included in the CDC definitions and may be added at a later point.
2. Coding practices change over time.  Certain codes used in earlier years are no longer used.  For example, CPT code G0450 is not included in the 2015 codes.  As a result, longitudinal analysis may exclude codes that should be included.  
3. There may be other qualifying services, which are not included.  For example, lung cancer screenings are not included in this version.
4. Through the conversion from ranges to itemized list of codes, a risk of error exists due to the structure and organization of the coding hierarchy.  This project seeks to improve the process in an iterative manner over time and encourages suggestions on how to do so.
