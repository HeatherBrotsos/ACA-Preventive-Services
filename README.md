
## ACA Preventive Services ##

_currently work in progress_

As part of the Affordable Care Act (ACA), private plans must cover a set of preventive services with no patient [cost sharing](https://www.healthcare.gov/glossary/cost-sharing/).  

These services are outlined [here](https://www.healthcare.gov/preventive-care-benefits/) by HHS. 

Three organizations contributed recommendations on what services to include:  
- [U.S. Preventive Services Task Force (USPSTF)](http://www.uspreventiveservicestaskforce.org/Page/Name/uspstf-a-and-b-recommendations/)  
-  [Health Resources Services Administration](http://www.hrsa.gov/womensguidelines/)  
-  [Advisory Committee for Immunization Practices](http://www.cdc.gov/vaccines/hcp/acip-recs/index.html)

Additional description of these services, including effective dates, other restrictions and background is documented by the [Kaiser Family Foundation](http://kff.org/health-reform/fact-sheet/preventive-services-covered-by-private-health-plans/?utm_campaign=KFF%3A+The+Latest&utm_source=hs_email&utm_medium=email&utm_content=21094055&_hsenc=p2ANqtz--zIJs8wbq4DTDh07BVoNAizYbQMiW43pZk7mO4pVSEjJGJhH5W4X9rTlX9UP5-GL8dVrRAXIj_8lezzzPIqS1kloaGF44LvxCoR3yIQ_y0z8dR1Xk&_hsmi=21094055). USPSTF published The Guide to Clinical  Preventive Services, available [here](http://www.uspreventiveservicestaskforce.org/Page/Name/tools-and-resources-for-better-preventive-care). 


### What procedure codes correspond to these services? ###

An initial search for this information began with the HHS Innovation Lab [Demand Driven Open Data project](https://github.com/demand-driven-open-data/ddod-intake/issues/44).


While there is no official guidance, CDC published a list of procedure and diagnostic codes that align with these services [here](http://www.cdc.gov/prevention/billingcodes.html).  This project transforms the information provided into two machine-readable data set ready for analysis:  
1. **ICD-9 diagnosis codes** that correspond to each preventive service and qualify certain circumstances under which a service is provided with no patient cost sharing.  
2. **Procedure codes** that correspond to each service, along with the effective service date and other restrictions that may need to be considered.


A high level description of the process to create these files follows.

**Step 1**: Convert the CDC html into a non-normalized [.csv  file](data/ACA_Preventive_Services_CDC_Copy.csv).



**Step 2**: Transform into tabular format.


**Step 3**: Add relevant restrictions and date each service is effective.

Additional description is located [here](https://github.com/HeatherBrotsos/ACA-Preventive-Services/blob/master/Method%20Details.md).
