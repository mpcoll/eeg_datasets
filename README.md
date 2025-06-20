List of relevant/useable EEG paindatasets
# Internal datasets

pllab_eeg_pain_reward
* participants: 50 healthy  
* pain conditions: 5 calibrated shock pain levels
* other conditions: 5 levels of reward, pain vs reward decision, pain anticipation, reward anticipation
* System/n_channels: 64 channel EEG Acticap (EGI amp)  
* questionnaires: PCS, STAI, BDI, SOCIO

----------------------------------------------
 pllab_eeg_pain_database_laval

* participants: ~80 healthy (still growing)
* pain conditions: tonic heat pain, tonic orofacial chemical pain
* other conditions: rest (eyes open), rest (eyes closed), tonic auditory stimulation, tonic orofacial disgust
* system/n_channels: 64 channel EEG Acticap (EGI  + BrainVision amp)  
* questionnaires: PCS, STAI, BDI, SOCIO, Debrief

----------------------------------------------
 pllab_eeg_svr

* participants: 44 healthy   
* pain conditions: heat pain (~ 5 s ) 
* other conditions: svr
* system/n_channels: 64 channel EEG Acticap (EGI  + BrainVision amp)
* questionnaires: PCS, STAI, BDI, SOCIO

----------------------------------------------
 roylab_eeg_pain_mcgill

* participants: 42 healthy   
* pain conditions: tonic heat pain,  
* other conditions: rest (eyes open), tonic auditory stimulation  
* system/n_channels: 64 channel EEG Acticap (EGI  + BrainVision amp)
* questionnaires: PCS, SOCIO 

----------------------------------------------

 massealarie_eeg_cohort

* participants: 50 acute back pain
* pain conditions: rest (eyes closed) before/after back movement
* other conditions: SEP
* system/n_channels: 64 channel EEG Acticap (EGI  + BrainVision amp)
* questionnaires: PCS, SOCIO, ++ other
* Other measures: TMS, SEP

----------------------------------------------

External open datasets
Experimental pain
https://osf.io/q8tgj/ 
Chowdhury et al. (seminowicz)
*Name: A novel cortical biomarker signature predicts individual pain sensitivity 
*Link https://openneuro.org/datasets/ds005486/versions/1.0.0
*Paper: https://pmc.ncbi.nlm.nih.gov/articles/PMC11469350/ 
*Participants: 150 healthy (100 training set and 50 test set), aged 18 to 44 years  
*Pain conditions: injection of nerve growth factor (NGF) to the right masseter muscle on Days 0 and 2 to induce prolonged temporomandibular pain lasting up to 4 weeks. Prolonged temporomandibular pain (outcomes collected over 30 days).		 	 	 		
*Measures: →PAF (5 minutes eyes-closed resting-state EEG)- day 0,2 and 5
                   → CEM (transcranial magnetic stimulation (TMS) mapping)- day 0, 2 and 5
	       → Corticomotor excitability (by MEP amplitudes)
	       → Growth mixture modelling (GMM) in R to form two classes: high and low pain sensitive; use to label the test set.
        →The locked machine learning model was assessed on the test set.
*other measures: Sensorimotor PAF, CME, Sex, Pain Catastrophizing Scale (PCS) Total and PCS Helplessness (biomarker performance combined with covariates). 5 machine learning models, etc.
*questionnaire: electronic pain diaries (Day 1 to 30 at 10 am and 7 pm), scale pain (1-10) during different activities.

Strube et al. (2023)
*Name: Agency affects pain inference through prior shift as opposed to likelihood precision modulation in a Bayesian pain model
*Paper: 10.1016/j.neuron.2023.01.002 
*Participants: 2 experiments. 1→ n=25, used continuous pain ratings to establish a precise readout of pain perception during painful heat stimulation and after treatment. 2→ n=54, additionally employed EEG to evaluate neurophysiological correlates of the modulation via expectations and agency.
*Pain conditions: heat pain to capsaicin-sensitized skin on the left radial forearm. Self-treatment vs external treatment.
*Measures: Bayesian modeling  to assess the mechanisms by which agency influence pain perception in the context of different pain treatment expectations. EEG. 
	Experiment 1:
