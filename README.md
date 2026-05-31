TITLE <br>
Rocket Fin Bending Vibration Analysis
<br>
Objective: Evaluate the dynamic response of a rocket fin subjected to aerodynamic and propulsion-induced excitation.

Methodology: In this code, a fin has been modelled as a cantilevered beam using Euler-Bernoulli beam theory. Modal analysis was performed to determine the natural frequencies and mode shapes of the structure. The dynamic behaviour of the fin was further investigated through frequency response analysis and damped transient vibration simulations to evaluate resonance characteristics under aerodynamic and propulsion-induced vibration.
Software used are Python, NumPy, SciPy and Matplotlib.
Fin Properties:
	Length:          150.0 mm
	Chord:           80.0 mm
	Thickness:       3.0 mm
	Material:        Aluminum (ρ = 2700 kg/m³, E = 70 GPa)
	Second moment I: 1.800e-10 m⁴
	Mass per length: 0.648 kg/m

Governing Equation:
The code is based on Euler-Bernoulli beam theory:

EI (∂^4 w)/(∂x^4 )+ρA (∂^2 w)/(∂t^2 )=0

Where the rocket fin was approximated as a uniform cantilever beam and analysed using the aforementioned formula.
Here, w(x,t) = Lateral deflection of the beam as a function of position and time,
EI = Flexural rigidity of the beam (Young’s modulus x second moment of area),
A = Area of cross section of the beam,
ρ = Density of the beam.


Results:  
	Mode Shapes: The first five bending modes were successfully extracted, with the fundamental bending mode occurring at 109.67 Hz and higher modes occurring at progressively larger frequencies.
	FRF: Frequency response function showing resonance amplification and damping effects under harmonic excitation. 
	Transient Response: Time-domain damped free vibration response lasting for a duration of 300 milliseconds following an imposed maximum initial tip displacement of 1mm. 
	Natural Frequencies: Calculated bending eigenfrequencies used to assess resonance susceptibility and structural dynamic performance.

Engineering Findings: 
	First natural frequency = 109.67Hz
	Forced response identified at 98.7Hz, close to the first natural frequency of 109.67 Hz, demonstrating the sensitivity of the structure to resonance excitation.
	Maximum tip displacement = 4.508mm 
	The first bending mode dominated the dynamic response, while higher-order modes exhibited reduced contribution to overall tip displacement under typical vibration conditions.
Conclusion:
	Developed a computational structural dynamics model to analyze bending vibration characteristics of rocket fin structures using Python, NumPy, SciPy, and Matplotlib.
	Implemented cantilever beam modal analysis to calculate natural frequencies, mode shapes, transient response, and forced harmonic vibration behavior.
	Simulated damped and forced vibrational response using modal superposition techniques and frequency response functions relevant to aerospace structural resonance analysis. 
	Generated engineering visualizations including mode shapes, frequency response plots, transient vibration decay, and resonance characteristics for structural dynamic assessment.

Engineering Significance:
Rocket fins are subjected to aerodynamic forcing, engine-induced vibration, and transient loading throughout flight. If excitation frequencies approach the natural frequencies of the fin, resonance may result in excessive vibration amplitudes and potential structural failure. The present study demonstrates how modal analysis and frequency response techniques can be used during preliminary design stages to identify critical frequencies and evaluate the effectiveness of structural damping.

Future Work:
	Validation using FEA modal analysis in ANSYS. 
	Investigation of carbon-fibre reinforced composite fins under similar loading conditions. 
	Comparative study of Aluminium and Composite Fin configurations dynamic performance. 
	Investigation of the interaction of aeroelastic coupling with aerodynamic loading. 
	Structural optimization for minimum mass and maximum stiffness.
	Extension to transient launch and propulsion-induced loading environments

Key skills demonstrated: Structural dynamics, modal analysis, numerical methods, scientific computing (Python), aerospace structures, vibration analysis, engineering data visualization.
