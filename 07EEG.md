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
