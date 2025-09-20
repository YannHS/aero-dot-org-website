---
title: Advanced Class - 2025
description: Overview of 2025 micro class aircraft design
---

{{< columns count=2 >}}
{{< column >}}
## Project Longshot
### The 2025 Aero uOttawa Advanced Class aircraft platform is designed for autonomous payload delivery and capture via VTOL and conventional flight.

|              |          | 
| ------       | ------   |  
| Wingspan     | 1.2 m    | 
| Length       | 0.97 m   | 
| Mass (empty) | `1.5 kg  |

{{< /column >}}

{{< model-viewer model="/models/advanced-2025.glb" poster="/models/advanced-2025.webp" camera-orbit="-137deg 80.15deg 2.514m" field-of-view="30" skybox-image="/models/stem.webp" skybox-height="0.3m" exposure="2">}}



{{< /model-viewer >}}

{{< /columns >}}



{{< columns count=2 >}}

{{< column >}}
Built around a modular carbon fibre and 3D-printed frame, the aircraft features a 1.2 m wingspan with a Clark-Y airfoil for aerodynamic efficiency. Powered by three lightweight T-Motor MN2806 units and vectored front motors for vertical lift, it balances thrust and weight under strict competition limits. A Pixhawk 6C flight controller running ArduPilot handles navigation and stability, supported by a Raspberry Pi CM4 for onboard computer vision and RTK-enabled GNSS for precise positioning. The design emphasizes reliability, modularity, and repairability, offering a strong foundation for mission success in the SAE Advanced Class competition {{< emoji src="/emoji/Blobhaj_Thanks_Wow.png" >}}.
{{< /column >}}

{{< galimg src="img/adv-2025-longshot-glamour.jpg" caption="Project Longshot, assembled for a glamour shot" >}}

{{< /columns >}}

## Airframe Construction

{{< columns count=2 >}}

{{< column >}}

Our airframe is based on a system of carbon fiber rods glued to 3d printed splines. Using Splines allows the components attached to the frame to be easily replaced, while still being securely mounted. This allows us to take advantage of the rapid iterative process from using 3d printed components.
{{< /column >}}

{{< galimg src="img/adv-2025-spline.jpg" caption="Our 3d printed Spline glued to a carbon bar" >}}

{{< /columns >}}




## Wing Construction

{{< columns count=2 >}}

{{< column >}}

We chose an new, innovative technique for wing manufaturing: 3d printing. 3d printing our airfoils allows for flexibility when selecting our airfoil as well as the overall wing shape. Since we used ASA Aero, a foaming filament that has an extremely low density, our wing is also extremely light for it's size. The 3d printed wing segments can be slid onto our carbon bar frame, keeping our wings modular while allowing easy replacement of damaged wing sections.
{{< /column >}}

{{< galimg src="img/adv-2025-3d-printed-wing.jpg" caption="Our 3d printed wing on the print bed" >}}

{{< /columns >}}



## Electronics

{{< columns count=2 >}}

{{< column >}}

Cantered around a Pixhawk 6c, we assembled an electronics system from off-the-shelf parts for rapid prototyping and knowledge that all individual modules were well tested. The Pixhawk 6c was chosen for its robust IO, featureset, and compatibility with the [Ardupilot](https://ardupilot.org/) firmware. Ardupilot is able to perform autonomous and controlled stabilized flight in both Horizontal and VTOL configurations, perform precision landing using optical data, and perform the VTOL to Horizontal flight transition. To acquire the realtime precision landing data, we are using a Raspberry Pi CM4 module with a global shutter monochrome camera to optically track a fiducial tag on the payload at around 15hz. Control and Telemetry is accomplished using two separate modules: an Sik telemetry module and an ERLS module for manual control and arming. The Pixhawk uses a digital protocol, DShot, for ESC communication, and analog PWM for servos.
{{< /column >}}
<div>
{{< galimg src="img/adv-2025-electronics-plate.jpg" caption="The electronics all plugged in" >}}
{{< spacer 50 >}}
{{< galimg src="img/adv-2025-ochin-and-camera.jpg" caption="the CM4 stack wired to the Arducam OV2311 as a proof-of-concept" >}}
</div>
{{< /columns >}}

---

## Photo Gallery
{{< gallery >}} 
