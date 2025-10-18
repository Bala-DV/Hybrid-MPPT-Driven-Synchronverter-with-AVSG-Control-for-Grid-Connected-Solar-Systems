# Hybrid-MPPT-Driven-Synchronverter-with-AVSG-Control-for-Grid-Connected-Solar-Systems
A grid-connected solar PV system using hybrid MPPT (VPA, CPA, ACP), boosting 2953 V to 5000 V DC, then converting to 4 kV peak AC via synchronverter with AVSG control. Stepped up to 25 kV RMS for grid synchrononization.

System Architecture
1. Solar PV Generation

    Custom PV model developed in Simulink.

    Variable irradiance and temperature profiles using Signal Builder.

    Output: ~2953 V DC (under STC conditions).

2. Hybrid MPPT Algorithm

    A Hybrid MPPT combines:

      VPA (Voltage Perturbation Approach)

      CPA (Current Perturbation Approach)

      ACP (Adaptive Conductance Perturbation)

   Features:

      Faster convergence to MPP.

      Reduced oscillations around MPP.

      High efficiency under partial shading and dynamic irradiance.

3. DC-DC Boost Converter

      Steps up the PV voltage from 2953 V to 5000 V DC.

      Controlled by the Hybrid MPPT algorithm output.

4. Synchronverter with AVSG Control

      Converts 5000 V DC to 4 kV peak AC.

      Uses IGBT-based SPWM inverter with AVSG-based phase angle generation.

      Implements frequency-adaptive control using real-time Δω feedback.

      Emulates inertia and damping properties of a synchronous machine.

 5. Grid Synchronization

      Output voltage stepped up via transformer to 25 kV RMS.

      Ensures seamless grid connection and stable synchronization using zero-crossing detection and θ(t)-based SPWM reference.

Key Features

  ✅ Hybrid MPPT combining VPA, CPA, and ACP methods
  ✅ AVSG control for frequency-adaptive synchronization
  ✅ θ(t)-based SPWM pulse generation
  ✅ Real-time irradiance and temperature input
  ✅ Efficient DC–AC conversion with minimal ripple
  ✅ Seamless grid connection at 25 kV RMS

Applications

  Grid-connected solar farms

  Microgrids and distributed energy systems

  Smart grid integration research

  Virtual inertia and synchronization studies
