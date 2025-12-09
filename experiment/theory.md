## Theory

 Pressure gauges are essential instruments for measuring fluid pressure accurately in industrial, scientific, and engineering applications. However, their readings can drift over time due to mechanical wear, environmental factors, or material fatigue, which can potentially lead to unsafe or unreliable outcomes. To maintain precision, gauges must be periodically calibrated against a primary standard of measurement. One of the most common methods for calibrating a pressure gauge is the use of a dead-weight tester. This instrument generates a known pressure by applying accurately calibrated weights to a piston of known cross-sectional area. The pressure is transmitted through an incompressible fluid (usually oil), ensuring that the force applied is entirely converted into fluid pressure. The dead-weight tester operates on the fundamental hydrostatic principle that a known force applied over a precise area generates a predictable pressure. Weights of calibrated masses are stacked on a free-floating piston immersed in a cylinder filled with oil. The downward gravitational force from these weights balances the upward hydrostatic force from the pressurized oil, achieving equilibrium when:

$$Pressure = \frac{F}{A} \tag{1}$$ 

$$F = M g \tag{2}$$

where,

<span style="font-family:'Bodoni MT';font-style:italic">F</span> = force applied to the liquid in the calibrator cylinder in Newton (N);

<span style="font-family:'Bodoni MT';font-style:italic">M</span> = Total mass including the mass of the piston in kilograms (kg);

<span style="font-family:'Bodoni MT';font-style:italic">A</span> = cross-sectional area of the piston in square meter (m<sup>2</sup>);

<span style="font-family:'Calibri';font-style:italic">g</span> = Acceleration due to gravity in meter per second square (m/s<sup>2</sup>).

Therefore, for each weight added, the pressure transmitted within the oil in the dead weight tester is calculated using the above formula, as the area of the piston in the tester is accurately known. Thus, by knowing <span style="font-family:'Bodoni MT';font-style:italic">M</span> and <span style="font-family:'Bodoni MT';font-style:italic">A</span>, the applied pressure can be precisely calculated. A typical dead-weight tester consists of an oil reservoir, a piston-cylinder assembly, a set of calibrated weights, a plunger, and a gauge connection port. The oil reservoir contains the working fluid, usually oil, which transmits pressure throughout the system. The piston-cylinder assembly converts the applied mass into fluid pressure, while the calibrated weights generate known forces when placed on the piston. The punger is used to fine-tune and stabilize the pressure within the system, ensuring precise calibration conditions. The gauge connection port provides an interface for attaching the pressure gauge that needs to be calibrated. The entire system is filled with clean oil, and the piston is carefully adjusted to float freely, minimizing friction and enhancing measurement accuracy. Fig. 1 illustrates the schematic diagram of a dead weight tester used for calibrating a pressure gauge. Fig. 2 shows the image of a real pressure gauge used for practical applications.
 

<div align="center">				
<img alt="" src="./images/plantscth.png" style="width:80%">

<b>Fig.1. Schematic of Dead Weight Tester</b>
</div>

During calibration, the system is first primed with oil to remove any trapped air and ensure the fluid remains incompressible. Calibrated weights are then placed on the piston to generate known pressures within the system. The plunger is moved gradually until the piston reaches equilibrium neither rising nor falling indicating that the pressure applied by the weights is balanced by the fluid pressure. Once equilibrium is achieved, the corresponding pressure gauge reading is recorded. This process is repeated for a series of increasing and then decreasing loads to evaluate the gauge’s accuracy and to check for hysteresis effects. Throughout the procedure, the piston-weight assembly is allowed to rotate, which helps reduce viscous friction between the piston and the cylinder walls, thereby improving the precision and consistency of the calibration.

Even in a precisely designed tester, small errors arise due to several factors:

Gravitational variation: In a dead-weight tester, the applied force used to generate pressure is defined as the product of the true mass and the local acceleration due to gravity. Since gravitational acceleration is not constant and can vary over the Earth’s surface, the gravity at the test location may differ from the gravity value used during the original calibration of the dead-weight tester. When such a difference exists, the pressure values stated in the calibration report must be corrected to obtain the actual pressure at the test site. The local acceleration due to gravity (<span style="font-family:'Calibri';font-style:italic;font-size:20px">g<sub>l</sub></span>) varies with latitude(<span style="font-family:'Bodoni MT';font-style:italic;font-size:20px">&straightphi;</span>) and elevation (<span style="font-family:'Bodoni MT';font-style:italic;font-size:20px">z</span>). It can be calculated using the following equation [Ref. 3,4]:

$$g_{l} = 9.780327 (1 + 0.0053024 sin^{2} (\phi) - 0.0000058 sin^{2} (2 \phi)) - 3.086 \times 10^{-6} \times z \tag{3}$$

A correction factor is required to account for differences between the local gravity at the test site and the reference gravity (<span style="font-family:'Calibri';font-style:italic;font-size:20px">g</span>) used during calibration. The gravity correction can be applied using:

$$e_{gravity} = \frac{g_l}{g} \tag{4}$$

<div align="center">				
<img alt="" src="./images/plantscth2.png" style="width:70%">

<b>Fig.2. Dead weight Tester (H6900, Nagman Instruments)</b>
</div>

<b>Air buoyancy:</b> The buoyant force of air slightly reduces the effective mass of the weights. The buoyancy correction is applied as:

$$e_{buoyancy} = - \frac{\rho_{air}}{\rho_{masses}} \tag{5}$$

<b>Piston friction:</b> Friction between the piston and cylinder may prevent free movement, leading to measurement lag or hysteresis.

Uncertainty in piston area: Any dimensional inaccuracy directly affects the calculated pressure.

Then the indicated pressure of the gauge, <span style="font-family:'Bodoni MT';font-style:italic">&rho;<sub>i</sub></span> , can be corrected as:

$$\rho = \rho_i (1 + e_{gravity} + e_{buoyancy}) \tag{6}$$

The least count of an instrument is the smallest value that it can measure accurately. It defines the resolution or precision of the measurement. For a pressure gauge, the least count corresponds to the minimum change in pressure that produces a noticeable change in the pointer reading. It depends on the scale range and the number of divisions on the dial. The accuracy of calibration is affected by the least count, since any pressure difference less this value cannot be reliably detected. Hence, while comparing the actual and indicated pressures, the least count should be considered to estimate the uncertainty and overall measurement accuracy.
				

						
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>								