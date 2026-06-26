# About the dataset

The dataset is built from the initial dataset consisting of 600,000 transactional records collected over 6 years (period 2014–2019), indicating date and time of sale, pharmaceutical drug brand name, and sold quantity, exported from the Point-of-Sale system in an individual pharmacy.

A selected group of drugs from the dataset (57 drugs) is classified into the following Anatomical Therapeutic Chemical (ATC) Classification System categories:

- **M01AB** — Anti-inflammatory and antirheumatic products, non-steroids, Acetic acid derivatives and related substances
- **M01AE** — Anti-inflammatory and antirheumatic products, non-steroids, Propionic acid derivatives
- **N02BA** — Other analgesics and antipyretics, Salicylic acid and derivatives
- **N02BE/B** — Other analgesics and antipyretics, Pyrazolones and Anilides
- **N05B** — Psycholeptics drugs, Anxiolytic drugs
- **N05C** — Psycholeptics drugs, Hypnotics and sedatives drugs
- **R03** — Drugs for obstructive airway diseases
- **R06** — Antihistamines for systemic use

Sales data are resampled to hourly, daily, weekly, and monthly periods. The data is already pre-processed, where processing included outlier detection and treatment, and missing data imputation.

Here is a version of the categories written in plain language:

- **M01AB** — Painkillers that also reduce inflammation and swelling (the "non-steroid" kind, not like cortisone). Includes drugs like **diclofenac**, often used for joint and muscle pain.
- **M01AE** — The same family of anti-inflammatory painkillers, just a slightly different chemical type. This is the group that includes **ibuprofen** — the everyday pain and fever reliever most people recognise.
- **N02BA** — General pain and fever relievers based on **aspirin** and its relatives. Used for headaches, minor aches, and fever (and in low doses, for the heart).
- **N02BE/B** — Other pain and fever relievers, most notably **paracetamol** (acetaminophen / Tylenol). Common for headaches and fever, and gentler on the stomach than the anti-inflammatory types above.
- **N05B** — **Anti-anxiety medications** (anxiolytics). Calming drugs used to reduce anxiety and tension — for example, diazepam-type medicines.
- **N05C** — **Sleeping aids and sedatives** (hypnotics). Drugs that help people fall asleep or stay calm, closely related to the anxiety group above.
- **R03** — **Asthma and breathing medications**. Treat conditions where the airways narrow, such as asthma or COPD — inhalers fall into this group.
- **R06** — **Antihistamines** (the "allergy" group). Used for hay fever, allergic reactions, and sometimes as a sleep aid.

The first letter is the body system the drug acts on. **M** = musculoskeletal (muscles and joints), **N** = nervous system (brain), **R** = respiratory (breathing).
