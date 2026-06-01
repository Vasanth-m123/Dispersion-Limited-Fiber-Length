# Dispersion-Limited-Fiber-Length
Dispersion Limited Fiber Length
# Objective: 
 
Calculate the dispersion-limited fiber length for a fiber optic transport system that 
employs standard single-mode fiber and a directly-modulated single-mode laser diode 
transmitter. 
 
Simulate the resulting system and verify that it meets performance objective.  
 
# Theory: 
 
The maximum allowable dispersion (or pulse spread) <img width="76" height="52" alt="image" src="https://github.com/user-attachments/assets/52dff457-e7aa-4312-aef4-aa4e234afb47" /> is given in terms of the transmission rate R by the following engineering guideline <img width="192" height="124" alt="image" src="https://github.com/user-attachments/assets/4fcb3de9-6a4a-48db-ba5f-f020a6c85d8b" /> This guideline provides reasonable assurance that there will be no significant inter
symbol interference (ISI) due to pulse spread. 
 
For standard single-mode fiber driven by a directly-modulated laser diode transmitter, the 
pulse spread due to chromatic dispersion is given by
<img width="898" height="694" alt="image" src="https://github.com/user-attachments/assets/5499f4b0-2405-4a5f-b773-ce004a76e850" />
<img width="1300" height="974" alt="image" src="https://github.com/user-attachments/assets/bbd90891-43d6-4a5d-92d2-73ed3e4e57eb" />
# Layout: 
Open up the OptiPerformer file called “Dispersion Limited Fiber.osp”. This layout uses 
the Laser Rate Equations laser diode component with default parameters.  It models a 
directly modulated laser diode based using a standard rate equation model. One of the 
effects of this model is that it generates a signal with a spectral width of about 0.6 nm for 
the default parameters with 2.5 Gb/s, return to zero modulation. 
Within the layout, there are several “Visualizers.” The “Optical Time Domain 
Visualizers” allow the user to the view the simulated signal as a function of time. There is 
one at the output of the laser and one at the end of the fiber.  This allows the user to 
directly observe the changes in the pulses due fiber dispersion. The “Optical Spectrum 
Analyzer” allows the user to view the spectral content of the signal. It this lab it is used to 
verify that the spectral width is about 6 nm. The “BER analyzer” provides calculations of 
the Q factor, the bit error rate (BER) and provides a plot of the eye diagram. 
# Simulation:  
Set the laser power such to achieve a transmitter output power of 0 dBm. The transmitter 
power can be viewed by double clicking the “Output Power Meter Visualizer.” The 
power will read -100 dBm until the first run is made.  
Using the chromatic dispersion factor equation, determine the dispersion of the fiber at 
1550 nm and set the fiber dispersion parameter accordingly. 
Using the equations above, determine the dispersion-limited fiber length. 
<img width="1262" height="1044" alt="image" src="https://github.com/user-attachments/assets/e0b20ca6-42b4-4f1b-ac9a-e4f931a85001" />
# Tabulation
<img width="1920" height="1080" alt="Screenshot (145)" src="https://github.com/user-attachments/assets/e75ab842-5f97-45a2-b824-06267b9c3622" />
<img width="1920" height="1080" alt="Screenshot (146)" src="https://github.com/user-attachments/assets/b18876e7-2742-4139-86c7-0c9c21c67d5e" />
<img width="1920" height="1080" alt="Screenshot (147)" src="https://github.com/user-attachments/assets/ebae7684-de12-45d5-be0c-3babbe74c2fa" />
<img width="1920" height="1080" alt="Screenshot (148)" src="https://github.com/user-attachments/assets/9e379bd1-b40e-4961-9ef8-ff9c73228cd7" />
<img width="1920" height="1080" alt="Screenshot (149)" src="https://github.com/user-attachments/assets/fa04ce83-e350-44b1-92f0-fe5226232b42" />
<img width="668" height="1280" alt="image" src="https://github.com/user-attachments/assets/f4ba66d7-7297-49c8-b4e5-37a9cf209c18" />
<img width="1280" height="1186" alt="image" src="https://github.com/user-attachments/assets/d687620a-e88c-441e-8f04-c8d4093fc063" />

# Result
The dispersion-limited fiber length for the given optical communication system was found to be approximately 10 km. The simulation results showed acceptable BER performance with a clear eye diagram and minimal intersymbol interference. Hence, the system operated successfully within the dispersion limit.