→ high and low treatment expectation conditions are related to the predictive cues signaling high or low treatment success and not to actual expectation ratings. Used VAS. Agency and expectation effects.
	Experiment 2:
→repeated ANOVA with all three stimulis intensitiesin post-treatment VAS rating  (including conditioning and test trials): VAS10, 30 and 50. Agency and expectation effects. 
	Conditioning:
→ predictive cue indicated an upcoming highly or weakly effective treatment on the ongoing VAS70 stimulus (established during conditioning trials), representing VAS10 + cue indicating low treatment representing VAS50. VAS10 vs VAS50.
	Agency:
→participants initiate the treatment themselves or by the experimenter (external). Test t for EEG time-frequency data + agency w cue-locked. Reaction times (explained, maybe, agency effects, Exp.2).
Expectation:
→ cluster-corrected dependent samples t test on cue-locked data. Pearson’s correlation analysis on z-standardized behavioral expectation effects per subject.
	Interaction of agency and expectation:
→ cluster-corrected dependent samples t test, post hoc t tests.
*Other measures: 

Clinical datasets
plonerlab_eeg_chronicp_analgesics

* Name : Effects of analgesics on EEG biomarkers of chronic pain
* Link https://osf.io/mj9xr/
* Paper: https://www.sciencedirect.com/science/article/pii/S1526590025000148#bib16
* participants: 118 (same as Dinh et al. 2019) and 102 (new) all chronic pain  
* pain conditions: chronic pain resting state (eyes open and closed)
* 102 new: 29 channel EEG (Quick 32-r)
* 118: 64 channel EEG (ActiCap 64)

### Ploner neurofeedback plos biology
*Name: Neurofeedback and attention modulate somatosensory alpha oscillations but not pain perception
*Link: https://osf.io/2mnys/ 
*Paper: https://pmc.ncbi.nlm.nih.gov/articles/PMC11756787/ 
*Participants: the final sample comprised 75 healthy right-handed participants → short version of the Edinburgh handedness inventory
*Pain condition: Noxious stimuli were applied using cutaneous laser stimulation on the dorsum of the left hand
*Measures: EEG-based neurofeedback, bidirectional control design with 2 verum and 2 sham conditions (completed during 2 sessions) → asymmetry of alpha oscillations, pain perception, and pain processing
	First verum: focus attention on right hand 
	Second verum: focus attention on the left hand (same 2 conditions with sham)
	→ 40 trials with 15s of neurofeedback training (noxious laser stimulus applied to the dorsum of the left hand), perceived pain intensity (NRS) 1 to 100.
	→To quantify baseline measures: painpre (20 noxious) and EEGpre (5 min of resting-state, eyes open)
*other measures: BrainAmp MR plus amplifiers and 64 actiCAP snap sensors placed according to the 64-channel extended international 10–20 system, electrooculographic activity with a bipolar Brain Amp ExG MR amplifier, Ag/AgCl sensors; motivation→ using a seven-point Likert scale, etc. 

### ploner mediation multiple laser pain
*Name: Perceptual and motor responses directly and indirectly mediate the effects of noxious stimuli on automatic responses 
*Link: https://osf.io/bsv86/ 
*Paper:https://journals.lww.com/pain/abstract/2019/12000/perceptual_and_motor_responses_directly_and.14.aspx 
*Participants: 47 healthy, right-handed (46 participants for the motor condition). 
*Pain condition: perceptual, motor, and autonomic responses to noxious stimuli in 4 experimental conditions → 60 painful stimuli were applied to the dorsum of the left hand, Tm:YAG laser, different levels of pain. Eyes closed. 
-Participants were asked to react as fast as possible to the noxious stimuli by releasing a button with the right index finger→ a measure of motor responses.
-Participants were prompted by an auditory cue to provide ratings of perceived pain intensity 3 seconds after the stimulus→ a measure of perceptual responses. 
-Skin conductance was recorded during the experiment→ a measure of autonomic responses. 
Before the actual experiment, pain thresholds and stimulation intensities were determined+ 10 minutes of resting-state EEG data were recorded. 
*Measures: Multilevel 2-path and Multilevel 3-path. 
*Other measures: Single-trial pain ratings (perceptual), reaction times (motor), and SCRs (autonomic responses; 2 Ag/AgCl electrodes). Auditory cue presented 3 seconds → verbally rate their pain (1 to 100), etc.

