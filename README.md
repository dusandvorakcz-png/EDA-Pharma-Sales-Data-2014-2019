# About the Dataset

This dataset comes from the Point-of-Sale system of a single pharmacy. It is built
from around 600,000 transactional records collected over six years (2014–2019),
each recording the date and time of sale, the drug name, and the quantity sold. A
selected group of 57 drugs is classified into 8 categories using the Anatomical
Therapeutic Chemical (ATC) Classification System.

The source provides the data resampled to hourly, daily, weekly, and monthly
periods. **This project uses the monthly file.** The daily file is used only once,
to confirm a data-quality issue in the cleaning section.

The source also describes the data as already pre-processed (outlier treatment and
missing-data imputation). In practice I still found two months that needed handling
— a corrupt January 2017 and a partial October 2019 — so I did my own checks rather
than assume the data was clean (see Data Quality and Cleaning).

## Drug categories

The first letter of each code is the body system the drug acts on:
- **M** = musculoskeletal (muscles and joints),
- **N** = nervous system (brain),
- **R** = respiratory (breathing).

## Dictionary

- **M01AB** — Painkillers that also reduce inflammation and swelling (the "non-steroid" kind, not like cortisone). Includes drugs like diclofenac, often used for joint and muscle pain. *(ATC: anti-inflammatory/antirheumatic, acetic acid derivatives)*
- **M01AE** — The same family of anti-inflammatory painkillers, a slightly different chemical type. Includes ibuprofen, the everyday pain and fever reliever most people recognise. *(ATC: propionic acid derivatives)*
- **N02BA** — General pain and fever relievers based on aspirin and its relatives. Used for headaches, minor aches, and fever (and in low doses, for the heart). *(ATC: salicylic acid and derivatives)*
- **N02BE** — Other pain and fever relievers, most notably paracetamol (acetaminophen / Tylenol). Common for headaches and fever, and gentler on the stomach than the anti-inflammatory types above. *(ATC: pyrazolones and anilides)*
- **N05B** — Anti-anxiety medications (anxiolytics). Calming drugs used to reduce anxiety and tension, for example diazepam-type medicines. *(ATC: psycholeptics, anxiolytics)*
- **N05C** — Sleeping aids and sedatives (hypnotics). Help people fall asleep or stay calm, closely related to the anxiety group above. *(ATC: psycholeptics, hypnotics and sedatives)*
- **R03** — Asthma and breathing medications. Treat conditions where the airways narrow, such as asthma or COPD; inhalers fall into this group. *(ATC: drugs for obstructive airway diseases)*
- **R06** — Antihistamines (the "allergy" group). Used for hay fever, allergic reactions, and sometimes as a sleep aid. *(ATC: antihistamines for systemic use)*
