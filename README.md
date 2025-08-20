# Two-Layer PCB for IR Sensor Module

This project is a custom-designed two-layer PCB for an infrared (IR) proximity sensor module, created using KiCad 9.0. The aim was to build a compact and reliable board that could be used for object detection, proximity sensing, or reflective surface detection.  

The module is built around three main parts:
- An IR LED to emit infrared light
- A photodiode to detect the reflected light
- An op-amp comparator to process the signal and output a clean digital logic level  

The design was done with manufacturing in mind, keeping the board simple, efficient, and noise-resistant.

## Schematic Design

The schematic includes:
- IR LED for transmitting modulated IR light  
- Photodiode for sensing reflected light  
- Op-amp comparator for generating a digital HIGH/LOW output  
- Resistor network for biasing and setting comparator thresholds  

## PCB Layout

Component placement:
- IR LED and photodiode are placed at the edge of the board for proper optical alignment with the environment  
- The op-amp is placed centrally to allow balanced trace routing  
- Custom footprints were used in some cases to simplify routing and save space  

Routing strategy:
- Sensitive signals (especially the photodiode output) are kept short and direct to reduce noise  
- A ground plane was added to the bottom layer for shielding and noise reduction  
- Power and output signals are routed on the top layer with standard trace widths  
- Vias are minimized to maintain signal integrity  
- Components are clearly labeled on the silkscreen  

## Files Included

The repository includes the following files:
- 2-Layer-Proximity-PCB.kicad_pcb – the PCB layout  
- 2-Layer-Proximity-PCB.kicad_sch – the schematic file  
- Gerbers/ – a folder containing the full Gerber set, exported in JLCPCB format and ready for fabrication  

## Verification

The design was checked using KiCad’s DRC (Design Rule Check) and ERC (Electrical Rule Check) tools to ensure it meets both electrical and manufacturing requirements.  

## Conclusion

This PCB design provides a simple but effective IR sensor module that is well-suited for small-scale proximity detection applications. Working on this project gave me more hands-on experience in PCB design, especially with handling analog signals and optimizing layouts for sensor performance.
