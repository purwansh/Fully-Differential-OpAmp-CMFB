# Fully-Differential Two-Stage Miller Op-Amp with CMFB

This repository documents the design and simulation of a fully-differential two-stage operational amplifier with Miller compensation and dual common-mode feedback (CMFB) loops.

The project was completed as part of **EE610: Analog IC Design**.

## Specifications
- Closed-loop gain: -2
- Load: 20 kΩ || 1 pF
- Minimum DC loop gain: 60 dB
- Closed-loop bandwidth ≥ 1 MHz
- CMFB phase margin ≥ 60°

## Architecture
- First stage: NMOS differential pair with PMOS active loads
- Second stage: PMOS differential pair with NMOS active loads
- Compensation: Miller capacitors with series resistors
- CMFB: Two 5-transistor OTA-based CMFB loops

## Key Results
| Parameter | Value |
|--------|------|
| DC Loop Gain | 60.7 dB |
| Differential UGB | 3.95 MHz |
| Phase Margin | 64° |
| Closed-loop BW | 6.19 MHz |
| CMFB1 PM | 61.1° |
| CMFB2 PM | 72.6° |

## Tools Used
- Cadence Virtuoso
- Spectre Simulator
- 65nm CMOS Technology (PDK not included)

## Disclaimer
This repository contains only documentation and simulation results.  
No proprietary PDKs or Cadence design files are included.

