---
layout: post
title: Trial Domain
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [SDTM,Clinical Trail]
---

BACKGROUND :

We finally we over the 5 study design trials, TA, TE, TI, TV, TS. As we mentioned last time, TS acts like the outline of the puzzle, how can we fit the puzzles together? What are the relations between these five datasets?

Rather than focusing on individual datasets, today we will connect the 5 trial design datasets together with a good story line!

PURPOSE:

FDA can use trial design, especially TS info to track and report the clinical study data for submission. Those Trial design datasets provides the standard info for reviewers to understand:

A clear clinical trial design model
Key info with simple data structure for centrally search
Rules for subjects transition through various periods or phases
Machine-readable versions of the high-level protocol info overview
Differences between actual and planned treatment arms 

The following Trial Design Model (TDM) is based on TE (Trial element), TA (Trial arm), and TV(trial visit).

General Example:

TS: submits trial-level summary info, including blinding schema, drug indication, and trial objectives.

TE: describes the Element(unique study cell value), including planned interventions, event starts, end, duration. (Link to EX, SE)

TA: describes the sequence and rules of moving of the Elements within each Arm.(Link to DM, consistent with TE)

TV: describes planned visit.(Link to SV domain)

TI: describes the protocol specified inclusion/exclusion criteria in study level to screen subjects. (Link to IE domain)

Since Trial Summary  would help us to be familiar with the protocol, and Element is the basic building block for interventions, we usually generate the dataset in the sequence of TS ->TE -> TA -> TV -> TI

If we view TDM as a building, TS is the outline or sketch of the building we conceived, TE are the number of floors, TA would be the different styles of decoration, TV are the planned number of rooms, and TI would be the standard to select construction materials.

Detailed Example:


CHALLENGES :

My friend 77's team had multiple round of checking the Trial design data not only because it involves with massive info from protocol, but also they need to ensure TA, TE, and TV domain are consistent with Subject Elements and Subject Visits (SE, SV). In another words, individual level data have to match with the planned protocol document when systematically check across all subjects with multiple domains. 

Little tips:

When come to check the Trial Design data, I wouldn't be shy to ask for colleagues' suggestions or comments. Maybe they will have some insightful ideas or sporadic checkpoints that might be critical and I wasn't aware of.  As a saying, sharing is more in knowledge ^-^!

Happy Reading!

Ref:

Graph: https://www.pharmasug.org/proceedings/2014/DS/PharmaSUG-2014-DS03.pdf

https://www.pharmasug.org/proceedings/2011/CD/PharmaSUG-2011-CD13.pdf

INC research, Trial Design Introduction. Elke sennewald
