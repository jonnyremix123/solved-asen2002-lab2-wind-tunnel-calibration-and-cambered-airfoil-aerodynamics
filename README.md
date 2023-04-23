Download Link: https://assignmentchef.com/product/solved-asen2002-lab2-wind-tunnel-calibration-and-cambered-airfoil-aerodynamics
<br>
<h1></h1>

<ul>

 <li>Learn basic concepts and definitions associated with flow measurements, wind tunnel testing, and two-dimensional flow around airfoils.</li>

 <li>Apply the conservation of mass and Bernoulli’s equation to measure the airspeed.</li>

 <li>Observe the development of viscous boundary layers in the test-section and understand the impact they have on the airspeed in the test-section.</li>

 <li>Gain an understanding of the origins of Lift and Drag through measuring and integrating the surface pressure distribution on a cambered airfoil.</li>

 <li>Observe how changes in the Lift and Drag force coefficients are related to the angle of attack (flow incidence angle) and the free-stream velocity.</li>

 <li>Develop an awareness of sources of error and error analysis.</li>

</ul>

<h1>2       Required Deliverables</h1>

<ul>

 <li>Attendance at every lab period is recommended. Instructions for weekly tasks and the deliverables will be presented during the scheduled lab time.</li>

 <li>Prepare and present a single slide (“quad chart”) of the results. Use the guidelines that will be provided to complete your report.</li>

 <li>Prepare a written brief report (“executive summary”) of the results. Use the guidelines that will be provided to complete your report.</li>

</ul>

<h1>3      Text References</h1>

<ul>

 <li>Fundamentals: 2.1, 2.3, 2.4</li>

 <li>Conservation Equations: 4.1, 4.3</li>

 <li>Wind Tunnels and the Measurement of Velocity: 4.10, 4.11</li>

 <li>Viscous Flow and Boundary Layers: 4.15, 4.16, 4.18, 4.20, 4.21</li>

 <li>Airfoil Nomenclature and Data: 5.2, 5.4</li>

 <li>Pressure and Force Coefficients: 5.3, 5.6</li>

 <li>Obtaining Forces from Pressure: 5.7</li>

</ul>

1

“Fundamentals of Thermal Fluid Sciences” 4th ed. by Cengel, Cimbala, and Turner

<ul>

 <li>Measurements: 2-6, 2-7, 2-8</li>

</ul>

“Introduction to Error Analysis” 2nd ed. by Taylor

<ul>

 <li>Error and Uncertainty Analysis: Chapters 1-4</li>

</ul>

<h1>4     Motivation</h1>

Wind tunnels are tools utilized in the aeronautical testing world to reveal a detailed understanding of how a flowing gas physically interacts with a “stationary” test article. As with any tool you must first understand how it performs and what its limitations are before you can be confident that you have selected the appropriate tool and that the results will be accurate.

You will be using the PILOT Low-Speed Wind Tunnel regularly throughout the Smead Aerospace Engineering curriculum here at CU Boulder. Thus this laboratory assignment will serve as a foundational component in developing your fundamental understanding of how the wind tunnel performs through a “calibration” of the test-section. Specifically you will focus on understanding how the wind tunnel operates and how its speed is measured in the test-section. Then you must understand the limitations on this measurement through a detailed quantification of the uncertainty in the air-speed measurement. Additionally, it is typically assumed that the velocity throughout the test-section is uniform and constant. This is often not true! You must measure the variation in the airspeed and discover how it is governed by the fundamental theories discussed in lecture. All of this will help you as you progress through the curriculum and perform more complex measurements in the wind tunnel during this and future courses.

In addition to learning about wind tunnel basics in this lab, you will also explore the aerodynamics of a cambered airfoil. Airfoils compose the fundamental cross-sectional geometry in an aircraft’s wing and thus play a critical role in the production of lift and drag on aerodynamic vehicles. Furthermore we fundamentally understand that the pressure and shear-stress distributions on the physical surfaces of a body provide the source of all aerodynamic forces applied to that body. As a result, quantifying and integrating the pressure distribution around an airfoil geometry will provide you a fundamental understanding of the origins of lift and drag on aerodynamic vehicles.

To this end we have selected a canonical airfoil geometry, namely a cambered Clark Y-14 airfoil, which is instrumented with 19 flush mounted pressure taps around the surface. You will measure the pressure distribution on the airfoil surface for variations in angle of attack and free-stream airspeed. From this data you can then compute the resultant forces and determine the aerodynamic performance (i.e. lift and drag) of the wing section. This will fundamentally show where the aerodynamic forces originate, as well as how they depend on the flow conditions.

<h1>5        Experimental Section 1: Measurement of Airspeed</h1>

<h2>5.1        PILOT Low Speed Wind Tunnel Background</h2>

<h3>5.1.1     Configuration</h3>

The PILOT Low-Speed Wind Tunnel is an Eiffel or open-circuit suction type wind tunnel. A schematic of the wind tunnel is presented below in Figure 1. This schematic includes labels for each of the sections of the wind tunnel and nominal dimensions, in inches, from the manufacturer: Aerolab LLC.

The wind tunnel has a “closed” test-section that is nominally 12 in. by 12 in. by 24 in. long. Air is “pulled” through the test-section by a 9 bladed fan driven by a 10 HP electric motor that is located downstream from the test-section at the wind tunnel exit. It is also worth noting that the airspeed is accelerated theoretically from rest in the surrounding room into the “test-section” by way of the inlet, flow conditioners, stilling chamber, and contraction (or nozzle) that has a 9.5 to 1 area ratio. Each of these sections plays an important role in ensuring that the flow is uniform, steady, and at the right speed in the test-section.

Figure 1: Engineering drawing views of the PILOT Low-Speed Wind Tunnel. Flow is from left to right in the side view (left) drawing and out of the page in the rear (right) drawing.

<h3>5.1.2    Measurement Devices</h3>

There are a variety of different measurements that can be made in the wind tunnel. For Experimental Sections 1 and 2 of this laboratory, we will focus on quantifying the airspeed in the test-section from the direct measurement of temperature and pressure. We will use a temperature sensor, a U-tube manometer, pressure transducers, static pressure rings, and a Pitot-Static Probe to make these measurements. For Experimental Section 3 of this laboratory, airspeed and pressure distribution measurements will be required to accurately calculate the lift and drag force coefficients for the Clark Y-14 airfoil. We will use the aforementioned measurement devices as well as a Scanivalve Multi-Port pressure scanner for this section. For more details on the measurement devices used in the wind tunnel, see Appendix A.

<h3>5.1.3      Fundamental Operation of the Wind Tunnel</h3>