Nat Comm and Pain??

### ploner bott sci advances
*Name: Local brain oscillations and interregional connectivity differentially serve sensory and expectation effects on pain
*Link: https://osf.io/fn76w/ 
*Paper: DOI: 10.1126/sciadv.add7572 
*Participants: 40 healthy human participants at the University Hospital of the Technical University of Munich (TUM); right-handedness and age > 18 years. 21 females; age, 23.4 ± 2.9 years. 
*Pain condition: brief heat pain stimuli; varying stimulus intensity and expectations about upcoming stimulus→ two levels of noxious stimulus intensities (hi and li) and two types of visual cues (HE and LE), resulting in four experimental conditions. The visual cues probabilistically predicted the intensity of the subsequent noxious stimulus. 
	-Laser pulse (1340 nm); duration of 4 ms and diameter of approximately 7 mm on left hand + change places.
-Li and Hi stimuli: 3 and 3,5 J, respectively. 
 *Measures: 3s after the painful stimulus, verbal rating of the perceived pain intensity→ scale ranging from 0 (no pain) to 100. To ensure attention to the visual cues, participants were visually prompted to indicate by a button press whether a HE or a LE cue had been presented in 10% of the trials (catch trials). 
	-Brain activity recorded→ actiCAP snap/slim with 64 activesensors (Easycap) placed according to the extended 10-20 systemand BrainAmp MR plus amplifiers. 
	-BrainVision Analyzer software → preprocessing. 
	-Local oscillatory brain activity was assessed as frequency-specific source power of the six ROIs (explained in detail on page 11).
	-Connectivity analyses were performed on the 1-s poststimulus intervals of the source-level time series of the six ROIs (page 11).
*Other measures: Average anxiety and depression scores (Hospital Anxiety and Depression Scale). Familiarized with the stimulation and the intensity rating→ 10 heat stimuli +  training run comprising 16 trials was conducted (after knowing about the paining between cues and stimulus intensities). ICs from eye movements or muscles. Sensor-level time series to source level→ Linearly constrained minimum variance (LCMV) beamformers (62) implemented in FieldTrip (61); For each of the four trial types (liLE, hiLE, liHE, and hiHE), behavioral and EEG measures were computed based on an identical number of trials; PEs, etc.

### ploner_tacs
*Name: Modulating Brain Rhythms of Pain Using Transcranial Alternating Current Stimulation (tACS)- A Scam-Controlled Study in Healthy Human Participants
*Link: https://osf.io/fn76w/
*Paper: 10.1016/j.jpain.2021.03.150  
*Participants: 29 healthy participants, all right-handed, 13 females, age: 25.7±4.0 years. Inclusion criteria→ age above 18 years and right-handed. 
*Pain condition: experimental model of chronic pain
*Measures: pre-registered at ClinicalTrials.gov→ 6 recording sessions (​​separated by at least 24 hours). In each session, tACS was applied over prefrontal cortex (PFC) or somatosensory cortex + using alpha frequency (10 Hz), gamma frequency (80 Hz), or sham stimulation. 
-Heat pain stimulus of varying intensities→ left hand 10 minutes using a thermode; continuously rated the perceived pain intensity (visual analogue scale (VAS) ranging from 0 (“no pain”) to 100 (“worst tolerable pain”)) + autonomic responses (skin conductance and electrocardiogram) continuously measured→ palmar distal phalanges of the left index and middle finger using Ag/ AgCl electrodes connected to a GSR-MR module w constant 0.5 V voltage (nSF) and the heart rate (HR). Data were recorded in direct current (DC) mode with low-pass filtering at 250 Hz. EEG→ using a bipolar Ag/AgCl electrode montage (right clavicule). Both skin conductance and ECG were sampled at 1000 Hz using the BrainAmp ExG MR amplifier
9 plateaus with 3 temperature levels (low, medium, and high), adjusted to each participant.  Pain ratings were sampled with a frequency of 1000 Hz by a BrainAmp ExG MR amplifier. 
-tACS: Ten minutes of tACS were applied simultaneously to painful heat stimulation: Neuroconn DC-STIMULATOR MR and 2 carbonized rubber electrodes with a size of 5x5 cm. Validate electrode placement→ SimNIBS 2.1. Other measures for tACS on page 1259 (or 4).
-Before and after the stimulation, 5 minutes of resting state EEG were recorded (tACS electrodes)--> quantify potential tACS effects on oscillatory brain activity.  EEG data obtained before and after tACS were downsampled to 250 Hz.
Data Analysis:

