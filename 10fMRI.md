# fMRI 1 Basics

- pixel : 2d point on one slice
- voxel : 3d cube on stack of slices
  for anatomical accuracy get voxel as small as possible
  for connectivity measure voxel as many times as possible
- spatial resolution : in plane resolution (pixel size) and depth (slice distance)
  usually 1mm isotropic

- cortex - 1mm thick
  gray matter : cell bodies
  white matter : axons

**Anatomical Imaging**

3 dimensions
1 mm x 1 mm x 1 mm voxel
5 minutes to take 176 slices , 20 minutes if DTI
Adequate for most anatomical imaging.

Higher resolution imaging requires more time. .5 mm is possible as is .2 mm.
Approaching .2 mm increases the signal to noise ratio due to positional disturbances from circulating blood flow motion. Highest resolutions are achieved from cadavers as scanning can be left to run for hours exceeding live tolerances and there are no motional disturbances from the cadaver.

**Functional Imaging**

4 dimensions
1 mm x 1 mm x 1 mm voxel x 2 s
To achieve 5 minutes for one voxel spatial resolution can be 3 x 3 x 3 for 30 slices and 2s for temporal resolution. This results in a voxel that is 27 times larger than the 1 x 1 x 1 voxel. This sacrifices spatial resolution for temporal resolution.

Temporal resolution is time needed to return to the same slice.

Neural activity occurs at around 3ms.

Parameters
- temporal resolution
- spatial resolution
- coverage (slices)

# fMRI Timecourse

Within a 1mm x 1mm x 1mm voxel there are hundreds of thousands of neurons.

Average neural activity can be detected but which types of neurons are firing cannot be determined.

**Hemodynamic Response Function**

- An increase in neural activity depletes the local oxygen supply (initial dip).
- Body overcompensates with a slow and higher replenishment of oxygen at the site. This occurs 4s to 6s after stimuli presentation.
- As oxygen levels return to baseline they dip slightly below baseline before returning fully to baseline (overshoot).

Concerns
- Distinguishing between local capillaries and transport vessels.
  Large blood vessels within a voxel could simply be carrying blood to a distant site and not terminate at the voxel of interest.

In the primary visual cortex in regards to orientation pinwheels , astrocytes have a one to one orientation with neurons in which its dendrite receives the same input as the neuron and its output wraps around a blood vessel. This allows for precise control of blood flow to that neuron in direct response to an input signal directed at that neuron.

The standard generic HRF may be inadequate for groups such as the elderly and non neurotypical populations but may be sufficiently adequate without alterations for standard studies.

- alpha : time to peak
- beta : peak

![hrf](hrf.png)





---

# MRI
tomography
high spatial resolution

Areas of increased oxygenated blood flow indicate increased neuronal activation as activated cells require more oxygen.

Measures BOLD signal.
- base line signal
- stimulus presentation
- slight dip in signal
- high signal overshoot
- level signal
- stimulus removed
- signal undershoot
- return to baseline signal

# Experiment

Series of scans and continuous tasks.

**Block Design**

Stimuli grouped into blocks.
- control 1 block
- task another block

**Event Related Design**

Stimuli presented separately in random order.

# Data Analysis

**logic of activation**

**multiple comparisons problem**

Repeated testing of same data set increases false positives due to setting significance level at 5%.

Make sure to use correction methods to minimize this issue.

# pharmaco FMRI

- Administer drug that blocks receptor.
- Compare treatment vs non treatment tasks.

Memantine blocks glutamate action on NMDA receptor sites.

**Cross Over Design**

Split into 2 equal groups.
- treatment + no treatment
- no treatment + treatment
