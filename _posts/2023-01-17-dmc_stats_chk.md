---
layout: post
title: "DMC Statistical Review Check"
tags: [DMC,Clinical Trials]
---

**Background Story:** One day, my boss took one peak at the DMC delivery tables and said, there must be a data issue in death or AE dataset. 

I was extremely shocked by her "Hawk Eyes". I asked my boss how did she noticed the discrepancies, she told me a couple of tricks by experiences.

Then I asked around about an efficient DMC table delivery cross-validation checks, combined many people's idea, and summarized the DMC table checklist.

KEYWORDS: DMC, DEATH, AE, EX, DM

DMC: Data Monitoring Committee(3-7 members) is an independent group of experts who monitor patient safety and treatment efficacy data for ongoing clinical trials. 
based on the study, we will present the reports to the DMC one to four times per year.

DMC Termination Reasons:

Safety Concerns: If AE of particularly serious type are more common in Trial than Control
Overwhelming benefit: If Trial demonstrated undeniably superior to Control, then can apply to next step earlier
Futility: No widely recognized safety issue, nor any benefit from the trail

### DMC OUTPUT CHECKLIST:
Death data consistency

the death number from ADSL, should match ADAE (AE leading to death) and Death form


    2. Exposure dose level and Weight  

if the drug administration is based on the weight, we need to make sure the dose level is correct

    3. Discrepancy from Different data Source:

        EDC vs Randomization

Sometimes some variables (disease stage, PDL1 status) will have multiple source, if the discrepancy is too large we need to inquire the DM about it.


    4. Cross Check:
        -  AE leading to Dose Modification vs EX modification due to AE
        - TEAE overall vs By SOC/ PT tables

   5. Event in Individual Arm vs Pooled Arm:
       Event in Pooled Arm should be equal or more than Individual arm

If it is an ISS or Pooled study for certain indication, we need to make sure the Pooled Arm has equal or more counts than the Individual Arm

**MISC DATA Checks**

```
   AE grade 5  and AE out = Fatal are consistent 
   All start date <= All end date (trtsdt<=trtendt, aestdt<= aeendt)
   Missing AEBODSYS /AEDECOD
   Data Values are in programming formats (E5= "xxx")
   No Truncation (especially while concatenation)
   Lab values with numerical results but No Units (except Ratio)
   Lab test name and LBTESTCD are 1-1 mapping (LBTEST -LBTESTCD)
  Subject Visit are EX, Vital Sign, or any other Visit dataset need to be consistent
  Missing Birthdate
  
 ``` 

Note: This is a quick high level output checklist for personal references, scenarios will  be way more complicated in real life studies.  

THANKS FOR ALL MY GENEROUS BOSS AND FRIENDS (YAO.L, JUN.Z, SAMANTHA.X, YAJNES.B, RUIQI.L ) WHO ARE WILLING TO SHARE THEIR PRECIOUS EXPERIENCES!

Thanks for reading, if you have a check list, please let me know!

REFERENCE:

https://en.wikipedia.org/wiki/Data_monitoring_committee

Data Integrity: One Step before SDTM - LexJansen

Pre-Data Checks for SDTM Development