*Other measures: None included participants showed signs of clinical anxiety or depression (Hospital Anxiety and Depression Scale). 3 questions were asked during the experiment: page 1260 (or 5). 

## ploner nickel pnas
*Name: Temporal-spectral signaling of sensory information and expectations in the cerebral processing of pain
*Link: https://osf.io/jw8rv/
*Paper: 10.1073/pnas.2116616119 
*Participants: 48 healthy, recruited through advertisements→ were age above 18 and right-handedness, 23 females, age: 23.7 ± 3.4 y. 
*Pain condition:  dorsum of the left hand using a neodymium yttrium aluminum perovskite laser, 1,340 nm, a pulse duration of 4 ms, and a spot diameter of ∼7 mm. Stimulus intensity→ 3.5 J for hi stimuli and 3 J for li + site was slightly changed. 
*Measures: two noxious heat stimulus intensities (hi and li) and two visual cues (HE and LE) resulting in four experimental conditions. HE cues→ followed by hi 75% of trials (hiHE) + li, 25% of trials (liHE);  LE cue→ 75% of trials (liLE) and by hi stimuli in 25% of trials. 2 × 2 factorial design. After the offset of the cue presentation, a brief painful heat stimulus was applied→ Rate the perceived pain intensity, numerical rating scale ranging from 0 to 100. 
	-Quantified brain activity before the painful stimulus, including the stimulus preceding negativity [SPN (29)] and oscillatory activity at alpha and beta frequencies.
*Other measures: Average clinical anxiety and depression scores (Hospital Anxiety and Depression Scale); 10 heat stimuli with different intensities to familiarize. EEG data were recorded using actiCAP snap/ slim with 64 active sensors (Easycap) placed according 10-20 system and BrainAmp MR plus amplifiers (N1, N2, and P2 components; alpha, beta, gamma), Skin conductance→ two Ag/AgCl electrodes attached to the palmar distal phalanges of the left index and middle finger; prestimulus differences in oscillatory brain activity induced by the expectation of hi or li stimuli; PEs, etc. 


## ploner dinh chronic pain pain
*Name:Brain dysfunction in chronic pain patients assessed by resting-state electroencephalography. 
*Link: https://osf.io/hbkms/
*Paper: https://pubmed.ncbi.nlm.nih.gov/31356455/ 
*Participants: 101 patients suffering from chronic pain (age 58.2 ± 13.5 years, 69 F)+ 84 age- and sex-matched healthy control participants (age 57.8 ± 14.6 years, 55 F). Pain at least 6 months and a min. Pain intensity ≥4/10 during the past 4 weeks. Patients on medication with benzodiazepines = excluded, other medication was not restricted+maintained. 
*Pain condition: Chronic pain→ 47 back pain, 30 widespread pain, 6 joint pain, 5 unspecific neuropathic pain, 7 postherpetic neuralgia, 6 polyneuropathic pain.
*Measures: Brain activity→ EEG during resting state, with eyes closed and open for 5 minutes each. 64 electrodes+ 2 below anthus of each eye+ BrainAmp MR plus amplifiers. 
	-Two categories of analyses were performed, based on 2-second epochs of resting-state data: 1. local, ie, spatially specific→ obtained for every electrode, voxel, or brain region; included comparisons of power topographies on electrode level and comparisons of connectivity and local network measures topographies. 2. global, ie, spatially holistic→ average across all electrodes, voxels, or brain regions, ie, the peak frequency, the power spectrum, and all global network measures. 
*Other measures: short-form McGill pain Questionnaire, Pain Disability Index, painDETECT (PDQ), Beck Depression Inventory II (BDI-II), State-Trait-Anxiety Inventory, and the Veteran's RAND 12-Item Health Survey (VR-12)--> before EEG. Brain activity analysis: analyzed in electrode space; Connectivity analysis: source space (PLV, dwPLI, AEC); topographical maps of brain activity for theta, alpha, beta, and gamma. 


