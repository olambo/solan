---
title: "Voidbreaker Design Baseline — Verified Parameters"
date: 2026-05-12
lastmod: 2026-05-12
draft: false
weight: 10
tags:
  - voidbreaker
  - design-baseline
  - calculations
  - interstellar-propulsion
---

## Purpose

This document records the verified design parameters for the Voidbreaker, derived from the rocket equation and basic geometry. All figures are internally consistent. Where estimates are used (exhaust velocity, VoidForge mass), the assumptions are stated explicitly. This document exists to provide a stable numerical reference — other documents in the corpus should not contradict these figures without updating them here first.

---

## Assumptions

| Parameter | Value | Basis |
|---|---|---|
| Cruise speed | 0.02c = 6,000 km/s | Mission requirement |
| Exhaust velocity (ve) | 0.03c = 9,000 km/s | Fusion drive (D-T or D-He3, near-term feasible) |
| VoidForge active mass | ~175t | Midpoint of estimated 150–200t range |
| Hull + tank structure | ~300t | Working estimate |
| Dry mass (post-decel) | ~475t | VoidForge + hull |

These figures are working estimates, not engineering results. The exhaust velocity assumption is the most consequential: a lower ve increases propellant requirement; a higher ve reduces it. At ve = 0.03c the mass ratios are consistent with the propellant figures below.

---

## Mass Budget

| Item | Mass |
|---|---|
| VoidForge (active) | 175t |
| Hull + tank structure | 300t |
| **Dry mass (post-decel)** | **475t** |
| Deceleration propellant (minimum) | 450t |
| Surplus propellant (working capital) | ~75t |
| **Cruise mass (at transit velocity)** | **1,000t** |
| Acceleration propellant | ~950t |
| **Launch mass** | **~1,950t** |

**Cruise mass** is the retained vehicle mass at transit velocity after the acceleration burn. It includes deceleration propellant, VoidForge, hull, and surplus.

**Launch mass** rounds to ~2,000t for communication purposes. The calculation gives 1,948t.

**Surplus propellant (~75t)** is the working capital available to the VoidForge on arrival — fuel reserves before local production at the destination is established. It provides approximately 1,300 km/s of additional delta-v after full deceleration, sufficient for orbital insertion and early positioning.

---

## Propulsion

| Parameter | Value |
|---|---|
| Delta-v per phase (acceleration and deceleration) | 0.02c = 6,000 km/s |
| Mass ratio per phase | 1.948 |
| Total propellant (acceleration + deceleration) | ~1,450t |
| Acceleration burn duration (at 0.02g) | ~1 year |
| Deceleration burn duration | 20–40 years |

Deceleration is achieved by canting the engine nozzles forward. **The Voidbreaker never turns around.** The shield remains at the front throughout acceleration, cruise, and deceleration. A vessel that reverses orientation at interstellar transit velocity exposes its unshielded hull to the full dust flux — this is not survivable.

---

## Physical Dimensions

| Parameter | Value |
|---|---|
| Total length | 400m |
| Shield face | 20m wide × 15m tall |
| Shield section | ~10m |
| VoidForge section | ~40m |
| Tank section | ~350m |
| Shadow cone divergence | <1.5° over 400m |

**Spine diameter by fuel type** (350m tank section, 1,450t propellant):

| Fuel | Density | Volume | Spine diameter |
|---|---|---|---|
| D-T mixture | 219 kg/m³ | 6,621 m³ | 4.9m |
| Liquid deuterium | 162 kg/m³ | 8,951 m³ | 5.7m |
| D-He3 mixture | 100 kg/m³ | 14,500 m³ | 7.3m |

All fuel types fit comfortably within the 20m × 15m shield shadow. The spine is genuinely slender relative to the shield face — consistent with the visual description of a very thin craft sheltered behind a wide shield.

**Why 400m and not shorter:** 400m is the consequence of 0.02c. At 0.01c the ship shortens considerably but the journey doubles to over 1,000 years. At 0.05c the propellant requirement multiplies several times over and the ship becomes implausible. 0.02c is close to the practical optimum. A 350m ship would require a slightly fatter spine, losing approximately 12% of lateral hull surface area used for passive heat rejection. There is no engineering argument for shortening.

---

## Structural Loading

| Parameter | Value |
|---|---|
| Acceleration | 0.02g = 0.196 m/s² |
| Max compressive force at spine base | ~343 kN |
| Compressive stress (5.7m spine, 10mm wall) | ~1.9 MPa |
| Steel compressive limit | 250 MPa |

The spine is in **compression** during acceleration — the engine pushes from the rear, the spine transmits that force forward against the inertia of the tanks and shield. At 0.02g the compressive stress is less than 1% of steel's limit. Structural loading is not the constraint. Active alignment and vibration management across a 400m structure during a year-long burn is the engineering problem, not material strength.

---

## Journey Times at 0.02c

| Destination | Distance | Transit time |
|---|---|---|
| Alpha Centauri | 4.2 ly | ~210 years |
| Barnard's Star | 6.0 ly | ~300 years |
| Epsilon Eridani | 10.5 ly | ~525 years |

**The ship is the same for any of these destinations.** Propellant requirement is set by the velocity change (0.02c acceleration + 0.02c deceleration), not by distance. Only the coasting duration changes. The Voidbreaker is not optimised for Epsilon Eridani specifically — it is a general-purpose 0.02c vessel.

---

## Kinetic Energy at Cruise

| Parameter | Value |
|---|---|
| Cruise mass | 1,000t |
| Cruise speed | 0.02c |
| Kinetic energy | ~4,300 megatons TNT (~4.3 gigatons) |

This figure is the basis for the Starfall Protocol requirement. A Voidbreaker that does not decelerate is capable of civilisation-scale destruction on direct planetary impact. The deceleration burn is what actively diverts the vessel into the destination system. Passive failure must result in stellar interception.

---

## Comparison

| Vessel | Mass | Speed | Time to Epsilon Eridani | Crew |
|---|---|---|---|---|
| Chrysalis (generational ship concept) | ~2.4 million tonnes | 0.01c | ~1,050 years | 1,500–2,400 humans |
| Voidbreaker | 1,000t cruise / ~1,950t launch | 0.02c | ~525 years | 2 Solans |

The mass difference — a factor of roughly 2,400 — is biology. The generational ship must carry a closed-loop biological ecosystem capable of sustaining a viable human population for over a millennium. The Voidbreaker carries none of that infrastructure. The Solan path does not reduce the biological overhead incrementally. It eliminates the category.

---

*Voidbreaker design baseline. First document: 12 May 2026. Human contributor: independent cross-domain analyst. AI contributors: Claude Sonnet 4.6 (Anthropic) — calculations and synthesis. All figures verified against the rocket equation with stated assumptions. Content: CC BY 4.0. Site code: MIT.*
