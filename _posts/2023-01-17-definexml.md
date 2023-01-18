
---
layout: post
title: Define.xml

tags: [SDTM,Clinical Trail]
---

Background Story:

Once, we need to check a define file, one of my colleagues found many miscellaneous issues, such as punctuation, typos in algorithms, and variable is not on the correct CRF pages. I was surprised by how meticulous he worked. Define file is the critical document while filing an FDA submission, so today we will go over the general structure of Define.pdf/ Define.xml for ADaM and SDTM.

DEFINE.XML DEFINE.PDF ADAM CONTENTS:
Study Datasets: INTO1-2021
Dataset, Description, Class, Structure, Purpose, Key, Location, Documentation
Individual Datasets: ADSL, ADAE ...
Variable, Label, Type, Length/Display format, Controlled Terms or ISO Format, Source/Derivation/Method/Comments, Condition
Code list: List all the code number and decoded values
permitted value, Display Value (Decode)
Ex.




*AEDOSCN: dose action
1 dose not changed;
2 dose reduced;
3 drug interrupted;
4 drug withdrawn;

Methods: All the derivation rules
ex.




*ADSL.RANDFL
if subjects are enrolled and randomized date(RANDDT non-missing)
then RANDFL="y".
otherwise RANDFL="n".





Sample Mini ADaM Define.xml Document:




DEFINE.XML DEFINE.PDF SDTM CONTENTS:
Annotated CRF, CSRG Clinical Trial Reviewer's Guide  
Study Datasets: INTO1-2021
Dataset, Description, Class, Structure, Purpose, Key, Location, Documentation
Individual Datasets: DM,AE,VS, EX ...
Variable, Label, Type, Control Terminology, Origin, Role, Comments
Value List:
variable, value, label, result variable, type, control Terminology, origin, comments
ex. Heart Rate, Diastolic blood pressure...

     5. Controlled terms
          Reference Name, Code Value, Display Value
          ex. various Windowing rule, test name, and Visit numbers.




Sample Mini SDTM Define.xml Document:

Note: While review the Define files, we need to make sure the variable order is the same as the dataset.

Thanks Manesh, Renee, Cindy, 77's help so I can put this define summary together.

Happy studying!