## ploner 1/f elife
*Name: Assessing the balance between excitation and inhibition in chronic pain through the aperiodic component of EEG
*Link: https://osf.io/qgfma/
*Paper: https://pmc.ncbi.nlm.nih.gov/articles/PMC11729367/ 
*Participants: 149 with chronic pain+ 115 healthy. 
*Pain condition: Dataset 1→ 101 people with different chronic pain + 88 healthy= three different cohorts. 
-First one: 20 chronic widespread pain + 22 healthy. 
-Second: 34 chronic back pain. 
-Third: 47 chronic pain + 66 healthy. 
Dataset 2→ longitudinal, 50 with different types of chronic pain underwent multimodal pain therapy. Dataset 3→ 27 healthy (not been previously analyzed or published). 
People with chronic pain: 98 females and 53 males, healthy: 74 females and 41 males, with chronic pain aged 86–18, healthy aged 79–18. 
*Measures: Brain activity→ EEG during the resting state. Two blocks of 5 min each→ one eye closed and one with eyes open. This study only analyzed the eyes closed condition. The aperiodic component is a recent measure of brain activity→ two-step approach. 1. Pre-registered analyses, predefined the steps and parameters to estimate the aperiodic activity. 2. Performed a multiverse analysis (robustness of the results across different methodological ways of computing the aperiodic activity).
*Other measures: clinical and demographic questionnaires→Age, Average pain intensity (rating scale from the PainDetect questionnaire) + Clinical diagnosis. To spatially localize brain activity→ source reconstruction of the preprocessed, segmented, and band-passed filtered signals. Power spectrum computation + parametrization.


## chronic pain
*Name: EEG frequency band analysis in chronic neuropathic pain: A linear and nonlinear approach to classify pain severity
*Link: https://data.mendeley.com/datasets/yj52xrfgtz/1
*Paper: https://www.sciencedirect.com/science/article/pii/S0169260723000160#bib0024    
*Participants: 36 chronic NP, different types of chronic NP (28 F age of 44±13.98) + 22 channels were registered (250 Hz and a bandwidth of 0.1–100 Hz). Control→ 13 with no NP + 19 channels were registered (256 Hz and within a bandwidth of 0.1–100 Hz). 
*Measures: Chronic Neuropathic Pain: EEG data in eyes open (5 min) and eyes closed (5 min) with questionnaire reports, Version 3. Absolute band power and ApEn EEG features in the five clinical frequency bands (delta, theta, alpha, beta, and gamma) were estimated for all channels in both groups.
*Other measures: Pain Detect Questionnaire (PDQ) and Brief Pain Inventory (BPI), Hospital Anxiety and Depression Scale (HADS), Kruskal Wallis and post-hoc Dunn’s tests.


