# Inclinician

Funded by me:
**TODO**: www.inclinician.org (website)
**TODO**: hosting (Linode, etc)

**In an incomplete model, almost all data is relevant**! This is open source project intended to help educate and empower 
individuals ability to measure, analyze, diagnose and own all data to resolve health issues. This platform is 
intended to:

 1. Provide an accessible, open platform to facilitate sharing and education of individual health data. 
    - Share via blockchain contract for research and medical analysis
 2. Encouraging better communication between patients, clinical staff, researchers and educators
    - collecting & correlating patient symptom data (voice-to-text: chest tightness, achilles pain, etc)
    - patient diagnostic measurement tools (skin, ultrasound, spectometry, mast cells, cytokines, etc) 
 3. Science & health education for doctors, patients and researchers
 4. Data analysis to help identify gaps in physiological testing methods

 * [Data Complexity & Detailed Overview](#detailed-overview)
 * [Usage](#usage)
   - [Example: Blood Donations](#blood)
   - [Example: Current (current devices) Data Sample](#current-data-options)
   - [Example: Future (new devices) Data Sample](#future-data-options)
 * [Collaborate](#collaborate)

<a name="detailed_overview"/></a>
## Data Complexity & Detailed Overview

Our planet and DNA would not exist without an enormous number of bacterial, viral and environmental influences 
over the course of 1.5+ billion years. The net result is 7+ billion highly unique people within the context of 
diminishing biodiversity and the interaction of our collective immune systems. Individual immune expression is a 
complex differential equation relative to time, stimuli, genetic & adaptive immune response. With over 4 million 
SNPs and hundreds of types of immune cells (cytokines, macrophages, tcells mast, etc) constantly change, there is 
no deterministic formula that works. Billions of data points for immune signaling and adaptive immune responses are 
required for people of different ages and locations. A large enough data matrix makes group correlations possible, 
which in turn invites more data for further refinement. For example, data from household sanitary labs for septic 
waste and air filtration. Data from personalized detection instruments ranging from spectrometers, 
ultrasound/thermal/electro-magnetic field imaging, oxygen/breathe saturation and embedded nano-sampling of immune 
signaling. And finally, voice-to-text symptom description. This will allow for safer and more effective medicines, 
vaccines and treatments. A healthier world of scientific discovery awaits... 
 
 * Providing an accessible, open platform for individual health data
   - Tracked and enforced via blockchain contracts 
 * Functional, Specialty and Cultural medicine resources
 * Cataloging and correlating symptoms with lab tests
   - Written or voice symptom journaling is valuable data
 * Encouraging better communication between patients, clinical staff, researchers and educators
   - Increasing empathy and understanding to reduce suffering 
 * To Facilitating and incentivizing an individual's ability to share anonymized patient data for research
   - Receive research results
   - Blockchain contracts?
 * Educating patients and the medical community on **Functional Medicine** and **custom treatment**
   - Nutrition
   - Detoxing
   - The uniqueness of genetic expression
   - Test availability and lab quality
   - Immune signaling is very dynamic and complex
   - Biological pathogens (bacteria, virus, parasites, etc) & toxins (metals, molds, man-made, etc)
     - Protein fragments from immune action
   - Autoimmune conditions  
   - Immune signature key to assign to test result sets
 * Promoting science based data driven advances in complex health systems
   - Understanding statistical confidence
   - Understanding scientific method, **continual measurement**, new variables, etc      
 * Root Cause Analysis
   - Symptoms may be overlapping and caused by a combination of toxins, pathogens and genetic expression
   - **Inflammation usually causes pain** and/or tissue/organ damage, alleviating pain is only part of the answer

### Risks
Due to the large number of unknowns in human physiology, there are a number of existing risks to account for:

 1. Failure to advance understanding of human immune systems
 2. Exposure of personal information for abuse by criminals & private or public institutions
 3. Accidental or deliberate falsification of data
 4. Insufficient tests, equipment, data or understanding
 5. Misdiagnosis & poor analysis
 6. Side effects from pharmaceutical, supplements, herbs, vaccines, etc

<a name="usage"/></a>
## Usage
Given the enormous variation and uniqueness of the human population and the cumulative, ongoing changes with
immune expression (signaling, T-cells, b-cells, etc), it is important to gather as much data as possible before
meaningful correlation and understanding of our unique immune responses can be understood.

 1. Capture physical aches/pains/fatigue/mood data via voice-to-text to schema (ex: medschema)
 2. Capture data from any personal medical equipment pulse/temperature/dermoscopy/spectrometers/etc to schema (ex: medschema)
    - including equipment ID, etc
 3. Ownership of all laboratory tests to schema
    - including lab ID and test ID
 4. Use this/any platform to identify medical research studies
 5. Establish contract within a blockchain construct
    - credit, research results, donate, etc
 6. Get study results
 7. Analyze or submit for analysis to larger groups
 8. Repeat as necessary with new data

<a name="blood"/></a>
### Blood Donation Labs

Blood donations are important, but given the biological nature of Earth and the immune expression of the donor, 
it is possible to transmit more than blood and plasma. Recently, screening blood for Babesia, a less virulent red
blood cell ~parasite, in many blood collection facilities in the US. 

All blood donations should be **screened**, **scored** and **ranked** for safety based conditions for things like pathogens
and anomalies. Then the data is correlated, via donor Blockchain, with research studies and stored in blood banks. 

For example, the blood could be tested for common pathogens (Borellia, Bartonella, Babesia, Erlichia, Corona, etc) with
**antibody testing** or **T-cell response** testing. This can help minimize the unintended transmission of pathogens or
transmission of pathogens with treatment options.

<a name="sample-data"/></a>
### Sample Data

Submitting data with associated blockchain and contract for research, etc. The goal is to establish a few 
defined schemas to facilitate data correlation. The following samples are from [Medschema](https://github.com/dmillett/medschema)
Fields like **age**, **location** and **time** are important because the adaptive portion of the human immune
system learns over time. Mold toxins (mycotoxins), and heavy metals can accumulate over time which can suppress some
immune function (more data needed). Insects and animals can vector a plethora of viral/bacterial/parasitic pathogens that
are new or reactivate immunity when previously encountered.

<a name="current-data-options"/></a>
#### current: personal equipment available today
Descriptions and measurements with readily available personal equipment. It's a good start to detect disease
migration and provides meaningful physical data for analysis. Billions of data points needed across hundreds of
millions of people. Educating patients and protecting their data is a priority.

Submit with **blockchain_id**, contract, etc

```json
{"identity":"foo123", "blockchain":{"id":"", "contract":""}, "location":{"postal-code": "", "type": "home"}, 
 "date_time":"2020-03-28T17:07:31.000", "age":42, "gender":"", 
 "data":{"temperature":{"device":"braunXyz" , "value":98.4, "unit": "F"}, "pulse":{"device":"hand", "value":68}, 
         "oxygen":{"device":"oxi", "value":99, "unit": ""}, "weight": {}, 
         "descriptions":{"head":"", "sinus":"", "throat":"", "eyes":"", "stomach":"", "intestines":"", "lungs":"",
                         "heart":"", "arms":"", "hands":"", "legs":"", "feet":"", "urine":"", "bowels":"", "skin":"",
                         "back":"" ,"teeth":"", "tongue":"", "energy":"", "general":""},
         "photographs":{},
         "diet":{"time":[{"food":{}, "supplements":{}, "herbals":{}}]}, "exercise": {},
         "prescription":[{"time":"", "name":"", "dose":"", "form":"pill"}]}},

{"identity":"foo123", "blockchain":{"id":"", "contract":""}, "location":{"postal-code": "", "type": "home"},
 "date_time":"2020-03-28T22:17:22.000", "age":42, "gender":"" 
 "data":{"temperature":{"device":"braunXyz" , "value":100.5, "unit": "F"}, "pulse":{"device":"hand", "value":78}, 
         "oxygen":{"device":"oxi", "value":97, "unit":""}, "weight": {}, 
         "descriptions":{"head":"mild headache", "sinus":"heavy pressure", "throat":"sore", "eyes":"red", "stomach":"", 
                         "intestines":"", "lungs":"cough with phlegm", "heart":"", "arms":"", "hands":"", "legs":"", "feet":"", 
                         "urine":"", "bowels":"", "skin":"", "back":"low back ache", "teeth":"", "tongue":"", 
                         "energy":"tired, low", "general": "mild body aches"},
         "photographs":{},
         "diet":{"time":[{"food":{}, "supplements":{}, "herbals":{}}]}, "exercise": {},
         "prescription":[{"time":"", "name":"", "dose":"", "form":"pill"}]}}
```

<a name="future-data-options"/></a>
#### future: future personal equipment (to advance medical science)
Descriptions and measurements with potential future personal equipment. Tens of billions of data points across billions
of people are required. Educating patients and protecting their data is a priority.

```json
{"identity":"foo123", "blockchain":{"id":"", "contract":""}, "location":{"postal-code": "", "type": "home"},  
 "date_time":"2020-03-28T17:07:31.000", "age":42, "gender":"",
 "data":{"temperature":{"device":"braunXyz" , "value":98.4, "unit":"F"}, "pulse":{"device":"hand", "value":68}, 
         "oxygen":{"device":"oxi", "value":99, "unit":""}, "weight": {},
         "descriptions":{"head":"", "sinus":"", "throat":"", "eyes":"", "stomach":"", "intestines":"", "lungs":"",
                         "heart":"", "arms":"", "hands":"", "legs":"", "feet":"", "urine":"", "bowels":"", "skin":"",
                         "back":"", "teeth":"", "tongue":"", "energy":"", "general":""},
         "photographs":{},
         "diet":{"time":[{"food":{}, "supplements":{}, "herbals":{}}]}, "exercise": {},
         "prescription":[{"time":"", "name":"", "dose":"", "form":"pill"}],
         "ultrasound":{"device":"abc", "location":"", "data":{}},
         "spectrometer":{"device":"foo", "location":"", "data":{}},
         "breathalyzer":{"device":"foo", "data":{}},
         "urinalysis":{"device":"foo", "data":{}},
         "stool_analysis":{"device":"foo", "data":{}},
         "saliva_analysis":{"device":"foo", "data":{}},
         "immune_signal_analysis":{"device":"foo", "location":"", "data":{"cytokines":{}, "white":{}, "mast":{}}} } }          
```

### Labs

In many cases where chronic conditions exist improvements in health are delayed for specific conditions:

 * HLA DRB/Q genetic SNP testing (one time)
   - can indicate potential to accumulate mold toxins and heavy metals over a lifetime
   - http://hla.alleles.org/data/hla-drb.html
 * Genova Ion Panel (repeat as necessary)
   - nutritional evaluation 
   - https://www.gdx.net/product/ion-profile-nutritional-test-blood
 * Inflammation markers (as necessary)
   - SED
   - C3a
   - C4a
   - TGF-b1

## Thoughts
In general, there is a huge gap in microbiology knowledge for each person's immune landscape. There is also
a problem of opaque data and results. How can feedback and improvement be incorporated into the ongoing development
and application of vaccines and pharmaceuticals? How can doses and ingredients be customized to increase effectiveness
and reduce risk for patients?

### Sars-Cov-2 ('covid 19')
A lot more data is needed from severely ill patients and asymptomatic people to get a better understanding of
 * How is immunity working for asymptomatic people?
 * How can previous exposure and pre-existing ~immunity be measured (T-cells: CD8? CD4? etc)
 * How are asymptomatic & immune people affected? 
   - Are any chronic conditions noted?
   - Was there minor, repairable organ damage?  
   - Was there stroke damage? (see D-dimer lab)

#### mRNA Vaccines Questions
How to collect immune response data and measure variability?
 * How long does the mRNA payload reside in the system (~half life or time-to-live)?
 * What other cells are most likely to absorb mRNA payload (tissue, biofilms, etc)?
 * How much does the adjuvant(s) increase system availability of the payload?
 * What are the protein (sub-unit?)  fragments & structure variations generated by the immune system from mRNA?
 * How is the mRNA payload affected by metals/toxins in tissue and biofilms?
 * How would/do existing pathogens (Lyme, Bartonella, etc) in biofilms uptake the mRNA?
 * Will HLA genetic SNPs play a role in removing generated protein fragments from the body?
   - Is this what "long haulers" experience?
 * Spike protein presentation from natural infection (nasal/airways/eyes) vs localized/systemic muscle tissue generated?
 * What similarity between non-spike proteins produced & other proteins, current & probable, Ab/T immune function? 
   - Would this potentially result in auto immune responses?
   - Epigenetic changes?

How is the vaccine effectiveness measured among recipient distributions?
 * Were there T-cells demonstrating no previous exposure prior to vaccine for trial & placebo groups
 * How similar were the infected & effective vaccine recipients for:
   - local population densities?
   - safety protocol adherence?
   - age?
   - gender?
   - ethnicity?
   - coordinates? 
   - genetics?
 * What was different about the 5 - 10% of vaccine recipients who got sick?
   - see metrics above
 * How does vaccine delivery differ from normal, droplet transmission?
 * What about Antibody Disease Enhancement (ADE) risk for SARS-COV-2 vs other coronaviruses?
   - This is an acknowleged risk by the FDA, but is ignored by the media.

#### Nutrition
 * Vitamin D (immune, T-cell increase)
 * Turmeric (reduce IL-6)
 * Blood thinners OR Nattokinase (effective blood clot dissolver)
 * Zinc (anti-covid cellular integrity)
 * Vitamin C (antioxidant, detox)
 * Glutathione (antioxidant, detox)

#### Astra Zeneca
 * A Phase 2 recipient developed Multiple Sclerosis
   - It was 'determined' to be from something else?
   - What else would trigger a neurological issue besides the vaccine/adjuvant/ingredients in close proximity to the vaccine?
   - What labs & criteria were the "healthy patients" screened with?
 * A Phase 3 recipient developed Transverse Myelitis 
   - How could this be avoided for other susceptible people? 
 * Phase 3 doses were incorrect for 2000+ trial recipients
   - Why was there a dosing error?
   - Why was the reduced dose (1/2, 1 ... 3/4 full dose) more effective?
     - What metrics were better?
     - Why isn't the reduced dose used going forward?
     - Should Phase 3 be updated?

#### BioNtech/Pfizer
 * https://www.fda.gov/media/144245/download
 * T-cell testing for Phase 1 (45/90 - vaccine/placebo) baselines and post vaccine
   - Was this for both vaccinated & placebo groups? (missing/no data)
   - What were baseline values? (missing/no data)
   - Did baseline values indicate previous exposure and/or responsiveness? (missing/no data)
 * T-cell response testing happened for first ~360 Phase 2 recipients
    - Was this for both vaccinated & placebo groups? (missing/no data)
    - What were baseline values? (missing/no data)
    - Did baseline values indicate previous exposure and/or responsiveness? (missing/no data)  
 * Age, ethnicity and gender groups data provided, but no location data
   - Population density increases risk of spread 
   - Population density also indicates increased chance of previous exposure
   - What were the geographic locations of infected placebo, vaccine recipients?
   - What were the locations of the non-infected placebo, vaccine recipients?
 * Autoimmune conditions can arise from any new proteins/pathogens/toxins/etc in the body
   - Why is the study limited to 8 weeks for new vaccine type mRNA?
 * No positive tests are counted between Day 1 (dose 1) + 7 days after last dose
   - Why is phase 2+ testing limited to nasal turbinate PCR (or equivalent) test?
   - Why is any positive test between Day 1 (dose 1) - Day 28 (dose 2 + 7 days) ignored/excluded?
   - Since the vaccine failed to provide immunity for some, where is their immunogenicity data?
 * Why are there no recommendations of a single dose for people with lower risk factors (age < 65)?

#### Moderna
 * Similar to Pfizer except no positive test counted until last dose + 14 days
 * No T-cell testing indicated from phase 1 testing in FDA report (seems like they did it though)
 * ADE risk is acknowledged, but will likely require more than 8 weeks of surveillance for all recipients.
 * FDA and media pointed out Moderna's 3 cases of Bells Palsy out of ~13k+ vaccine recipients, but did not
give similar mention to Pfizer's 4 cases for 18k+ vaccine recipients.

## Resources
 * Statistical Confidence (wikipedia)
 * Scientific Method (wikipedia)
 * Cellular Biology (wikipedia; "Molecular Biology of the Cell, 6th; etc)
 * Medschema (https://github.com/dmillett/medschema) 
   - Standardizing symptom and test data into a standard schema or structure

<a name="collaborate"/></a>
## Collaborate & Contribute

**TODO**

## License

Copyright © 2019 FIXME

This program and the accompanying materials are made available under the
terms of the GNU LESSER GENERAL PUBLIC LICENSE Version 2.1