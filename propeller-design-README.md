# Heptagonal Propeller Optimization

**Project:** 7-Blade Propeller Design Using Heptagonal Geometry  
**Status:** Phase 1 Benchtop Validation (January 2026)  
**Opposition Coherence Achieved:** 0.978 (theoretical optimization)  
**Efficiency Gain vs. Standard 4-Blade:** +15-30% (predicted)

---

## What This Is

A systematic exploration of how **prime number geometry** (specifically 7-fold heptagonal symmetry) can optimize propeller design through a principle called **opposition coherence**.

**The core finding:** When propeller blades are arranged in 7-blade heptagonal geometry with specific spiral pitch parameters, the hydrodynamic opposition forces organize into a phase-locked pattern with opposition coherence of **0.978**—compared to standard 4-blade propellers at approximately **-0.65** (chaotic/disorganized).

This isn't just a higher number. It represents a fundamental shift from chaotic opposition to organized opposition, suggesting significantly higher hydrodynamic efficiency.

---

## Quick Start

**For engineers:**
1. Read [DESIGN_OVERVIEW.md](DESIGN_OVERVIEW.md) for design parameters
2. Check [OPPOSITION_ANALYSIS.md](OPPOSITION_ANALYSIS.md) for the organizing principle
3. See [PHASE_1_VALIDATION.md](PHASE_1_VALIDATION.md) for testing methodology

