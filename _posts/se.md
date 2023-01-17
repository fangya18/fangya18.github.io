---
layout: post
title: SDTM: SE Subject Element Domain
subtitle: SE
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [SDTM]
comments: true
include: false transitions:
---

**Background Story :**

One day, my friend 99 discussed with me if a patient is randomized but not treated has some lab results besides screening, how should we classify the EPOCH variable for him/her in SE domain?
So today we will go over a basic example for SE domain: Subject Element.

**Purpose:**

The SE stores treatment data linked together with demographic data and Trial Design data,  which is possible to standardize and create unique data-driven mapping for a high level view of study.

**Basics:**

SE (Subject Element) contains subject level data about the timings of each subject transition from one element period to the other (screening, treatment, follow-up) and the treatment information (active, non-active) from multiple sources.




**Key Variables:**

STUDYID, DOMAIN, USUBJID, SESEQ, ETCD, ELEMENT, SESTDTC, SEENDTC,TAETORD,EPOCH

Variable Derivation Rules:

*1.Seseq
Sequential number is unique for the records within the domain by USUBJID.

*2.ETCD
Element Code is assigned (SCREEN, Treatment, Placebo, FUP).

*3.ELEMENT
Description of Element is assigned.(Screening, Treatment info, Follow up).

*4.SESTDTC
Start date of the element depends on Planned Arm
relates to Informed consent date, Reference start date, Treatment Exposure Date.

*5.SEENDTC
End date of the elements equal to the next SESTDTC of next element.

*6.TAETORD
Planned Order of Elements within Arm is directly from TA

*7.EPOCH
Epoch is directly from TE.EPOCH
it originated from to reference start/end date.




**SE Mini Sample Data Set: **




Note: The dataset is a dummy sample, real data will have different SESTDTC, SEENDTC dates

To end the story we started, SE would only keep the Screening record for a patient without treatment even he/she has follow up records.

Thanks 99 for sharing a case study with me!

Happy Studying!

*Ref:*

https://www.lexjansen.com/pharmasug/2010/CD/CD08.pdf