In future experiments you will operate the wind tunnel by commanding it to achieve a set test-section airspeed via a control program on the wind tunnel computer. The program will achieve this desired velocity through a “feed-back control system” that incorporates the computer software with wind tunnel measurement sensors and the wind tunnel fan-motor system. A general engineering schematic outlining this control system is presented in Figure 2 below. You will learn more about dynamics and control in your future courses, namely ASEN 2003, ASEN 3128, and ASEN 3200. However, there are two functions within the control system that are pertinent to the goals of this class and they are required for the control system to function properly. The first is an algorithm for calculating the airspeed from the direct measurements of the atmospheric pressure, atmospheric temperature, and the dynamic pressure in the test-section. The second is an airspeed model that converts the desired speed into a voltage input for the wind tunnel fan-motor system. These two components are critical to calibrating a new wind tunnel facility and are thus the focus of the first part of this experimental laboratory assignment. More details on each are discussed in the following.

Figure 2: Schematic of the wind tunnel feedback control system, highlighting the airspeed model and calculation functions.

For more details on the PILOT Low-Speed Wind Tunnel and the measurement devices within it, see the virtual wind tunnel walk-through presentation.

<h2>5.2      Airspeed Calculation</h2>

Unfortunately there is no way to directly measure the airspeed. Airspeed is a quantity that is typically derived from a combination of other direct measurements. This is discussed in detail in sections 4.10 and 4.11 of Introduction to Flight by Anderson. Specifically, for the PILOT Low-Speed Wind Tunnel, we can use Bernoulli’s Equation, the ideal gas law, atmospheric temperature and pressure measurements, and one of two standard airspeed measurement configurations to calculate airspeed. The first of the two airspeed measurement configurations is the Pitot-Static Probe configuration; in this configuration, airspeed can be calculated with the following equation:

The second is the Venturi Tube Configuration; in this configuration, airspeed can be calculated with the following equation:

For more information on each configuration and how to calculate airspeed, see Appendix B.

QUESTIONS TO CONSIDER: <em>How well do the two velocity measurement methods compare? Are there any differences between the velocity results? If so, what do you think is causing them? What happens as the area ratio, </em><em> , between the settling chamber and the test-section changes? Do you think there would be a benefit to having a larger or smaller area ratio, why?</em>

<h2>5.3     Airspeed Model</h2>

As highlighted above the wind tunnel airspeed is directly controlled by the fan. More specifically, as with a standard household fan the velocity in the test-section will increase with the fan rotational speed (i.e. RPM). The fan speed is driven and controlled by a 10 HP electric motor and a variable frequency speed controller. The details of how the controller operates are not critical for this laboratory assignment. What is important to understand is that the fan speed is set by a DC voltage command to the controller between a minimum of 0 volts and maximum of 10 volts. These correspond to zero RPM and the maximum safe operating RPM for the wind tunnel motor and fan assembly. In order to accurately predict the voltage required to achieve a desired velocity we need to first develop a model or a mathematical equation that relates the wind tunnel speed to the input voltage for the current ambient conditions (i.e. atmospheric pressure and temperature).

To build this model you will measure the wind tunnel airspeed at multiple fixed voltage settings distributed across the full voltage range (i.e. 0 – 10 VDC). Then you will post-process and analyze these results through applying an appropriate curve fit through the data to develop a mathematical model that relates the direct measurements (i.e. pressure and temperature) to the motor-controller command voltage. This process should be done for each of the airspeed measurement configurations and a comparison should be made.

QUESTIONS TO CONSIDER: <em>How does the velocity change with the input voltage? What type of relation best matches the response (i.e. linear, quadratic, cubic, logarithmic, etc)?</em>

<h2>5.4      Airspeed Uncertainty Analysis</h2>

Up to this point, we have discussed the measurements that we are taking as steady-state individual values with exact precision. By now you should be aware that no measurement has exact precision and very few (if any) are perfectly constant in time. Thus we must develop some level of confidence in our measurements by quantifying a mean value and level of uncertainty (or range) within which we expect that true value to reside.

Statistically we will quantify the mean of each physical measurement by taking the time-average of a series of measurements acquired at a set frequency for a defined period of time. For this laboratory experiment we will sample all of the electronic sensors at a rate of 500 Hz for 0.04 seconds giving us 20 samples. From this we can calculate the mean measurement for each signal and compute the average airspeed using the previously developed analytical function (see Airspeed Calculation section above).

Estimating the uncertainty in the airspeed is a multistep task. Since the airspeed is a measurement that is derived from other direct measurements we must consider the propagation of the uncertainties from each of these measurements into the calculation of airspeed. For more information on uncertainty you should refer to chapters 1- 4 from the textbook “Introduction to Error Analysis” by Taylor that is used in ASEN 2012. Specifically in Section 3.11 a general formula for computing the propagation of uncertainty in a function of several variables is developed. Specifically it states:

where <em>δq </em>is the total uncertainty for the function of interest and <em>x…z </em>are the independent variables governing <em>q</em>. When we apply this for our case to determine the uncertainty in airspeed we find:

Now to be rigorous, the uncertainties in each of the independent variables (i.e. <em>δ</em>∆<em>p </em>,<em>δp<sub>atm</sub></em>,and <em>δT<sub>atm</sub></em>) should include the errors associated with the random fluctuations (or statistical variation) of the measurement, the errors associated with the measurement hardware, and errors provided by the sensor manufacturer relating to the sensor calibration and performance. For now let’s neglect the errors associated with the random fluctuations and the measurement hardware. Instead focus on only the manufacture quoted error (refer to Appendix A) and assess how the uncertainties in each of the independent variables propagate into the uncertainty in the airspeed calculation. Compute the uncertainty in velocity for both differential pressure measurement devices: (1) the differential pressure transducer and (2) the U-tube manometer.

QUESTIONS TO CONSIDER: <em>Is the uncertainty in airspeed constant with the wind tunnel airspeed? If not how does it change? Does it improve or degrade as we increase the mean tunnel airspeed? Does the U-tube manometer provide a more or worse accurate measure of the velocity? Which independent variable contributes the most to our uncertainty in airspeed? Or asked another way: If you could improve the accuracy of one sensor which one would give you the largest improvement in the airspeed uncertainty?</em>

<h2>5.5     Steps to Take</h2>

<ol>

 <li>Read 5.1-5.4 and referenced appendices to understand the background of this section.</li>

 <li>Take data according to the laboratory procedure outlined in Appendix F.1.</li>

 <li>Calculate airspeed from four different data files using the steps outlined in Appendix B. These four data files should cover the four measurement methods: Pitot-Static Probe to Pressure Transducer, Venturi Tube to Pressure Transducer, Pitot-Static Probe to Water Manometer, and Venturi Tube to Water Manometer. Include data for five different voltage values for a total of 20 airspeed measurements.</li>

 <li>Calculate the uncertainty of the airspeed measurements using the known measurement device uncertainties described in Appendix A and the airspeed uncertainty analysis method described in section 5.4.</li>

 <li>Plot velocity vs. input voltage with error bars for each measurement type. Devise a mathematical model relating the desired speed to the input control voltage based on these graphs.</li>

</ol>

<h1>6         Experimental Section 2: Measurement of Boundary Layer</h1>

<h2>6.1       Wall Boundary Layer Influence</h2>