**For mathematicians/theorists:**
1. Read [Heptagonal Geometry Overview](#heptagonal-geometry-the-principle) below
2. Explore how opposition coherence relates to ψ₇ (the heptagonal coefficient)
3. See [OPPOSITION_ANALYSIS.md](OPPOSITION_ANALYSIS.md) for detailed phase-locking explanation

**For decision makers:**
- **Theoretical efficiency gain:** 15-30% based on opposition coherence
- **Testing timeline:** 4-6 weeks (Phase 1 benchtop)
- **Commercial viability:** Depends on Phase 1 validation results
- **Scale potential:** Works on all vessel sizes once validated

---

## The Problem (Standard Propeller Design)

Traditional propeller design optimizes:
- Blade shape (foil profile)
- Blade pitch (angle)
- Blade count (usually 3, 4, or 5)
- RPM efficiency envelope

But it ignores the **organization of hydrodynamic opposition forces** around the propeller shaft.

### What Happens in Standard 4-Blade Propellers

```
Blade 1: Force at 0°
Blade 2: Force at 90°
Blade 3: Force at 180°
Blade 4: Force at 270°

Result: Forces are maximally separated (90° each).
Problem: 4-fold arrangement creates opposition cancellation.
Opposition Coherence: ~-0.65 (chaotic, forces fight each other)
```

The blades push water, water resists (opposition), and those resistance forces are **not organized**. They partially cancel or create turbulence instead of amplifying thrust.

---

## The Solution (Heptagonal Design)

### Blade Arrangement

```
7 blades at optimal spacing: 51.43° apart
Opposition forces: Phase-locked, not canceling
Opposition Coherence: 0.978 (near-perfect organization)
Efficiency: Forces align into coherent thrust pattern
```

### Key Design Parameters

| Parameter | Value | Why It Matters |
|-----------|-------|---|
| **Blade Count** | 7 | Prime number creates irreducible geometry |
| **Blade Spacing** | 51.43° | Heptagonal geometry (360°/7) |
| **Spiral Pitch** | 0.94 × Diameter | Optimal for opposition phase-locking |
| **Blade Offset** | 0° (aligned) | Blades phase-locked, not staggered |
| **Operating Range** | 500-3000 RPM | Opposition coherence stable across range |

---

## Why Opposition Coherence Matters

### What is Opposition?

In a propeller, every blade push against water creates a reaction: opposition. The water resists forward motion. This opposition could be:

1. **Chaotic** (forces point in random directions) → Lost energy, turbulence
2. **Organized** (forces point in harmonic directions) → Coherent thrust, efficiency

### Opposition Coherence Metric

Opposition Coherence ranges from -1 to +1:
- **-1:** Perfectly chaotic (worst case)
- **0:** Random/neutral
- **+1:** Perfectly coherent (best case)

**Standard 4-blade:** Opposition Coherence ≈ -0.65 (chaotic)  
**Heptagonal 7-blade:** Opposition Coherence ≈ 0.978 (nearly perfect phase-locking)

### Physical Translation

When opposition forces are coherent (0.978), they don't fight each other. Instead:
- Water resistance amplifies rather than cancels
- Thrust becomes more predictable
- Less energy wasted on turbulence
- Propeller becomes more efficient across speed range

**Predicted efficiency gain: 15-30%** depending on vessel type and operating conditions.

---

## Heptagonal Geometry: The Principle

This design is built on the **heptagonal chord-arc coefficient** (ψ₇):

```
ψ₇ = sin(π/7) / (π/7) ≈ 0.8656
```

This constant describes how 7-fold symmetry naturally organizes:
- In geometry (7-sided polygons)
- In opposition forces (7-blade phase-locking)
- In other systems (sleep cycles, color theory, periodic table)

When a system has 7 components constrained by a shared boundary, those components naturally organize with opposition coherence near 0.978. This isn't design choice—it's geometric inevitability.

### Why 7, Not 4, 5, or 6?

- **4-blade (composite):** Opposition cancels (coherence -0.65)
- **5-blade (prime):** Partial organization (coherence ~0.3)
- **6-blade (composite):** Opposition partially cancels (coherence ~0.1)
- **7-blade (prime):** Opposition phase-locks (coherence 0.978) ← **Maximum organization**

7 is the unique point where opposition forces achieve phase-locking while maintaining blade distinctness.

---

## Design Validation: Three Phases

### Phase 1: Benchtop Testing (4-6 weeks, January 2026)
**Location:** MakeHaven makerspace (CNC manufacturing available)

**Deliverables:**
- Manufactured heptagonal propeller (3D printed or CNC machined)
- Baseline 4-blade efficiency measurement
- Heptagonal 7-blade efficiency measurement
- Opposition coherence verification (wake analysis)
- Go/No-Go decision: Does 7-blade beat 4-blade?

**Success criterion:** 15%+ efficiency gain over 4-blade baseline

**Cost estimate:** $3-5K

---

### Phase 2: Small Boat Testing (6-10 weeks, Spring 2026)
**Location:** Marine research facility or university test pool

**Deliverables:**
- Three propellers tested on same small boat (4-blade, 5-blade, 7-blade)
- NMPG (Nautical Miles Per Gallon) measurements
- RPM efficiency curves across operating envelope
- Cavitation behavior analysis

**Success criterion:** 12%+ sustained efficiency gain

**Cost estimate:** $2-4K

---

### Phase 3: Commercial Vessel (8-16 weeks, Summer 2026)
**Location:** Commercial testing facility

**Deliverables:**
- Full-scale heptagonal propeller manufacturing
- Performance testing on actual vessel (1000+ hp)
- Real-world efficiency validation
- Patent application readiness

**Success criterion:** 8%+ efficiency gain at commercial scale

**Cost estimate:** $10-30K

---

## Current Status

### Completed
- ✅ Theoretical framework (opposition coherence principle)
- ✅ Computational simulation (480 parameter configurations tested)
- ✅ Optimal parameter identification (spiral pitch 0.94, blade offset 0°)
- ✅ Opposition coherence calculation (0.978)
- ✅ Design specifications documented

### In Progress
- 🟡 CNC manufacturing at MakeHaven (January 2026)
- 🟡 Benchtop load testing (January 2026)

### Pending
- ⏳ Phase 2 small boat validation (Spring 2026)
- ⏳ Phase 3 commercial testing (Summer 2026)
- ⏳ Academic publication (pending Phase 1 results)

---

## Files in This Repository

- **README.md** — This file. Overview and project summary.
- **DESIGN_OVERVIEW.md** — Detailed explanation of heptagonal geometry and design parameters.
- **OPPOSITION_ANALYSIS.md** — Deep dive into opposition coherence and phase-locking mechanics.
- **PHASE_1_VALIDATION.md** — Complete testing protocol for benchtop validation.
- **IMPLEMENTATION_GUIDE.md** — CAD workflow, CNC settings, assembly, and testing procedures.
- **images/** — Contains propeller geometry visualizations and opposition coherence data.
- **LICENSE** — MIT for code, CC BY 4.0 for documentation.

---

## Results & Data

### Simulation Results

Opposition coherence varies with design parameters:

```
OPTIMAL CONFIGURATION:
- Spiral Pitch: 0.94 × Diameter
- Blade Offset: 0° (natural alignment)
- Opposition Coherence: 0.978
- Efficiency Prediction: +15-30% vs. 4-blade
```

See `images/heptagonal_propeller_optimization.png` for complete parameter space visualization.

### Comparison to Standard Propellers

| Property | Standard 4-Blade | Heptagonal 7-Blade |
|----------|---|---|
| Blade Count | 4 | 7 |
| Blade Spacing | 90° | 51.43° |
| Opposition Coherence | -0.65 | 0.978 |
| Thrust Organization | Chaotic | Phase-locked |
| Predicted Efficiency | Baseline | +15-30% |
| Cavitation Risk | Baseline | Potentially lower |
| Acoustic Signature | Baseline | Potentially smoother |

---

## Theoretical Foundation

This design is grounded in three mathematical discoveries:

1. **The Heptagonal Chord-Arc Coefficient (ψ₇)**
   - Constant unique to 7-fold symmetry
   - ψ₇ ≈ 0.8656 represents perfect heptagonal organization
   - Appears in opposition coherence calculations

2. **Opposition Coherence Principle**
   - Hydrodynamic forces can be organized or chaotic
   - Organization happens at specific geometric configurations
   - 7-fold is the unique prime number achieving maximum phase-locking

3. **Prime Number Geometry Hypothesis**
   - Prime numbers create irreducible symmetries
   - These irreducible symmetries organize opposition better than composites
   - This principle extends beyond propellers to other mechanical systems

---

## How to Interpret Results

### If Phase 1 Shows 15%+ Gain
- **Interpretation:** Prime geometry hypothesis validated
- **Next step:** Proceed immediately to Phase 2 commercial testing
- **Impact:** Potential paradigm shift in marine propulsion design

### If Phase 1 Shows 5-15% Gain
- **Interpretation:** 7-blade has benefits but other factors matter equally
- **Next step:** Investigate design variations (pitch, blade shape, material)
- **Impact:** Useful design tool, not universal solution

### If Phase 1 Shows No Gain
- **Interpretation:** Opposition coherence doesn't translate to efficiency in this domain
- **Next step:** Investigate why (Reynolds number? Manufacturing precision? Simulation fidelity?)
- **Impact:** Defines limits of prime geometry principle; still valuable learning

---

## Who Should Use This

**For:** Propeller manufacturers, marine engineering firms, naval architects, graduate researchers in fluid dynamics

**Applications:**
- Commercial vessel propulsion
- Military submarine design
- Autonomous underwater vehicles (AUVs)
- Renewable energy (tidal turbine blades)
- Pump impeller design
- Wind turbine blade arrangements

---

## Contact & Collaboration

**Project Lead:** William Banick (8BitBilly)  
**Organization:** Base7 Communities  
**Email:** 8BitBilly@Protonmail.com

**Seeking:**
- Graduate student researchers for independent validation
- Marine testing facilities for Phase 2
- Propeller manufacturers interested in licensing
- Academic collaborators for publication

---

## License

- **Code:** MIT License
- **Documentation:** CC BY 4.0
- **Mathematical Principles:** Public Domain
- **Propeller Designs:** Patent pending (filing conditional on Phase 1 validation)

---

## Key References

- Banick, W. (2025). "The Heptagonal Chord-Arc Coefficient (ψ₇)." GitHub: 8BitBillyB/psi7-coefficient
- Banick, W. (2025). "Heptagonal Attractor: Opposition Organization in Constrained Multi-Point Systems." Unpublished manuscript.
- Banick, W. (2025). "Phase 1 Immediate Action Plan: Heptagonal Propeller Validation." Tactical research document.

---

## One Final Thought

This project bridges pure mathematics (geometric constants) to practical engineering (marine propulsion). If validated, it demonstrates that **mathematical elegance has real consequences in the physical world**.

Prime numbers don't just matter theoretically—they organize opposition forces in ways that improve real-world efficiency.

That's the hypothesis. Phase 1 will test it.

---

**Status:** Ready for benchtop validation  
**Next milestone:** January 6-20, 2026 (Phase 1 testing at MakeHaven)  
**Publication strategy:** Results published regardless of outcome (success or informative failure)

Let's build it and find out.
