# EXPERIMENT NO. 4 – HALF WAVE AND FULL WAVE BRIDGE RECTIFIERS

| **Name:** | | **Reg. No.:** | |
|---|---|---|---|
| **Date:** | | **Batch / Section:** | |

---

## AIM

To study the half wave and full wave bridge rectifiers with and without filter and to observe their input and output waveforms using Proteus.

## COMPONENTS AND EQUIPMENT REQUIRED

| S. No. | Components / Equipment |
|:---:|:---|
| 1 | Diodes |
| 2 | Resistor (load) |
| 3 | Capacitors (filter) |
| 4 | Step-down transformer |
| 5 | Voltmeter |
| 6 | Ammeter |
| 7 | Breadboard |
| 8 | CRO |
| 9 | Connecting wires |
| 10 | Simulation software – Proteus Design Suite |

## THEORY

A rectifier changes AC to DC and is an essential part of a power supply. The unique property of a diode, permitting current to flow in only one direction, is utilised in rectifiers.

### Half wave rectifier

Mains supply is applied to the primary of the step-down transformer. All the positive half cycles of the stepped-down AC supply pass through the diode and all the negative half cycles are eliminated. The peak value of the output voltage is less than the peak value of the input voltage by about 0.6 V because of the voltage drop across the diode. For a half wave rectifier, **Vrms = Vm/2** and **Vdc = Vm/π**, where Vrms is the RMS value of the output, Vdc is the average value of the output and Vm is the peak value of the output.

### Full wave bridge rectifier

During the positive half cycle of the secondary voltage, diodes D1 and D3 are forward biased and D2 and D4 are reverse biased, so current flows through the secondary winding, D1, the load resistor and D3. During the negative half cycle, D2 and D4 are forward biased and D1 and D3 are reverse biased, so current flows through the secondary winding, D2, the load resistor and D4. In both half cycles the current through the load resistor is in the same direction. The peak output voltage is less than the peak input voltage by about 1.2 V due to the drop across two diodes. For a full wave bridge rectifier, **Vrms = Vm/√2** and **Vdc = 2Vm/π**.

### Filters

All rectifier outputs contain a considerable amount of ripple in addition to the DC component. To remove the AC components, a filter is connected at the output of the rectifier. Capacitor input, choke input, RC, CRC, LC and CLC filters are commonly used; the capacitor input filter is the simplest and cheapest. A high-value capacitor C is connected in shunt with the load resistor RL. The capacitor charges to the peak voltage when a half cycle appears at the output. After the peak, the capacitor discharges slowly through RL, since the diode is reverse biased by the capacitor voltage. Before the capacitor voltage drops substantially, the next output cycle arrives and the capacitor recharges to the peak.

## PROCEDURE

1. Wire up the half wave rectifier circuit without capacitor after testing all the components.
2. Switch on the mains supply. Observe the transformer secondary voltage waveform and the output voltage waveform across the load resistor simultaneously on the CRO.
3. Connect the capacitor filter across the load and observe the waveforms. Repeat for different capacitor values.
4. Repeat the above steps for the full wave bridge rectifier.
5. Simulate both rectifiers, with and without filter, in Proteus and capture the input and output waveforms on the virtual oscilloscope.

## CIRCUIT DIAGRAMS

### Half wave rectifier without filter

<img width="1183" height="668" alt="Screenshot 2026-11-25 123514" src="https://github.com/user-attachments/assets/cd2dde0c-acf3-4381-a8b8-e87738f7800c" />


**Figure 1:** Half wave rectifier without filter

### Half wave rectifier with filter

<img width="1255" height="736" alt="Screenshot 2026-11-25 134126" src="https://github.com/user-attachments/assets/161e423b-fa4e-4e60-b35c-0829c7e60db9" />


**Figure 2:** Half wave rectifier with filter

### Full wave bridge rectifier without filter