Boundary layers are regions of retarded flow (or velocity deficit) concentrated around bodies due to the enforcement of the no-slip condition at the body’s surface as a fluid flows past it. Furthermore you should be aware that the thickness of a boundary layer will grow as the flow moves downstream due to the inherent viscosity within the flowing fluid. For additional details on the fundamentals of viscous flow and boundary layers you should refer to Sections 4.15, 4.16, and 4.17 in the text book by Anderson.

It should come as no surprise then that boundary layers will form and grow on each of the test-section walls within the wind tunnel. As these boundary layers grow they will effectively produce a blockage to the main flow in the wind tunnel. This is graphically depicted in Figure 3 below. Since the flow is confined within the walls of the “closed” test-section this boundary layer induced blockage will create a reduction in the effective cross-sectional area of the wind tunnel. From the application of the conservation of mass it should be clear that the velocity in the test-section must accelerate to compensate for this reduction in the effective test-section area. Thus to completely understand how our wind tunnel behaves we must quantify how the flow naturally accelerates through the test-section. This will allow us to determine the limitations on where we can effectively mount models and sensors in the wind tunnel. Additionally it will also provide us an understanding of what the true airspeed is at those locations.

Figure 3: Schematic displaying the influence of the wall boundary layers on the airspeed in the wind tunnel testsection.

As a result, during the wind tunnel calibration we must measure centerline airspeed at multiple locations downstream from the test-section inlet. We will do this using the Pitot Probe mounted on the two axis traverse located on the ceiling of the test-section. Note that a Pitot probe only measures the total or stagnation pressure in contrast with the Pitot-Static probe we used earlier. However to calculate the airspeed we need the differential pressure between the total and a static pressure at the same streamwise position. Thus we will measure the static pressure from a port on the wind tunnel floor and use our fundamental understanding of boundary layer theory to assume that the static pressure will be constant vertically across the boundary layer and thus vertically constant across the test-section.

In order to relate the increase in centerline velocity back to the influence of the viscous boundary layers we must also quantify the thickness of the wall boundary layers at the same locations. Again we will use the same Pitot probe configuration discussed above in conjunction with the traversing system to precisely measure the velocity distribution away from the test-section wall. For these measurements, we will define the edge of the boundary layer at the point where we reach 95% of the free-stream velocity. Mathematically that is:

<em>δ </em>= <em>y</em>@<em>V </em>= 0<em>.</em>95 · <em>V</em><sub>∞                                                                                                                               </sub>(1)

Then using our understanding of the conservation of mass and physical measurements of the test-section size we can attempt to relate the boundary layer growth to the acceleration in the test-section airspeed.

QUESTIONS TO CONSIDER: <em>Does the measured increase in the centerline velocity match the expected flow acceleration due to the measured wall boundary layer thickness at your streamwise measurement location? If not why do you think they differ? When you compare the results at multiple streamwise measurement locations do you see a trend?</em>

<h2>6.2     Steps to Take</h2>

<ol>

 <li>Read section 6.1 to understand the background of this section.</li>

 <li>Take data according to the laboratory procedure outlined in Appendix F.2</li>

 <li>Calculate the airspeed at each y-position for each port location; use the class data files and the steps outlined in Appendix B for the Pitot-Probe setup to do so. Use the Airspeed Differential Pressure value for ∆<em>p </em>when calculating the free-stream velocity, and use the Aux Differential Pressure value for ∆<em>p </em>when calculating velocity values near/in the boundary layer.</li>

 <li>Plot velocity vs. ELD Probe y-location for each port.</li>

 <li>Determine the velocity at the edge of the boundary layer by calculating 95% of the free-stream velocity. Then, using the plot from Step 4 and the boundary layer thickness equation above, determine the thickness of the boundary layer (the y-position corresponding to 95% of the free-stream velocity). Then, plot boundary layer thickness (y) vs. port number.</li>

 <li>Determine if the boundary layer is laminar or turbulent (Hint: See sections 4.16 and 4.17 in Anderson for how to calculate boundary layer thickness specific to laminar and turbulent flow. Calculate these thickness values for each port location and compare them to the lab values you found to see which lines up better).</li>

</ol>

<h1>7          Experimental Section 3: Cambered Airfoil Aerodynamics</h1>

<h2>7.1        Clark Y-14 Cambered Airfoil Background</h2>

The Clark Y Airfoil is a commonly used wing section profile that can be found in many well-known aircraft. Specifically it is regularly used in model aircraft due to its relatively simple flat bottom construction. At a larger scale it can also be found in the Spirit of St. Louis, the plane flown by Charles Lindbergh in his first successful solo flight across the Atlantic Ocean. For our laboratory exercise we will use a modified version of the Clark Y airfoil configuration.

Figure 4: Airfoil schematic with relevant nomenclature.

As you have seen in lecture, all aerodynamic forces are the result of pressure and shear stress distributions around the surface of a body. In this lab we will show that the lift force produced by an airfoil is primarily the result of its pressure distribution. Furthermore we will study how the pressure distribution and thus lift force scales with the airspeed and varies with the angle of attack (incidence) between an airfoil and the free stream velocity. In order to accurately make these comparisons it is common practice to write the pressure and force components in terms of dimensionless coefficients. This allows experimental measurements to be made on a small model in a wind tunnel and scaled up to the full-size configuration. It also allows us to understand the dependence of a measurement on the other experimental variables. For detailed information on the coefficients of pressure, lift, and drag, see Appendix C.

<h2>7.2     Test Configuration</h2>

For this laboratory assignment we will be using a rectangular wing with a Clark Y-14 airfoil that spans nearly the full width of the wind tunnel (approx. 12 in). A picture of the model is presented in Figure 5. Note, that we will mount the model in the wind tunnel in a vertical orientation, however this should not influence the wing aerodynamics. Furthermore, we will neglect any three-dimensional effects at the tip and the root of the wing model. Thus we will assume that the flow is two-dimensional or spanwise uniform (i.e. the velocity and pressure distribution will be the same at each spanwise location). As a result we will collect static pressure measurements at only one spanwise location namely at 50% span, in the center of the wind tunnel. The ports of the airfoil are located at this height. For more information on how the ports are connected to measure the pressure distribution, see Appendix D.

Figure 5: Photograph of the PILOT Clark Y-14 airfoil model with 19 surface pressure ports.

<h2>7.3      Analysis of Pressure Distribution</h2>

