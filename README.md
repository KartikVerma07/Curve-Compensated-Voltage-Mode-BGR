# Curve Compensated Voltage Mode Bandgap Reference (BGR) 

## Overview
This repository contains the design and analysis of Curve Compensated Voltage Mode Bandgap References (BGRs). 
This readme includes brief explanations, schematics, and test results for the BGR components, including CTAT and PTAT components, 
folded current mirror, two-stage operational amplifier, and various compensation techniques to minimize temperature drift.

## Contents

1. **Two Stage Operational Amplifier:**
   - Consists of a differential amplifier and a common source amplifier for higher gain.
   - Gain of 60dB is achieved and Phase Margin of 66.19° can be seen in Bode Plot mentioned below:
     - Bode Plot:
   - ![BodePlot_graph](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/assets/60437757/eef02325-e2ee-474e-8a37-b340ddb250d5)
     - Schematic:
   - ![OpAmp_schematic](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/assets/60437757/48a36561-da47-45ae-9b62-7e32b8b25cfc)

  
2. **Voltage Mode Bandgap Reference (BGR):**
   - Provides a stable reference voltage by combining Complementary To Absolute Temperature (CTAT) and Proportional To Absolute Temperature (PTAT) components.
   - Using PNP BJTs : Vref of 1.197 V at 25°C
   ![BGR_pnp_graph](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/assets/60437757/c6a15e6d-73cb-4dc4-b81b-9b992c75b0bc)
     - Schematic
   - ![BGRPNP](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/assets/60437757/2832f9b1-bcc8-4319-b5ce-80ddbf4d7104)
   - Using NPN BJTs : Vref of 1.235 V at 25°C
   - ![BGR_npn_graph](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/assets/60437757/660e9f87-b5fa-450f-be44-74c3aea3a446)
     - Schematic
   - ![BGR_NPN](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/assets/60437757/ec0e17b8-fc7a-4f99-87d2-7e61aededc36)

3. **Curve Compensation Techniques:**
   - *Temperature Dependent Resistor Ratio Technique:*
     - Reference to the Paper: [A_2-V_23-A_5.3-ppm_C_curvature-compensated_CMOS_bandgap_voltage_reference.pdf](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/files/15395097/A_2-V_23-A_5.3-ppm_C_curvature-compensated_CMOS_bandgap_voltage_reference.pdf)
     - R4(27℃) = R2(27℃) + R3(27℃)
     - Schematic 
     ![CC_2 0](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/assets/60437757/b73f9759-409d-41b3-8d39-e04a81020d28)


   - *Curvature Up & Down Cancellation:*
     - Reference to the Paper: [New_Curvature-Compensation_Technique_for_CMOS_Bandgap_Reference_With_Sub-1-V_Operation.pdf](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/files/15395116/New_Curvature-Compensation_Technique_for_CMOS_Bandgap_Reference_With_Sub-1-V_Operation.pdf)
     - Schematic 
     ![CC2_schematic+tb(subtract)](https://github.com/KartikVerma07/Curve-Compensated-Voltage-Mode-BGR/assets/60437757/9d7d5fd3-cd50-45be-a74a-638bba56f660)

## Usage
This repository provides schematics and test results for the design and implementation of voltage mode BGR and associated curve compensation techniques. The provided figures and descriptions will help users understand the functionality and performance of each component. To use these designs in your projects, refer to the provided schematics and adjust the parameters as needed for your specific requirements.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

For further information, refer to the detailed descriptions and schematics provided in the repository. If you have any questions or need assistance, feel free to open an issue or contact me at vkartik764@gmail.com
    