## Ploner longitudinal
*Name: Longitudinal resting-state electroencephalography in patients with chronic pain undergoing interdisciplinary multimodal pain therapy
*Paper:https://journals.lww.com/pain/fulltext/2022/09000/longitudinal_resting_state_electroencephalography.23.aspx
*Participants: 41 participants with chronic pain before and 6 months after interdisciplinary multimodal pain therapy (IMPT). Age 51 ± 17 years, 25 F. 26 patients predominantly suffered from chronic back pain, 8 from joint pain, 4 from peripheral neuropathic pain, and 3 from chronic widespread pain. Apart from primary headache disorders, with pain lasting more than 6 months and a minimum reported average pain intensity ≥2/10 during the past 4 weeks. 
*Pain conditions: Chronic pain.
*Measures: Pre-IMPT (in the week before or within the first 3 days of the IMPT program) and post-IMPT (between 6 and 9 months)--> resting-state EEG. 5-minute blocks were recorded, 1 with the eyes open and another with the eyes closed.
*Other measures: To differ chronic vs healthy people→ dominant peak frequency; the amplitudes of neuronal oscillations at theta, alpha, beta, and gamma frequencies; graph theory-based measures of brain network organization. Pain intensity was assessed using a Numerical Rating Scale. Physical functioning→ focus on pain interference using the Pain Disability Index (simple seven-item questionnaire, rate their pain-related impairment in the domains “Family/Home responsibilities,” “Recreation,” “Social Activity,” “Occupation,” “Sexual Behavior,” “Self-Care,” as well as “Life-Support Activity” on a scale from 0 to 10. Depressive symptoms→ Beck Depression Inventory II.


Investigate:  
*Name: Multimodal Pain Dataset
*Paper: https://data.mendeley.com/datasets/mf2cgph9cy/4 
*Participants: 99 participants, self-reporting system + bio-signals
*Pain condition:  3 conditions → headache, back pain, and menstrual pain.
*Measures: EEG + wristband signals (EDA, BVP, temperature, accelerometer data), responses to a survey (including McGill Pain Questionnaire). Pain condition → E4 Empatica wristband and Mindware Mobile 2 EEG device (collect data).


## Other non-pain relevant datasets

The HBN-EEG Dataset
*Name: HBN-EEG: The FAIR implementation of the Healthy Brain Network (HBN) electroencephalography dataset
*Link: https://openneuro.org/datasets/ds005514/versions/1.0.1
*Paper: https://doi.org/10.1101/2024.10.03.615261 
*Participants: ∼5,000 children and young adults between the ages of 5 and 21, New York City area. 35% female, with a median age of 10.38 years, and mainly right-handed, with a median Edinburgh Handedness Questionnaire (EHQ) score of 76.7.
*Pain condition: none.
*Measures: HBN-EEG, the “analysis-ready” data from its high-density (128-channel) EEG, formatted as Brain Imaging Data Structure (BIDS) datasets. Includes behavioral and task-condition events annotated using Hierarchical Event Descriptors (HED)--> Six tasks, three with no participant behavioral input (passive tasks) and three including button press responses following task instructions (active tasks). 
	-Dark room, viewing a computer screen + a pre-recorded voice instructed them to hold their eyes closed or open. Passive tasks: Resting State, Surround Suppression, and Movie Watching (four short films of different types). Active tasks (mouse click responses): included Sequence Learning, Contrast Change Detection, and Symbol Search.
	- The six tasks were administered by a Linux workstation running Psychtoolbox.
	- Movie Watching: final passive tasks. (1) ‘Despicable Me’, (2) ‘Diary of a Wimpy Kid’, (3) ‘Fun with Fractals’, and (4) ‘The Present’. 
	-Contrast Change Detection: two co-centric flickering grated disks. One of the two flickering grated disks on the screen would change the contrast. Participants were asked to identify the left-leaning or right-leaning grated disks with dominant contrast as soon as they could identify the disk. Based on their responses, feedback (a smiley face or sad face) was presented. 
	- Sequence learning: shown a sequence of 10 flashed circles among 8 (or 6) possible and predetermined targets positioned on the periphery of a larger invisible circle on the screen. 5 times. 
	- Symbol search: emulation of a standard neuropsychological test on the computer screen, in which participants were asked to confirm if either of the target symbols in each row were present in the five search symbols present in the same row.
*Other measures: eye-tracking and behavioral data, cognitive and psychiatric assessments, and genetic and phenotypic data batteries collected→ EEG, eye tracking, physiological measures (respiratory belt, electrocardiogram, electromyography, electrodermal activity), voice and video recordings, actigraphy, body motion tracking, and using tablets for digital tracing.
	-Psychopathology factors: Child Behavior Checklist (CBCL). Internalizing and externalizing.

TDBRAIN dataset
*Name: The two decades brainclinics research archive for insights in neurophysiology (TDBRAIN) database
*Link: https://www.brainclinics.com/resources/tdbrain-dataset
*Paper: https://www.nature.com/articles/s41597-022-01409-z 
*Participants: 1274 psychiatric patients (collected between 2001 to 2021), 620 F, age 38.67 ± 19.21. Indications included → Major Depressive Disorder (N=426), attention deficit hyperactivity disorder (N=271), Subjective Memory Complaints (N=119), and obsessive-compulsive disorder (N=75).
*Measures: EEG to identify neurological or psychiatric dysfunction or to predict treatment response→ use of AI could identify sex, neurological EEG pathology, or response to different types of therapy. Resting-state (2-minute EO + 2-minute EC), raw EEG-data.
	-Data to investigate or replicate both diagnostic (ADHD, MDD, OCD) as well as prognostic biomarkers (rTMS, neurofeedback).
*Other measures: Demographic (gender, age, height, weight, sleep, education, alcohol and drug use), personality (​​NEO-FFI) and day measurement data included in the database. Behavioral measures (reaction-times and responses) are included for an auditory oddball task and a visual 1-back memory task, that were performed after the resting state conditions. Autonomic measures such as electro-cardiography. The ECG, measured at the clervical bone (Erbs) as well as the electromyogram (EMG, at the right masseter muscle) were recorded. 

LEMON dataset
*Name: A mind-brain-body dataset of MRI, EEG, cognition, emotion, and peripheral physiology in young and old adults
*Link: https://fcon_1000.projects.nitrc.org/indi/retro/MPI_LEMON.html 
*Paper: https://www.nature.com/articles/sdata2018308 
*Participants: 227 healthy. Two groups→ young (153, 25.1±3.1 years, range 20–35 years, 45 female) + elderly (N=74, 67.6±4.7 years, range 59–77 years, 37 female). Leipzig, Germany.
*Measures: mind-body-emotion interactions. 2 assessment days (4 hours each)--> Day 1. cognitive test battery, MRI scanning, blood pressure and anthropometric measurements + blood sample. Day 2. Resting-state EEG + psychological assessment (emotion and personality test battery and a psychiatric interview). 3rd occasion of blood pressure, Future Time Perspective questionnaire, Multidimensional Mood State Questionnaire. 
	-Cognitive Test Battery: six cognitive tests in a fixed order. 1. CVLT→ verbal learning and memory capacity. 2. TAP version 2.3.1→ Mistakes, omissions, and reaction times = measures of performance. 3. TMT→ cognitive flexibility (substests TMT-A + TMT-B). 4. WST→ verbal intelligence level and the assessment of language comprehension (crystallized intelligence). 5. Subtest 3 of the “Leistungsprüfsystem 2” (LPS-2)--> logical or inferential thinking and quantifies fluid intelligence. 6. Regensburger Wortflüssigkeitstest (RWT)--> verbal fluency. 

On day 2: electronic version of 18 emotion-related questionnaires. NEO-FF, UPPS, Behavioral Inhibition and Approach System (BIS/BAS), Emotion Regulation Questionnaire (ERQ), Cognitive Emotion Regulation Questionnaire (CERQ), Affect Regulation Style (MARS), Social Support Questionnaire (F-SozU K-22), Multidimensional Scale of Perceived Social Support (MSPSS), Brief COPE, Optimism Pessimism Questionnaire-Revised (LOT-R), Perceived Stress Questionnaire (PSQ), Trier Inventory of Chronic Stress (TICS), Eating Behavior (FEV), Addicted Eating Behavior (YFAS), TEIQue-SF, STAI-G-X2, STAXI, Toronto-Alexithymia Scale (TAS), MDBF, FTP, NYC-Q.
	-(!!!)
-Physiological data: MRI. During rs-fMRI (resting), EEG, pulse, blood pressure + respiration were recorded, MDBF before + NYC-Q after.

*Other measures: The Multidimensional Mood State Questionnaire (administered on each day); New York Cognition Questionnaire (after MRI scanning); The questionnaire of Future Time Perspective (during LEMON Rounds 1-3 only at the beginning). Assessment of Past and Present Psychiatric Symptoms (second day); Hamilton Depression Scale; Screening for Alcohol Abuse (last 28 days)--> Time Line Follow Back Questionnaire + The Alcohol Use Disorder Identification Test (alcohol abuse). Screening for Substance Abuse→ “Multi 8/2 Drogen-Tauchtest”.

-Additional Measures: Seated Resting Blood Pressure; Peripheral Blood Sample Collection and Analysis; Anthropometry; Hair Sample.



HBN-EEG Databasets
*Name:HBN-EEG: Healthy Brain Network EEG Datasets
*Link:https://neuromechanist.github.io/data/hbn/#:~:text=Overview,Brain%20Network%20(HBN)%20project 
*Participants: 3000 participants aged between 5-21 yo. 
*Measures: 
-annotations using Hierarchical Event Descriptors (HED)--> ideal for large-scale analyses and machine-learning inference related to child and adolescent mental health.
-11 dataset releases in the ​​Brain Imaging Data Structure (BIDS) format→ EEG (passive, task-based with behavioral input) + behavioral data (reaction times and accuracy are integrated with EEG events for streamlined analysis) from different participants performing the same tasks. 
*Tasks: six distinct tasks, categorized into passive and active tasks
1.Passive
-Resting state→ alternate between eyes-closed and eyes-open periods. This baseline condition allows researchers to measure spontaneous brain activity without external task demands.
-​​Surround Suppression: four flashing peripheral disks presented against contrasting backgrounds across two ~3.6-minute runs→ tests how the brain processes competing visual information when foreground and background elements have different contrast properties. Synchronized with behavioral recordings to ensure precise event timing.
-Movie: four themed (‘Despicable Me’, ‘Diary of a Wimpy Kid’, ‘Fun with Fractals’, ‘The Present’) w EEG→ captures brain responses to complex, dynamic visual and auditory content, providing insights into neural processing during realistic media consumption.
2.Active
-Contrast Change Detection: monitored two co-centric flickering grated disks + identified which disk showed increased contrast w immediate feedback (smiley or sad face). Measures visual attention, decision-making, and contrast sensitivity.
-Sequence Learning: memorized sequences of flashed circles positioned around an invisible circle’s periphery (10 circles for ≥8 years, 7 for younger children→ 8 or 6 possible targets). Viewing each sequence five times + reproducing w computer mouse. Testing visuospatial memory and motor learning.
-Symbol Search: performed a computerized version of the WISC-IV, searching for target symbols within rows of five search symbols. They worked through 15-row sequences, advancing to new sets after completing all rows. Visual processing speed, attention to detail, and symbol recognition abilities.
*Other measures: Child Behavior Checklist questionnaires (psychometric bi-factors (p-factor, internalizing, externalizing, attention)); each dataset release includes quality control checks to ensure data integrity→ checks for data length, sampling frequency, and event marker availability. 

Platform updates and future features:
Personalized Electrode Locations: more precise electrode location files tailored to each participant’s head anatomy.
Eye-Tracking Data: synchronized eye-tracking data to provide a better understanding of attention and visual behaviors during EEG tasks.
Lead Field Matrix: releasing customized lead-field matrices for source imaging analyses.


HBN-EEG Databasets (additional information)
*Name: HBN-EEG: The FAIR implementation of the Healthy Brain Network (HBN) electroencephalography dataset
*Link:https://neuromechanist.github.io/data/hbn/#:~:text=Overview,Brain%20Network%20(HBN)%20project 
*Paper: https://www.biorxiv.org/content/10.1101/2024.10.03.615261v2 
*Participants: ~5,000 children and young adults between the ages of 5 and 21 (median age of 10.38 years). More than 2,600 participants is freely available on NEMAR.
*Measures: 128 electrodes EEG. HBN-EEG sessions include six tasks, three with no participant behavioral input (passive) and three including button press responses following task instructions (active); annotations describing each of these event markers using Hierarchical Event Descriptors (HED). 
	- used nine model-based reliability indices to evaluate the bifactor models.
	-Sequence learning: The timestamps of this response were not recorded. Because of the difference in the target and sequence counts, we divided this task into two tasks: a six-target task, and an eight-target task.
	-Symbol search: confirm if either of the target symbols in each row were present in the five search symbols present in the same row. The test was presented to the participants in 15-row sequences, and participants were asked to go to the next set of sequences once they responded to all 15 rows. 
*Other measures: 1. four psychopathology dimensions (internalizing, externalizing, attention, and p-factor) derived from a bifactor model of questionnaire data→ Child Behavior Checklist, selected the McElroy et al., 2018 model, containing 66 items and four factors; 
2. eye tracking, physiological measures (respiratory belt, electrocardiogram, electromyography, electrodermal activity), voice and video recordings, actigraphy, body motion tracking, and using tablets for digital tracing; 
3. Photogrammetric scans of participant electrode locations were recorded at the end of the sessions of ~2,200 participants; quality checks;
4.Edinburgh Handedness Questionnaire (EHQ); 


Future development:
5. High-density leadfield matrix: There has been a significant effort to use the structural MRI scans of each HBN participant to create personalized computational head models and lead-field matrix for EEG source imaging. The personal lead-field matrix will help determine the sources of EEG signals with centimeter accuracy;
6. Skull conductivity estimation