Several additional steps are required to post-process and analyze the pressure distributions once the differential pressure measurements have been collected. First, as discussed in Appendix D, you need to estimate the pressure at the theoretical trailing edge point (port #11 in Figure 13). This should be done through extrapolating the pressure at the trailing edge from the upper and lower surfaces data. Then you can average these two extrapolations to provide a single estimate of the differential pressure at the trailing edge.

Second, you should compute and plot the pressure distributions in the form of the normalized pressure coefficient versus the normalized chord-wise position, x/c. Figure 6 presents an example of this distribution. This represents the classical form through which pressure distributions around airfoils are compared and allows researchers to easily scale and compare results for similar shaped airfoils at different conditions. Additionally, this will allow you to understand how the flow conditions alter the pressure distribution. For example, what changes do you observe in the pressure distribution when only different wind tunnel speeds are compared? How do changes in the angle of attack alter the distribution? Do you observe any features in the pressure distribution that would indicate the flow has separated at a point on the surface?

Figure 6: Conceptual graph of the pressure distribution Finally, knowing the distribution of pressure on the upper around an airfoil.

and lower surfaces, we can integrate (sum) all the contributions to determine the net forces perpendicular and parallel to the airflow, i.e., the lift and pressure drag. By repeating this exercise for each of angle of attack, we can then construct plots to see how the lift and pressure drag vary with the angle of attack, <em>α</em>. Furthermore, we could compare these plots at different airspeeds to understand the influence that the airspeed has on the separation and stalling characteristics of an airfoil. The following section lays out the computational procedure for integrating the pressure distributions.

QUESTIONS TO CONSIDER: <em>When properly normalized, how does the pressure distribution vary with the airspeed? How do changes in angle of attack alter the pressure distribution? Do you observe any features in the pressure distribution that would indicate the flow has separated at a point on the surface? Finally, where along the airfoil chord is the largest difference in the surface pressure between the upper and lower surfaces? What does this tell you about the pitching moment you can expect on a Clark Y-14 airfoil?</em>

<h2>7.4      Computation of Lift and Drag</h2>

As discussed previously, we must integrate the pressure distribution in order to calculate the lift and pressure drag. Since we sample the pressure at a discrete number of points, we must resort to a numerical integration of the pressure distribution. The airfoil section along with the coordinate systems to be used to carry out this procedure are shown in Figure 7 below. Lift and drag (L and D) are defined relative to the oncoming flow direction. The normal and axial forces (N and A) are referenced with respect to the airfoil. It is easiest to perform the force integrations in the airfoil coordinate system (thereby determining N and A) and then transfer these forces to the free-stream coordinate system (giving the desired L and D).

Figure 7: Airfoil orientation and reference systems. The following coefficient definitions are found by performing the aforementioned integration

See Appendix E for a detailed derivation of these expressions.

If the angle of attack is small we see that the lift is dominated by the normal force and the drag is dominated by the axial force. This procedure and these equations are similar to that presented by Anderson in section 5.7 of our textbook. Furthermore, with a little more analysis we can show that the sectional lift coefficient is fundamentally equal to the difference between the integrated pressure coefficient over the lower surface and the upper surface of an airfoil.

Now that we have defined the procedure for computing the coefficients of lift and pressure drag, we should repeat this computation for each angle of attack and freestream airspeed. We can then construct plots that compare the trends in the lift and pressure drag versus with the angle of attack, <em>α</em>. Furthermore, we could directly compare these same plots at different airspeeds to understand the influence that the airspeed has on the separation and stalling characteristics of an airfoil. Each of these tasks should be accomplished and included in your final report.

QUESTIONS TO CONSIDER: <em>How do each the lift and pressure drag vary with angle of attack? What is the maximum lift coefficient that this airfoil can generate, and at what angle of attack does that occur? What is the lift produced at zero angle of attack; is it zero? If not why and where is the lift equal to zero? What is the minimum pressure drag and where does that occur? How do these plots and values change at different airspeeds? Do your results match those produced by NACA in 1938 (i.e. Figure 11)? If not, what are the sources for error in your measurements?</em>

<h2>7.5     Steps to Take</h2>

<ol>

 <li>Read section 7.1-7.4 and referenced appendices to understand the background of this section.</li>

 <li>Take data according to the laboratory procedure outlined in Appendix F.3.</li>

 <li>Calculate the pressure value at the trailing edge (port #11) for each angle of attack as outlined in Appendix D.</li>

 <li>Calculate the coefficient of pressure at each Scanivalve port using the measured data and the method outlined in Appendix C.</li>

 <li>Plot the coefficient of pressure vs. normalized chord length for various airspeeds and angles of attack. Be sure to ”flip” your data to produce graphs that look similar to Figure 6.</li>

 <li>Calculate the normal force coefficient and the axial force coefficient. Then, using these values, calculate the coefficient of lift and the coefficient of drag for the airfoil. Details for these four calculations can be found in Appendix E.</li>

 <li>Plot the coefficient of lift vs. angle of attack and the coefficient of drag vs. angle of attack.</li>

</ol>

<h1>ANALYSIS OF LABORATORY DATA</h1>

You can and should begin the analysis tasks for this lab even before you have collected your own data sets at the wind tunnel. Several of these items can be accomplished before your assigned testing period as they do not require experimental data. For example, the quantification of the uncertainty in the velocity measurements and the prediction of the boundary layer’s influence on the streamwise speed are both tasks that do not require experimental data. Data collected by the professor, TAs, and Laboratory Staff has been posted on the website for you to use to help develop your code and in the event your group is unable to test on the physical wind tunnel. You can begin working on your MATLAB scripts that will load and process the data files. The computational procedure for computing the lift from the pressure distribution is very involved and should be started early. You should work on these tasks together with your group during your lab session. Use the background material, <em>Questions to Consider </em>in this document, and the grading rubric as a guide for your analysis.

It is recommended that you use MATLAB to analyze and plot all of the experimental data. You can use the sample data files posted on the course website and your classmate’s submitted data files to begin the process of building your data loading and post-processing scripts, even before you acquire your own data. Note that the data files collected with the wind tunnel are all stored in the same format as a .csv file where each column contains a different measurement and the rows are the individual data points collected (refer to the data measurement section above for more detail). To develop a complete understanding of how the wind tunnel performs, as well as how the lift and pressure drag vary with angle of attack and airspeed, you should also compare your measurements with those of your classmates. Your data is not complete on its own; you will need your classmate’s data to complement your own in your analysis. Specifically when comparing the different measurement configurations: (1) pitot-static probe vs. (2) static ring; you will only have taken measurements with the airspeed transducer for one of these configurations and measurements with the U-tube manometer for the other. As such you will need another group’s data that complements yours (i.e. the opposite measurement configuration) to make an accurate comparison! Further, due to the time constraints, you are only collecting pressure measurements at four angles of attack. When you combine your results with your classmates’ data you can reconstruct the lift and pressure drag distributions versus angle of attack from -15° to 15° for 1° increments. You should begin analyzing and processing these results early as the data files are available.

<h1>Appendices</h1>

<h2>A      Wind Tunnel Measurement Devices</h2>

Temperature Measurements

The concept of temperature was covered in great detail during the Thermodynamics section of this course. As a result, it is assumed that you have developed a fundamental understanding of how temperature measurements can be made. For the wind tunnel facility, ambient or atmospheric temperature, <em>T<sub>atm</sub></em>, measurements are made with an LM35 Precision Centigrade Temperature Sensor from National Semiconductor. Note that the manufacturer states that this device has a range -55°C to +150°C and a typical accuracy of° C at room temperature.

Pressure Measurements

As with temperature, pressures are always physically measured as a relative quantity. That said when discussing pressure measuring devices there are three common terms often used: (1) absolute, (2) gauge, and (3) differential. Each of these implies a different relative measurement. Specifically, an absolute pressure measurement device quantifies the pressure magnitude at a certain point of interest relative to a perfect vacuum. A gauge pressure measurement device quantifies the pressure of interest relative to the ambient or atmospheric pressure. Finally, a differential pressure measurement device quantifies the relative difference in pressure between two specific locations of choice. In the current laboratory assignment, three different pressure measurement devices will be used with the wind tunnel. These include a U-tube manometer, a differential pressure transducer, and an absolute pressure transducer, each of which is discussed below.

<h3><u>U-tube manometers</u></h3>

U-tube manometers represent the simplest and most traditional means of quantifying a differential pressure. They quantify the change in pressure through displacements in the static head of a known fluid (typically either water, oil or mercury). For more information on the operation of manometers refer to section 2-8 in the Thermo-Fluids text by Cengel et al. and section 4.10 in the Aero text by Anderson. The Dwyer Flex-Tube U-Tube manometer attached to the PILOT Low-Speed Wind Tunnel is filled with a red fluid which has a specific gravity of 0.826. The manometer ruler is calibrated to read inches of water and has a maximum range of ±6 in with 0.1 inch gradations.

<h3><u>Pressure Transducers</u></h3>

A pressure transducer is a device that converts the physical property of pressure into an electrically measurable signal. Be aware there are many different types of transducers available on the open market which can rely on drastically different means of measuring pressure. The type used with the wind tunnel, and one of the most common types, is a piezoresistive transducer. These are electro-mechanical transducers in that a pressure difference is applied across a thin diaphragm causing it to mechanically strain (or deform) under the applied force (see Figure 8). This strain results in a change in the electrical resistance of the diaphragm material (typically a piezo ceramic material) which through additional circuits (not discussed or displayed here) is measured as a change in voltage. To measure an absolute pressure the reference side of the transducer, P2, is sealed and held at a fixed

pressure. In contrast, P2 in a gauge pressure measure- Figure 8: Schematic showing the fundamental configurament would be left open to the ambient environment to tion of a piezo resistive pressure transducer allow for the relative pressure between P1 and the atmospheric pressure in the vicinity of the transducer.

For the current assignment we will be using three pressure transducers with the PILOT wind tunnel. The dynamic pressure in the wind tunnel can be measured with one of two separate Honeywell SCX01DN differential pressure sensors. The manufacture states that these devices have a full-scale operating range of 0 psid to 1 psid and that it has a calibrated accuracy of ±1% of the full scale span. The third transducer is used to measure the ambient or atmospheric pressure within the PILOT laboratory space. It is a Freescale Semiconductor MPX4250A Absolute Pressure Sensor, which has a full measuring range of 20 kPa to 250 kPa and an accuracy or ±1.5% of the full scale span, as quoted from the manufacturer.

Airspeed Measurements

Clearly, an accurate measure of the wind tunnel airspeed is required for all three experiments. This is made with the pitot-static probe mounted at the test section entrance or a venturi tube mounted before the test section, and the airspeed differential pressure transducer or manometer. Furthermore, the air density is computed using the ideal gas law and measurements of the ambient (atmospheric) pressure and temperature. The details about these measurement devices and methods are fully documented and discussed in Appendix B and are not repeated here for brevity. Please refer to this section to address any questions about the airspeed measurement system. In Experimental Sections 1 and 2, both the Pitot-Static Probe and Venturi Tube Configurations will be used to calculate airspeed; Experimental Section 3 will exclusively use the Pitot-Static Probe Configuration.

Pressure Distribution Measurements

Of primary interest in Experimental Section 3 of this laboratory assignment is the measurement of the surface pressure distribution on the Clark Y-14 airfoil. These measurements are made on the surface of the wing model at each of the port locations discussed previously. From the wing model each of these ports is plumbed, using flexible tubing, to an associated port on a Scanivalve DSA3217 Multi-Port Pressure Scanner; refer to Figure 13 for details about the port configuration. Specifically, the Scanivalve Pressure Scanner incorporates 16 individual pressure transducers that can be sampled nearly simultaneous. Each of these 16 channels has a full scale range of 10 in. of water and a manufacturer quoted long term accuracy of 0.20% of full scale. Note: this device does not measure absolute pressure, instead it measures the differential pressure between each of the designated channels and a reference channel. <em>This reference channel should be connected to the test section static pressure ring to provide each of the surface pressure measurements relative to the test section static pressure. </em>When connected properly this will simplify the calculation of the pressure coefficient discussed previously. If this is not connected then the Scanivalve will output each of the measurements relative to the room ambient (atmospheric) pressure.

<h2>B      Detailed Airspeed Calculation</h2>

As mentioned previously, there is no way to measure airspeed directly, so we must take a few steps to calculate it. Specifically, for the PILOT Low-Speed Wind Tunnel we can utilize Bernoulli’s Equation for incompressible flow to relate the pressure at various locations to the square of the velocity (or airspeed).

This equation relates pressure and velocity; however it also requires knowledge of the fluid density. Unfortunately the fluid density is another quantity that is also not directly measured. Instead we rely upon our understanding of the thermodynamics and employ the equation of state for a perfect gas to relate the density to the direct measurements of temperature and pressure.

For incompressible flow we assume that the density is constant at each location within the wind tunnel. Thus to compute density we need to know both pressure and temperature at only one location in the system. Typically we will use the atmospheric pressure and temperature measurements outside of the wind tunnel under similar stagnant flow conditions to accomplish this.

Through combining Bernoulli’s Equation and the Equation of State for a Perfect Gas we can now develop a single equation that relates wind tunnel airspeed directly to the quantities that we directly measure in the wind tunnel system. The next step is to consider where the direct measurements are acquired in the wind tunnel system and what assumptions we can make about the velocity at those locations. For the PILOT Low-Speed Wind Tunnel there are two standard air-speed measurement configurations that we can use, each of which is detailed in Figure 8 below.




First we can measure the differential pressure, ∆p, across a Pitot-Static probe mounted in the wind tunnel (Figure 10a) as discussed by Anderson in section 4.11. This method allows for a direct measure of the difference between the static pressure, <em>p<sub>s</sub></em>, and total pressure, <em>p</em><sub>0</sub>, at effectively the same location in the flow field. Furthermore, this differential pressure is then equivalent to the dynamic pressure, <em>q</em>; assuming that we have minimal losses between the total and static measurement locations. As a result from Bernoulli’s Equation:

but,

<em>V</em><sub>0 </sub>→ 0

and

<em>V</em><em>s </em>= <em>V</em>∞

so

This can be rearranged to provide:

One negative effect of using a Pitot-Static Probe to measure the wind tunnel speed is that this requires the insertion of the probe into flow upstream of where you may want to test a model. As a result the blockage and wake of your probe can influence your model and potentially bias other results. The second configuration eliminates the need for a probe through comparing the average static pressure at two different locations in the wind tunnel. Typically this comparison is made between the test-section and the settling chamber as discussed by Anderson in section 4.10 and presented in Figure 10b. Again in this case we can use Bernoulli’s equation:

Figure 9: Cross-sectional view of a Pitot-Static Probe configuration. In this case the static pressure is denoted as <em>p</em><sub>∞ </sub>and the total is denoted as <em>p</em><sub>0</sub>.

Figure 10: Schematic displaying the two standard airspeed measurement configurations for the PILOT LowSpeed Wind Tunnel. Note the static pressure is denoted as <em>p<sub>s</sub></em>.




and,

where

<em>V</em><em>s,</em>2 = <em>V</em>∞

However in this case the velocity in the settling chamber, <em>V<sub>s,</sub></em><sub>1</sub>, does not go to zero; as with the Pitot-Static Probe. So to reduce the number of unknowns we need to find a way to relate the velocity in the settling chamber to the velocity in the test-section. To do this we apply our understanding of the conservation of mass and our assumption that the flow is incompressible. Thus we arrive at:

<em>A</em>1<em>V</em><em>s,</em>1 = <em>A</em>2<em>V</em><em>s,</em>2

so

where <em>A</em><sub>1 </sub>and <em>A</em><sub>2 </sub>are the cross-sectional areas of the settling chamber and the test-section of the wind tunnel. We can now relate the pressure difference to the test-section velocity:

<em>.</em>

Now as before, this can then be reorganized to provide the test-section velocity:

This is known as the Venturi Tube equation. Where a Venturi Tube, is a general measurement probe/device that computes the velocity through relating the pressures and cross-sectional areas at two different stations within a channel or pipe. Fundamentally, in this case we are treating the wind tunnel as a large Venturi Tube.

<h2>C       Coefficients of Pressure, Lift, and Drag</h2>

It is first important to define a dimensionless quantity known as the coefficient of pressure:

(2)

where the subscript ∞ denotes the free-stream value far upstream of an object in the undisturbed flow and <em>q</em><sub>∞ </sub>is the dynamic pressure. This coefficient of pressure (or pressure coefficient) contains information for how pressure varies on the surface of an immersed object. Furthermore, using Bernoulli’s equation, we can directly relate the local speed at different points on the surface of the object to the coefficient of pressure.

(3)

In a similar manner we can define a coefficient of force, and will do this for both Lift and Drag Forces,

(4)

(5)

where L and D represent the lift and drag forces respectively, and S is a reference surface area. For a rectangular wing section we will simply define the reference area as the chord length, c, multiplied by the wing span, b,

<em>S </em>= <em>c </em>· <em>b                                                                                             </em>(6)

The coefficients of lift and drag for an airfoil are commonly reported values in literature that define the performance of an airfoil. The coefficients of a Clark Y-14 airfoil were experimentally measured and reported in a NACA Technical Report, specifically number 628 from 1938. Figure 11 is taken from page 42 of this report and displays the variation in all of these coefficients versus angle of attack at a Reynolds Number of <em>Re </em>= 3 · 10<sup>2</sup>.

Figure 11: Aerodynamic coefficients for a Clark Y-14 airfoil from NACA Technical Report 628 (pg. 42).

We have just defined the coefficients of lift and drag (<em>C<sub>L </sub></em>and <em>C<sub>D</sub></em>) for a finite span wing where the wing area is defined as S. When we are working with airfoils (i.e. an infinite span wing), as we are in this laboratory assignment, we will typically define a sectional coefficient of lift and drag

(7)

(8)

where <em>l </em>and <em>d </em>are the lift and drag forces per unit span of the wing surface. Note that these two coefficients will be equal for a rectangular wing that has a uniform distribution of lift and drag with respect to its span; as we are assuming in this activity. That said we will focus and discuss only the sectional coefficients of lift and drag as we discuss the aerodynamic performance of airfoils in this laboratory assignment.

<h2>D      Detailed Test Configuration</h2>

To measure the static pressure distribution on the wing surface, the Clark Y-14 wing model is instrumented with 19 static pressure ports uniformly distributed around the surface. These static pressure taps can be visually observed on the model in Figure 5 and their position is defined in the graph found in Figure 12 and by the table in Figure 13. We will not measure the absolute static pressure at each of these locations; instead we will measure the differential pressure referenced between each port and the freestream static pressure of the wind tunnel (i.e. the difference in pressure between the port and the tunnel freestream). This measurement will simplify our calculation of the pressure coefficient discussed previously.

Figure 12: Schematic outlining the position of the surface pressure ports on the Clark Y-14 airfoil model.

Figure 13: Measurement port configuration.

As mentioned above, the wing has 19 pressure ports, but our pressure scanner can only measure 16 channels at one time. Thus we cannot measure all of the airfoil pressure ports at one time. As a result for this lab we will only consider a subset of the ports available on the Clark Y-14 wing surface and will not connect ports 9, 13, and 15 as documented in Figure 13 above. Finally, to complete the pressure distribution around the airfoil we need a pressure value at the trailing edge (port #11) of the wing surface, however it would be nearly impossible to instrument a pressure port on the sharp trailing edge of the airfoil. Thus we will need to come up with a theoretical estimate of the differential pressure at the trailing edge. To do this we can extrapolate the pressure at the trailing edge (x = 3.5in) based upon pressure measured at the last two ports on both the upper and lower wing surfaces (upper: port 10, port 8 and lower: port 12, port 14. These linear extrapolations will give us two different estimates for the pressure at the trailing edge, but we know that the pressures from the upper and lower surfaces must converge at the trailing edge. Thus we should average these two pressure estimates to provide one estimate at the trailing edge. We can then incorporate this value into the pressure distribution to complete (and close) the distribution around the Clark Y-14 airfoil. Note: this pressure will change with angle of attack and velocity, thus this procedure will have to be repeated for each of the test cases.

<h2>E        Detailed Calculation of Lift and Drag</h2>

To perform the numerical integration introduced in the main body of this document, let the pressure tap locations be denoted as (<em>x<sub>i</sub>,y<sub>i</sub></em>) and the corresponding pressure be <em>p<sub>i </sub></em>where <em>i </em>= 1,2,…,<em>n</em>. In order to perform the force integrations we will break the airfoil surface into linear elements, each of which span two consecutive pressure taps. Such an element, spanning taps <em>i </em>and <em>i </em>+ 1, is shown in Figure 14. We shall assume that the pressure is constant over each element and equal to the average of the pressures at the two end points (where the taps are located).

Figure 14: Schematic displaying the elemental components related to the integration of surface pressure between two pressure ports.

According to the sketch, the normal force over the <em>i<sup>th </sup></em>segment is

(9) The sketch shows that <em>cosθ </em>= ∆<em>x<sub>i</sub>/</em>∆<em>s<sub>i</sub></em>, so that Eq. 8 can be simplified to give

(10)

A similar development shows that the axial force is given by

(11)

and similar to the normal force

(12)

Summing over all elements gives the total forces

(13)

and

(14)

Note that ∆<em>x<sub>i </sub></em>= <em>x<sub>i</sub></em><sub>+1 </sub>− <em>x<sub>i </sub></em>and ∆<em>y<sub>i </sub></em>= <em>y<sub>i</sub></em><sub>+1 </sub>− <em>y<sub>i</sub></em>.

As we discussed above, it is convenient to rewrite the force expressions in a non-dimensional form. We accomplish this by adding and subtracting the free-stream pressure (<em>p</em><sub>∞</sub>) from the right hand side and then dividing both sides by the quantity , where <em>c </em>is the airfoil chord. The result for the normal force is

(15)

The definition of the pressure coefficient is evident above and the last term vanishes since the summation is taken over a closed contour (the airfoil surface). Making these simplifications, and performing the analogous operations on the expression for the axial force gives

(16)

and

(17)

Notice that these expressions are nothing more than trapezoidal rule approximations to the following two contour integrals, which give the exact normal and axial force coefficients

(18)

(19)

In order to get the lift and drag, it is necessary to transfer the normal and axial force coefficients to the freestream coordinate system. With reference to Figure 7 it can be shown that

<table width="380">

 <tbody>

  <tr>

   <td width="358"><em>C<sub>l </sub></em>= <em>C<sub>n</sub>cosα </em>− <em>C<sub>a</sub>sinα</em></td>

   <td width="22">(20)</td>

  </tr>

  <tr>

   <td width="358"><em>C<sub>d </sub></em>= <em>C<sub>n</sub>sinα </em>+ <em>C<sub>a</sub>cosα</em></td>

   <td width="22">(21)</td>

  </tr>

 </tbody>

</table>

<h2>F      Laboratory Procedures</h2>

Take good notes of experimental setup, record data, and consider possible errors in the measurements. You are encouraged to take pictures of the tunnel and your experimental setup with your own devices to help you document your work. See the three Experimental Procedure Captivates on Canvas for more details.

<h2>F.1      Experimental Section 1: (Measurement of Airspeed)</h2>

COVID-19 UPDATE: A virtual wind tunnel analog has been developed in MATLAB. See the Canvas page to download it and run on your machine. You may use either the virtual wind tunnel or the posted data for you analysis. In the event campus is allowed to reopen you may use your group’s collected data. The following instructions have been left in this document so you may the operation that was used to collect the posted data. Prelab Tasks:

<ol>

 <li>Read the lab assignment in detail and ask questions prior to your assigned measurement period.</li>

 <li>Review the group assignments spreadsheet to determine the measurement configuration your team has been assigned and the voltages you are required to test at.</li>

 <li>Review the group assignments spread sheet to determine the filename you are required to use for your data. This is important since data will be shared with the entire class.</li>

 <li>Meet with your group and assign tasks and roles for each student to perform during the wind tunnel measurement period. Develop a plan to ensure you perform your tasks most efficiently.</li>

</ol>

Procedure:

<ol>

 <li>Visually inspect the tunnel and compare the facility to the theoretical expectations.</li>

 <li>Locate the pressure tubes for the pitot-static tube, the static pressure ring, the Airspeed Pressure Transducer, and the U-tube Manometer.</li>

 <li>Connect the pressure tube disconnects according to the configuration that was assigned to your team. Ensure that you connect the tubes to the Airspeed Pressure Transducer in the proper orientation.</li>

 <li>Ensure there are no objects left in the wind tunnel. Close and lock the wind tunnel door.</li>

 <li>Start the LabVIEW control program named WT2016 voltage control 2018 – Shortcut.vi which is located in the ASEN2002 courses folder H:AESSoftwareVIs DO NOT open: WT2018 – Shortcut.vi this will be used for Aero Lab 2.</li>

 <li>Set your data file path according to the naming convention assigned in the group assignment spreadsheet. <em>Note: Be careful not to overwrite another group’s data file!!!</em></li>

 <li>Once the LabVIEW VI that controls the wind tunnel and logs the measurements is open and running, zero the airspeed and pressure transducers using the green button on the VI front panel in the bottom left.</li>

 <li>Type the first voltage that was assigned to your team into the LabVIEW VI and bring the wind tunnel up to speed.</li>

 <li>Once the wind tunnel has reached equilibrium (typically between 30 and 60 sec), acquire measurements with the pressure transducer by clicking the <em>Send Samples to File Button </em>in the upper left corner of the VI.</li>

 <li>Visually measure the displacement of the U-tube manometer <em>Note: Be sure to measure the manometer from the bottom of the meniscus in each of the fluid columns!</em></li>

 <li>Document the differential pressure from the U-tube manometer in your lab notebook and in the provided Google Form: <a href="https://forms.gle/GKVGqtrWNVJk2itw6">Click Here</a></li>

 <li>Repeat the pressure measurements for each voltage assigned to your team. Note: You should be measuring five voltages in total.</li>

 <li>Slowly bring the tunnel back to zero. Allow time for the tunnel to completely stop, then Stop the VI to save and close your current data file.</li>

 <li>Immediately load data to the class folder: <a href="https://drive.google.com/drive/folders/1O-LdeTrj7Sglfhnp2tZe9zt259GLEy_c?usp=sharing">Click Here</a></li>

</ol>

F.2       Experimental Section 2: (Measurement of Boundary Layer Influence)

COVID-19 UPDATE: You may use the posted data for you analysis. In the event campus is allowed to reopen you may use your group’s collected data. The following instructions have been left in this document so you may the operation that was used to collect the posted data. Prelab Tasks:

<ol>

 <li>Read the lab assignment in detail and ask questions prior to your assigned measurement period.</li>

 <li>Review the group assignments spreadsheet to determine the streamwise location where your team has been assigned to make the boundary layer measurements. This is related to the port number that you were assigned. Refer to the supplemental drawings to determine the physical location of the measurement referenced from the entrance to the test-section.</li>

 <li>Review the group assignments spread sheet to determine the filename you are required to use for your data. This is important since data will be shared with the entire class.</li>

 <li>Meet with your group and assign tasks and roles for each student to perform during the wind tunnel measurement period. Develop a plan to ensure you perform your tasks most efficiently.</li>

</ol>

Procedure:

<ol>

 <li>Identify the static pressure port on the test-section floor and the corresponding streamwise position where your team was assigned to conduct your measurements.</li>

 <li>Connect the pressure quick disconnects of the ELD Boundary Layer Probe and your identified static port to the total and static disconnects of the “Auxiliary” pressure transducer. The ELD Probe should be connected to the “Aux Meas” tube and your team’s static port should be connected to the “Aux Ref” tube. Ensure that the pitotstatic probe is connected to the Airspeed Pressure Transducer in the proper orientation <em>Note: the pitot-static probe may or may not be connected already depending upon the orientation your group tested in Part 1.</em></li>

 <li>Align the leading edge of the ELD Boundary Layer probe just downstream of the identified port by moving the horizontal traverse by hand with the knurled adjustment knob.</li>

 <li>Vertically traverse the probe by hand with the vertical control knob until the tip is just barely touching the wind tunnel floor. Be VERY careful NOT to bend or damage the ELD Boundary Layer probe by driving it into the floor!</li>

 <li>Ensure there are no objects left in the wind tunnel. Close and lock the wind tunnel door.</li>

 <li>Start the LabVIEW control program named WT2016 voltage control 2018 – Shortcut.vi which is located in the ASEN2002 courses folder H:AESSoftwareVIs DO NOT open: WT2018 – Shortcut.vi this will be used for Aero Lab 2.</li>

 <li>Set your data file path to the desktop and enter the file name according to the naming convention assigned in the group assignment spreadsheet. <em>Note: Be careful not to overwrite another group’s data file!!!</em></li>

 <li>Once the LabVIEW VI that controls wind tunnel and logs the measurements is open and running, zero the airspeed and pressure transducers using the green button on the VI front panel.</li>

 <li>Zero the readout of the ELD Probe Location on the front panel of the LabVIEW control program. <em>Note that the ELD Boundary Layer Probe has a diameter of 0.8 mm, thus your actual measurement height is offset 0.4 mm above the floor and will not actually be at zero mm.</em></li>

 <li>Set the wind tunnel speed control to 5 Volts using the desired voltage knob on the LabVIEW VI front panel (mid-range in the voltage control) and bring the wind tunnel up to speed.</li>

 <li>Once the tunnel has reached a steady-state begin your measurement survey. Acquire measurements at locations according to your group’s assignment. These will be every 1 mm, starting at either 0 mm or 0.5 mm. There should be a total of 11 points measured.</li>

 <li>Take an additional measurement with the probe centered vertically in the wind tunnel test-section: (152.4 mm or 6 in).</li>

 <li>Verify that 12 measurements have now been sent to the data file (11 from before and one from the centered measurement).</li>

 <li>Bring the wind tunnel velocity back down down to zero by slowly lowering the voltage.</li>

 <li>After the wind tunnel has stopped, stop the VI to save and close your current data file!</li>

 <li>Immediately load data to the class folder: <a href="https://drive.google.com/drive/folders/1O-LdeTrj7Sglfhnp2tZe9zt259GLEy_c?usp=sharing">Click Here</a></li>

</ol>

F.3        Experimental Section 3: (Cambered Airfoil Aerodynamics)

COVID-19 UPDATE: You may use the posted data for you analysis. In the event campus is allowed to reopen you may use your group’s collected data. The following instructions have been left in this document so you may the operation that was used to collect the posted data.

Note that all of the measurements are acquired with the wind tunnel control program, written in the LabVIEW software language, at a rate of 500Hz for a period of 0.04 sec providing a set of 20 measurements at every collection point. These data points are then saved in a collimated data file in a comma separated (.csv) ASCII format. Please refer to the sample data posted on the course website if you have any questions and to help construct your analysis code. Note that this data file will store values for all the possible measurements that the wind tunnel data acquisition system can collect, however you may not be using some of these sensors and should thus ignore additional data.

Prelab Tasks:

<ol>

 <li>Read the lab assignment in detail and ask questions prior to your assigned measurement period.</li>

 <li>Review the group assignments spreadsheet to determine the measurement configuration your team has been assigned and the voltages you are required to test.</li>

 <li>Review the group assignments spread sheet to determine the filename you are required to use for your data. This is important since data will be shared with the entire class.</li>

 <li>Meet with your group and assign tasks and roles for each student to perform during the wind tunnel measurement period. Develop a plan to ensure you perform your tasks most efficiently.</li>

</ol>

Procedure:

<ol>

 <li>Visually inspect the tunnel and compare the facility to the theoretical expectations.</li>

 <li>Locate the pressure tubes for the pitot-static tube and ensure they are correctly connected to the Airspeed Pressure Transducer such that the wind tunnel control computer can monitor the wind tunnel speed.</li>

 <li>Locate all of the pressure tubes coming from the airfoil model and ensure that they are correctly connected to the Scanivalve Pressure Scanner such that you are confident in the measurement configuration of the wing model.</li>

 <li>Find the angle markings on the airfoil base plate, and align the airfoil angle of attack to the first position you were assigned. <em>Note: Make sure you have thoroughly tightened the retaining screws to ensure the airfoil is secure and will not move under wind load when the wind tunnel is operating.</em></li>

 <li>Close and lock the wind tunnel door.</li>

 <li>Open then Start the LabVIEW control program program by clicking the white arrow in the top left corner of the window named WT2018 – Shortcut.vi which is located in the AES Courses Folder (Courses/AES/Software/VIs/ASEN2002). DO NOT USE WT2016 voltage control – Shortcut.vi as this .vi does not contain the correct interfaces for this experiment.</li>

 <li>Set your data file path according to the naming convention assigned in the group assignment spreadsheet. <em>Note:</em></li>

</ol>

<em>Be careful not to overwrite another group’s data file!!!</em>

<ol start="8">

 <li>Once the LabVIEW VI that controls the wind tunnel and logs the measurements is open and running, zero the airspeed and pressure transducers using the green button on the VI front panel in the bottom left. .</li>

 <li>Type the first velocity that was assigned to your team into the LabVIEW .vi and bring the wind tunnel up to speed.</li>

 <li>Confirm with LA that the measurement parameters are correct: Sampling Rate of 500 Hz, Samples per Set of 20.</li>

 <li>Once the wind tunnel has reached equilibrium (typically between 30 and 60 sec), acquire measurements with the pressure transducer by clicking the <em>Send Samples to File Button </em>in the upper left corner of the VI.</li>

 <li>Type in the current angle of attack when prompted by the program.</li>

 <li>Once the data has been collected increase the tunnel speed to your next airspeed setting.</li>

 <li>Repeat your measurements for each of the velocities at one angle of attack.</li>

 <li>To change the angle of attack, bring the wind tunnel airspeed back to zero. DO NOT STOP THE .vi. Stopping the .vi will necessitate the creation of another data file.</li>

 <li>Once the tunnel has settled out, open the window, rotate and align the wing model to your next angle of attack, secure the model and close the wind tunnel door.</li>

 <li>Repeat the pressure measurements again for each velocity assigned to your team and at each angle of attack. <em>Note: Be sure to progress through the angles of attack in the assigned order. Also be sure to return the wind tunnel to zero airspeed when you change the angle of attack. Do not stop the .vi until the entire survey is complete.</em></li>

 <li>Once your data survey is complete, bring the tunnel back to zero, allow time for the tunnel to completely stop, then Stop the VI to save and close your current data file.</li>

 <li>Immediately load data to the class folder: <a href="https://drive.google.com/open?id=10x2TV-uvrxrdZjfkhOKQSyOET_bexHRA">Click Here</a></li>

</ol>