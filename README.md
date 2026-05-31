TITLE <br>
Rocket Fin Bending Vibration Analysis <br>

Objective: Evaluate the dynamic response of a rocket fin subjected to aerodynamic and propulsion-induced excitation. <br>

Methodology: In this code, a fin has been modelled as a cantilevered beam using Euler-Bernoulli beam theory. Modal analysis was performed to determine the natural frequencies and mode shapes of the structure. The dynamic behaviour of the fin was further investigated through frequency response analysis and damped transient vibration simulations to evaluate resonance characteristics under aerodynamic and propulsion-induced vibration. <br>

Software used are Python, NumPy, SciPy and Matplotlib. <br>

Fin Properties: <br>
	Length:          150.0 mm <br>
	Chord:           80.0 mm <br>
	Thickness:       3.0 mm <br>
	Material:        Aluminum (ρ = 2700 kg/m³, E = 70 GPa) <br>
	Second moment I: 1.800e-10 m⁴ <br>
	Mass per length: 0.648 kg/m <br>

Governing Equation: <br>
The code is based on Euler-Bernoulli beam theory:

EI (∂^4 w)/(∂x^4 )+ρA (∂^2 w)/(∂t^2 )=0

Where the rocket fin was approximated as a uniform cantilever beam and analysed using the aforementioned formula. <br>
Here, w(x,t) = Lateral deflection of the beam as a function of position and time, <br>
EI = Flexural rigidity of the beam (Young’s modulus x second moment of area), <br>
A = Area of cross section of the beam, <br>
ρ = Density of the beam. <br>


Results:  <br>
1. Mode Shapes: The first five bending modes were successfully extracted, with the fundamental bending mode occurring at 109.67 Hz and higher modes occurring at progressively larger frequencies. <br>
2. FRF: Frequency response function showing resonance amplification and damping effects under harmonic excitation. <br> 
3. Transient Response: Time-domain damped free vibration response lasting for a duration of 300 milliseconds following an imposed maximum initial tip displacement of 1mm. <br>
4. Natural Frequencies: Calculated bending eigenfrequencies used to assess resonance susceptibility and structural dynamic performance. <br>

Engineering Findings: <br>
	1. First natural frequency = 109.67Hz <br>
	2. Forced response identified at 98.7Hz, close to the first natural frequency of 109.67 Hz, demonstrating the sensitivity of the structure to resonance excitation. <br>
	3. Maximum tip displacement = 4.508mm <br>
	4. The first bending mode dominated the dynamic response, while higher-order modes exhibited reduced contribution to overall tip displacement under typical vibration conditions. <br>

Conclusion: <br>
	1. Developed a computational structural dynamics model to analyze bending vibration characteristics of rocket fin structures using Python, NumPy, SciPy, and Matplotlib. <br>
	2. Implemented cantilever beam modal analysis to calculate natural frequencies, mode shapes, transient response, and forced harmonic vibration behavior. <br>
	3. Simulated damped and forced vibrational response using modal superposition techniques and frequency response functions relevant to aerospace structural resonance analysis. <br> 
	4. Generated engineering visualizations including mode shapes, frequency response plots, transient vibration decay, and resonance characteristics for structural dynamic assessment. <br>

Engineering Significance: <br>
Rocket fins are subjected to aerodynamic forcing, engine-induced vibration, and transient loading throughout flight. If excitation frequencies approach the natural frequencies of the fin, resonance may result in excessive vibration amplitudes and potential structural failure. The present study demonstrates how modal analysis and frequency response techniques can be used during preliminary design stages to identify critical frequencies and evaluate the effectiveness of structural damping. <br>

Future Work: <br>
1. Validation using FEA modal analysis in ANSYS. <br>
2. Investigation of carbon-fibre reinforced composite fins under similar loading conditions. <br>
3. Comparative study of Aluminium and Composite Fin configurations dynamic performance. <br>
4. Investigation of the interaction of aeroelastic coupling with aerodynamic loading. <br>
5. Structural optimization for minimum mass and maximum stiffness. <br>
6. Extension to transient launch and propulsion-induced loading environments. <br>

Key skills demonstrated: Structural dynamics, modal analysis, numerical methods, scientific computing (Python), aerospace structures, vibration analysis, engineering data visualization. <br>
