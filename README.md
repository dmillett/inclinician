# Inclinician

Funded by me:
**TODO**: www.inclinician.org (website)
**TODO**: hosting (Linode, etc)

An open source project intended to help educate and empower individuals ability to measure, analyze, diagnose 
and own all data to resolve health issues.

 * Providing an accessible, open platform for individual health data
   - Share with doctors, research, etc via blockchain contracts, etc
 * Encouraging better communication between patients, clinical staff, researchers and educators
   - collecting & correlating patient symptom data (voice-to-text: chest tightness, achilles pain, etc)
   - patient diagnostic measurement tools (skin, ultrasound, spectometry, mast cells, cytokines, etc) 
 * Science & health education for doctors, patients and researchers
 * Data analysis to help identify gaps in physiological testing methods

 * [Data Complexity & Detailed Overview](#detailed-overview)
 * [Usage](#usage)
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
   - tracked and enforced via blockchain contracts 
 * Functional, Specialty and Cultural medicine resources
 * Cataloging and correlating symptoms with lab tests
   - written or voice symptom journaling is valuable data
 * Encouraging better communication between patients, clinical staff, researchers and educators
   - Increasing empathy and understanding to reduce suffering 
 * To Facilitating and incentivizing an individual's ability to share anonymized patient data for research
   - And to and receive research results
   - Blockchain contracts?
 * Educating patients and the medical community on **Functional Medicine** and **custom treatment**
   - Nutrition
   - Detoxing
   - The uniqueness of genetic expression
   - Test availability and lab quality
   - Immune signaling is very dynamic and complex
   - Biological pathogens (bacteria, virus, parasites, etc) & toxins (metals, molds, man-made, etc)
     - protein fragments from immune action
   - Autoimmune conditions  
   - Immune signature key to assign to test result sets
 * Promoting science based data driven advances in complex health systems
   - Understanding statistical confidence
   - Understanding scientific method, **continual measurement**, new variables, etc      
 * Root Cause Analysis
   - Symptoms may be overlapping and caused by a combination of toxins, pathogens and genetic expression
   - **Inflammation usually causes pain** and/or tissue damage, alleviating pain is only part of the answer

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

### Sample Data

Submitting data with associated blockchain and contract for research, etc. The goal is to establish a few 
defined schemas to facilitate data correlation. The following samples are from [Medschema](https://github.com/dmillett/medschema)
Fields like **age**, **location** and **time** are important because the adaptive portion of the human immune
system learns over time. Mold toxins (mycotoxins), and heavy metals can accumulate over time which can suppress some
immune function (more data needed). Insects and animals can vector a plethora of viral/bacterial/parasitic pathogens that
are new or reactivate immunity when previously encountered.

#### current
Descriptions and measurements with readily available personal equipment. It's a good start to detect disease
migration and provides meaningful physical data for analysis. Billions of data points needed across hundreds of
millions of people. Educating patients and protecting their data is a priority.

Submit with **blockchain_id**, contract, etc

```json
{"identity":"foo123", "blockchain":{"id":"", "contract":""}, "location":{"postal-code": "", "type": "home"}, 
 "date_time":"2020-03-28T17:07:31.000", "age":42, "gender":"", 
 "data":{"temperature":{"device":"braunXyz" , "value":98.4}, "pulse":{"device":"hand", "value":68}, 
         "oxygen":{"device":"oxi", "value":99}, "weight": {}, 
         "descriptions":{"head":"", "sinus":"", "throat":"", "eyes":"", "stomach":"", "intestines":"", "lungs":"",
                         "heart":"", "arms":"", "hands":"", "legs":"", "feet":"", "urine":"", "bowels":"", "skin":"",
                         "back":"" ,"teeth":"", "tongue":"", "energy":"", "general":""},
         "diet":{"time":[{"food":{}, "supplements":{}, "herbals":{}}]}, "exercise": {},
         "prescription":[{"time":"", "name":"", "dose":"", "form":"pill"}]}},

{"identity":"foo123", "blockchain":{"id":"", "contract":""}, "location":{"postal-code": "", "type": "home"},
 "date_time":"2020-03-28T22:17:22.000", "age":42, "gender":"" 
 "data":{"temperature":{"device":"braunXyz" , "value":100.5}, "pulse":{"device":"hand", "value":78}, 
         "oxygen":{"device":"oxi", "value":97}, "weight": {}, 
         "descriptions":{"head":"mild headache", "sinus":"heavy pressure", "throat":"sore", "eyes":"red", "stomach":"", 
                         "intestines":"", "lungs":"cough with phlegm", "heart":"", "arms":"", "hands":"", "legs":"", "feet":"", 
                         "urine":"", "bowels":"", "skin":"", "back":"low back ache", "teeth":"", "tongue":"", 
                         "energy":"tired, low", "general": "mild body aches"},
         "diet":{"time":[{"food":{}, "supplements":{}, "herbals":{}}]}, "exercise": {},
         "prescription":[{"time":"", "name":"", "dose":"", "form":"pill"}]}}
```

#### future (to advance medical science)
Descriptions and measurements with potential future personal equipment. Tens of billions of data points across billions
of people are required. Educating patients and protecting their data is a priority.

```json
{"identity":"foo123", "blockchain":{"id":"", "contract":""}, "location":{"postal-code": "", "type": "home"},  
 "date_time":"2020-03-28T17:07:31.000", "age":42, "gender":"",
 "data":{"temperature":{"device":"braunXyz" , "value":98.4}, "pulse":{"device":"hand", "value":68}, 
         "oxygen":{"device":"oxi", "value":99}, "weight": {},
         "descriptions":{"head":"", "sinus":"", "throat":"", "eyes":"", "stomach":"", "intestines":"", "lungs":"",
                         "heart":"", "arms":"", "hands":"", "legs":"", "feet":"", "urine":"", "bowels":"", "skin":"",
                         "back":"", "teeth":"", "tongue":"", "energy":"", "general":""},
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

## Resources
 * Medschema (https://github.com/dmillett/medschema) 
   - Standardizing symptom and test data into a standard schema or structure
 * Statistical Confidence
 * Scientific Method
 * Cellular Biology

<a name="collaborate"/></a>
## Collaborate & Contribute

**TODO**

## License

Copyright © 2019 FIXME

This program and the accompanying materials are made available under the
terms of the GNU LESSER GENERAL PUBLIC LICENSE Version 2.1