<img width="1155" height="723" alt="Screenshot 2026-11-25 141640" src="https://github.com/user-attachments/assets/db56c7d3-2159-46cb-8a5e-ecdc83558208" />


**Figure 3:** Full wave bridge rectifier without filter

### Full wave bridge rectifier with filter

<img width="1075" height="677" alt="Screenshot 2026-11-25 141815" src="https://github.com/user-attachments/assets/1fee547b-a6f6-4229-9a5a-8bff7d92194e" />


**Figure 4:** Full wave bridge rectifier with filter

## SIMULATION AND WAVEFORMS USING PROTEUS

Build each rectifier in Proteus, with and without the capacitor filter. Use the virtual oscilloscope to display the input (secondary) and output waveforms together, and paste the screenshots below.

### Half wave rectifier without filter – waveform

<img width="1745" height="947" alt="Screenshot 2026-11-25 123434" src="https://github.com/user-attachments/assets/388df2da-e5a1-4924-bd9a-53bc06ff15e2" />


**Figure 5:** Proteus waveform – half wave rectifier without filter

### Half wave rectifier with filter – waveform

<img width="1480" height="886" alt="Screenshot 2026-11-25 134111" src="https://github.com/user-attachments/assets/6d276c7a-a736-49fe-ab92-6c7094741d0e" />


**Figure 6:** Proteus waveform – half wave rectifier with filter

### Full wave bridge rectifier without filter – waveform

<img width="1566" height="877" alt="Screenshot 2026-11-25 141628" src="https://github.com/user-attachments/assets/4f3b2fd2-7785-482d-a9c1-0e5168de8ebc" />


**Figure 7:** Proteus waveform – full wave bridge rectifier without filter

### Full wave bridge rectifier with filter – waveform

<img width="1608" height="892" alt="Screenshot 2026-11-25 141804" src="https://github.com/user-attachments/assets/faccbb14-6c53-487e-9ff1-63cd91a1695c" />


**Figure 8:** Proteus waveform – full wave bridge rectifier with filter

## FORMULAE

### A. Half wave rectifier

- Average (DC) voltage: **Vdc = Vm / π**
- Average (DC) current: **Idc = Im / π**
- RMS voltage: **Vrms = Vm / 2**
- RMS current: **Irms = Im / 2**
- Ripple factor: **γ = √[(Vrms / Vdc)² − 1] = 1.21**
- Rectification efficiency: **η = Pdc / Pac × 100 = (Idc² RL) / (Irms² RL) × 100 = 40.6 %**
- Form factor: **FF = Vrms / Vdc = 1.57**
- Peak factor: **PF = Vm / Vrms = 2**
- Peak inverse voltage: **PIV = Vm**

### B. Full wave bridge rectifier

- Average (DC) voltage: **Vdc = 2Vm / π**
- Average (DC) current: **Idc = 2Im / π**
- RMS voltage: **Vrms = Vm / √2**
- RMS current: **Irms = Im / √2**
- Ripple factor: **γ = √[(Vrms / Vdc)² − 1] = 0.482**
- Rectification efficiency: **η = Pdc / Pac × 100 = (Idc² RL) / (Irms² RL) × 100 = 81.2 %**
- Form factor: **FF = Vrms / Vdc = 1.11**
- Peak factor: **PF = Vm / Vrms = √2 = 1.414**
- Peak inverse voltage: **PIV = Vm**

### C. With capacitor filter

- Half wave: **γ = 1 / (2√3 f C RL)**
- Full wave bridge: **γ = 1 / (4√3 f C RL)**

### D. Regulation

- **% Regulation = (VNL − VFL) / VFL × 100**

Vm – peak output voltage; Im – peak load current (Im = Vm / RL); RL – load resistance; f – supply frequency (50 Hz); C – filter capacitance; VNL – no-load voltage; VFL – full-load voltage.

## RESULT

Thus, the input and output waveforms of the half wave and full wave bridge rectifiers with and without filter were observed using Proteus.
