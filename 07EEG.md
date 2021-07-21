# iEEG

intracranial electroencephalography

Advantage
- directly measures neuronal population activity
- high temporal resolution , ms
- high spatial resolution , mm
- high signal to noise ratio
- low susceptibility to artifacts from patient movement

# ECoG

electrocorticography

Method
- electrodes placed directly on brain surface
- electrical stimulation mapping
- local cooling

# sEEG

stereo electroencephalography

Method
- electrode implanted deep within brain tissue
- electrical stimulation mapping
- local cooling

# Acute Intraoperative Experimentation

Intraoperative electrical stimulation to localize cortical tissue that should not be resected.

Advantage
- variety of recording devices
- devices can be repositioned during procedure

Limitation
- procedure duration less than 30 minutes , so experiment must be concluded within that time frame
- ambient noise
- magnetic interference

# Electrical Stimulation Mapping

A cortical site's function is temporarily disrupted with an electrical input.

Observed effects include
- auditory sensation
- attenuation
- speech processing deficit
- vestibular symptoms

Limitation
- can evoke seizure

# Focal Cortical Cooling

Blocks synaptic transmission.

Advantage
- effect is highly localized
- no risk of seizure

Limitation
- only performed intraoperatively

# Chronic Invasive Monitoring

Electrodes record activity for 1 to 2 weeks.

Advantage
- large surface area coverage
- longer duration for experimentation
- simultaneous recording from various cortical regions
- auditory activity can be researched during electrode removal and resection

Limitation
- substantial imaging artifacts
- implant causes medial displacement of the hemisphere
- head positioning during pre and post operative imaging is not identical

# Recorded Data

**Evoked Activity**

Averaged Evoked Potential (AEP)
- time and phase locked to the stimulus

Event Related Band Power (ERBP)
- time locked to stimulus

**Procedure**

- compute spectrogram for each trial's local field potential
- log transform normalization to a pre stimulus baseline
- average across trials
- compute normalized power envelopes for each frequency band

# Experimental Paradigms

**Trial Based**

Same stimulus presented multiple times. Responses are averaged.

Limitation
- habituation
- fatigue

<hr>

# EEG

electroencephalography

Records electrical activity.

Channels
- 128 electrodes
- 256 electrodes for a dense array

Sensitivity
- tangential sources (sulci)
- radial sources (gyri)

**Power Spectrum**

|Frequency|Hz|
|--|--|
|Delta|1 to 4|
|Theta|4 to 8|
|Alpha|8 to 14|
|Beta|14 to 30|
|Gamma|30 to 70|
|High Gamma|70 to 150|

# MEG

magnetic encephalography

Records magnetic fields.

Channels
- 200 to 300 sensors

Sensitivity
- tangential sources

Selectivity
- activity in cortical sulci

# Forward Problem

Calculation of scalp electrical field.

# Inverse Problem

Calculation of which neuronal populations generated the field.

# Independent Component Analysis

Statistical method for reducing number of signals from numerous channels to a minimum number of independent signals.

# Functional Connectivity

Statistical association between 2 signals.

Methods
- phase locking value

# Effective Connectivity

Causal association between systems.

Methods
- dynamic causal modeling
- granger causality

# Cross Frequency Coupling

Identifying connections between locations based on similar patterns from their individual recordings.

- power to power coupling : magnitude is consistent but frequency is different
- phase to phase coupling : phase is consistent between both regions but something else changes.

# Activity

**Evoked**

Locked to stimuli
- phase locked : response peaks occur at same time from one stimulus presentation to the next stimulus presentation
- temporal locked

Noise can be reduced by averaging.

**Induced**

Occur after the stimuli and has no phase locking.

Represents stimulus modulation of brain activity.

Requires non linear analysis prior to averaging.
