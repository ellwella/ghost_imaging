# Ghost imaging literature notes
Ghost imaging could provide high-resolution imaging for wavelengths where quality is scarce.
This process is comparatively cheap and more efficient.
## J Shapiro, 2008
### Classical (non-computational) ghost imaging
Two beams. One hits object- light is collected by a single pixel detector. One passes through a high-resolution detector and does not touch the object.
### Computational ghost imaging (CGI)
Abandons the use of a reference beam.  
Light is shone through an SLM in a sequence of different modulations.
The bucket detector record an intensity value for each of these events from the backscatter.  
Each SLM pattern is weighted by the brightness in the reconstruction.  
Iterating over many patterns allows the build-up of an accurate reconstructive image.
**Benefits:** no high-spatial detector required
#### 3D sectioning: 
The computational element means ∆I is calculated for a propagating wave. The computer can pre-predict the change in intensity for a different distance.   
Upon image reconstruction, the series of bucket detections is compared to pre-programmed pattern at many distance values. Stacking these gives a 3D sectioning with depth.  
The collection of intensities from the SLM can be reused for all ghost images of that system.  
## Padgett and Boyd, 2017
This paper is about classical ghost imaging, rather than computational ghost imaging.
### Correlated photons
Initial experiments were purely quantum: a single photon is PDC’d into ‘signal’ and ‘idler’ photons which are correlated. Correlation between these photons was used for imaging without physical interactions.  
Whilst these photons are entangled, ghost imaging only makes use of spatial correlation of photon pairs.  
The idler photon is incident on the object. The signal photon is only measured if the idler photon is detected.  
These pumped photons are emitted across a 2D crystal meaning a ‘shadow’ of the object can be formed by taking many intensity values. The idler photon is either transmitted/reflected (recorded) or blocked/absorbed (not recorded)
### Klyshko (back-projection) model
Replace bucket detector with a light source, and the crystal with a mirror (reverse order).  
The light profile from the object is reflected off of the mirror and captured by a camera (like holography)  
Spatial coherence is of paramount importance as it has drastic effects on resolution.
This is analogous to the single (scalar) intensity detection of the photons, allowing a high contrast.  
### Making use of entanglement  
For ghost imaging, the two photons must be spatially correlated. This is something a classical source could reproduce.  
For the quantum scenario, position is correlated and momentum is anti-correlated (conservation). Only a quantum setup can demonstrate the correlation between the two complementary variables.  
Due to the momentum anticorrelation, position in the far field will also be anticorrelated. As such, placing the object and detector in the far field produces an inverted image- something that classical correlations can not reproduce.
### Improvements to ghost imaging
Non-degenerate wavelengths: signal and idler photons can be made to have different wavelengths. Allows detection with visible light, but illumination with another
Detector arrays: the whole FOV can be captured using an array of single-element detectors. The high-gain is switched on during the window you can anticipate a photon being incident.  
Zeilinger’s interference approach: the interference between two PDC crystals’ photons. Blocking or shifting one idler beam affects the image produced due to change in interference.  
Quantum-secured imaging: encoding photons with polarisation info means we can verify that they have not been tampered with.  
Noise-suppression: recording the image of the idler and signal beams such that the ratio of the two suppresses noise.
### Low photon numbers
Images that are very distinct from one another (high orthogonality) required very few photons to tell them apart reliably. However, for intensity-based detection (no phase), differentiation is less reliable- more photons needed.   
Low photon number gives rise to larger statistical randomness (noise).
### Classical correlations
It was then ascertained that these same correlations could be made with classical (non-quantum) systems by using a beam splitter.
In short, single photon (quantum) and many-photon (classical) systems can be used for ghost imaging. The latter is limited by statistical fluctuations (Poisson) in photon numbers.   
A speckled filter continuously randomises the modulation of light.  
A resulting image sums over these random patterns, weighting them by detected intensity.   
## Glossary
**SLM:** Spatial light modulators. Spatially control light features. Allows wavefront manipulation.  
**Bucket detector:** a single-pixel detector that records the total light intensity of an event. Does not give any spatial variety.  
**Parametric down-conversion:** nonlinear process in which high-energy photons is converted into a pair of entangled (correlated) photons  
**Entangled photons:** pairs of particles that have interlinked quantum states, regardless of positions. Measuring one gives information about the partner   
**Orthogonality:** angular relation/ how perpendicular two planes are(geometric) or the degree of independence

