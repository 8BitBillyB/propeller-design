# IMMEDIATE ACTION PLAN
## Getting Phase 1 Benchtop Testing Started

---

## THIS WEEK: Make Three Decisions

### Decision 1: Testing Facility
**What you need:** A water tank or flow system where you can test a small propeller

**Options ranked by practicality:**

**BEST: University engineering lab (Fluid Mechanics, Naval Architecture, or Mechanical Engineering)**
- Most likely to have: water tank, load cells, precision instruments
- Access usually available: contact department chair or grad student advisor
- Cost: Often free or minimal in exchange for publishing results
- Contact script: "I'm investigating a novel propeller geometry and need benchtop validation. Can I access your water tank and load cell for 4-6 weeks of testing?"

**GOOD: Commercial marine testing facility**
- Examples: Universities with naval engineering, marine engineering services companies, propeller manufacturers' test facilities
- Cost: $100-500 for tank time depending on facility
- Advantage: Professional-grade equipment, data expertise
- Search: "propeller testing facility near [your location]"

**MODERATE: DIY Recirculating System**
- Build a 2-3m diameter tank with pump circulation (YouTube has guides)
- Cost: $500-2000 for pump, tank, piping
- Timeline: 2-3 weeks to build before testing
- Advantage: Your facility, flexible schedule
- Disadvantage: Less precision than professional lab

**LEAST (but possible): Open water test in controlled conditions**
- Use a dock-mounted test stand with thrust sensor
- Measure small propeller in still/shallow water
- Cost: ~$200-500 for thrust sensor + mounting hardware
- Advantage: Immediate start
- Disadvantage: Less control over water velocity, wake interference from dock

**ACTION:** Contact 2-3 options this week. Ask: "Can I test a small propeller in your facility? I need 4-6 hours of tank time over 4-6 weeks."

---

### Decision 2: 3D Printing or Machining

**Option A: 3D Print (FASTER, CHEAPER)**
- Cost: $50-150 per propeller (5 total = $250-750)
- Time: 1-2 weeks from design to hand
- Quality: Good for concept validation, acceptable for Phase 1
- Services: Shapeways, Sculpteo, or local makerspace
- File format needed: STL (can generate from simulation code)

**Option B: Machine or Cast (MORE PRECISE)**
- Cost: $300-500 per propeller (5 total = $1500-2500)
- Time: 2-4 weeks
- Quality: Production-grade, exact to specifications
- Where: Local machine shop or propeller manufacturer
- Better if: You want replication for Phase 2-3

**RECOMMENDATION for Phase 1:** Start with 3D printing. If it works, upgrade to machined versions for Phase 2.

**ACTION:** 
- I can create exact CAD specifications for all 5 propellers this week
- You choose 3D print service or local shop
- Order this week for delivery in 2 weeks

---

### Decision 3: Motor and Load Cell

**Motor (Variable-speed, 0.5-2 hp):**
- Electric motor + variable frequency drive (VFD): $200-400 total
- Or: DC motor + PWM speed controller: $100-200
- Or: Rent from local tool rental: $30-50/week
- Need: Can reach 500-3000 RPM, 0.5-2 hp continuous

**Load Cell (for measuring thrust):**
- Tension load cell (0-50 lbf range): $150-300
- With digital display: +$50-100
- Alternative: Use bathroom scale + mechanical lever system (free but less precise)
- Need: Measures force perpendicular to shaft (vertical setup typically)

**Data Logging:**
- Laptop + USB data acquisition card: $300-500 (one-time)
- Or: Rent from university lab
- Need: Simultaneous logging of thrust, torque, RPM

**TOTAL PHASE 1 EQUIPMENT COST:** $500-1500 (excluding tank, which is facility-provided)

**ACTION:** 
- Check what's available at your test facility first
- Many university labs have motors and load cells—just need propellers
- Document what exists vs. what you need to acquire

---

## THIS MONTH: Build Phase 1 Test Rig

### Step 1: Design Propeller Geometry (Week 1)

I'll create exact CAD files:
- **Heptagonal 7-blade:** spiral pitch 0.94×D, 0° offset, blade twist 15°
- **Standard 4-blade:** matched diameter, typical design
- **Standard 3-blade:** for comparison
- **Standard 5-blade:** optimization control
- **Standard 6-blade:** composite test

Each file will specify:
- Blade root diameter
- Hub geometry
- Attachment point (standardized quick-change)

### Step 2: Order Propellers (Week 1-2)

- Upload CAD files to 3D print service or machine shop
- Specify material: ABS plastic (light, rigid, cost-effective) or aluminum
- Delivery target: 2 weeks

### Step 3: Assemble Test Stand (Week 2-3)

**Mounting Design:**
- Motor on fixed stand
- Propeller shaft passes through tank wall (sealed bearing)
- Thrust sensor between motor and propeller
- Load cell positioned to measure vertical force (perpendicular to rotation)

**Schematic I'll provide:**
- Exact dimensions for motor mounting
- Bearing/seal specifications
- Quick-change propeller hub design (change blades in <2 minutes)
- Water jacket if needed (cooling)

### Step 4: Calibrate Sensors (Week 3)

- Load cell: Verify with known weights (0, 5, 10, 20, 50 lbf)
- Tachometer: Verify against strobe light or laser tach
- RPM sensor: Confirm accuracy across 500-3000 RPM range
- Temperature sensor: Baseline water temperature

---

## FIRST ACTUAL TEST: 4 Weeks In

**Setup:** 
- Motor running in tank with 4-blade baseline propeller
- Water velocity: 0.50 m/s (THIS is critical—matches simulation)

**Test sequence (30 minutes total):**
1. RPM = 1000, steady 60 sec → record thrust, power
2. RPM = 1500, steady 60 sec → record
3. RPM = 2000, steady 60 sec → record
4. RPM = 2500, steady 60 sec → record
5. RPM = 3000, steady 60 sec → record
6. Return to 1000 RPM, verify repeatability (check we haven't drifted)

**Data you're collecting:**
```
RPM | Thrust (lbf) | Power (watts) | Calculated Efficiency
1000 | [measured] | [measured] | Thrust × Velocity / Power
1500 | [measured] | [measured] | ...
etc.
```

**Success criteria:** Repeatability within ±2% (same RPM, same thrust/power)

---

## AFTER BASELINE: Compare Against Heptagonal

**Once 4-blade baseline is reliable:**
1. Stop motor
2. Quick-change to 7-blade heptagonal
3. Repeat same test sequence
4. Compare efficiency at each RPM

**Primary result:**
```
Efficiency Gain at 1000 RPM = (Eff_Heptagonal / Eff_Baseline - 1) × 100%

Expected (if simulation is right): +15-25%
Minimum acceptance: +10%
Failure threshold: <5%
```

---

## CONTINGENCY: If Test Facility Not Available

**Fallback option (rapid prototyping):**

Use a **small trolling motor** (electric boat motor, ~500W):
- Cost: $150-300 (or borrow)
- Thrust range: 5-20 lbf (measurable with bathroom scale + pulley)
- Plug-and-play: no need for lab tank
- Test location: backyard pool or dock with circulating water

**Setup:**
1. Attach trolling motor to rigid stand (pool-side or dock)
2. Motor propeller submerged but accessible
3. Bathroom scale on floor, thrust-measuring rig on top
4. Measure at different water depths/velocities

**Tradeoff:** Lower precision, but still validates concept. Could start Phase 1 in 2 weeks instead of 4.

---

## WHAT I NEED FROM YOU

**This week, answer:**

1. **Test facility:** Which option are you exploring? (university lab, DIY, commercial, fallback?)
   
2. **Timeline:** When do you want physical testing to START? (2 weeks? 4 weeks? 8 weeks?)

3. **Budget:** Rough budget for propellers + sensors? (under $1k? $2-5k? flexible?)

4. **Location:** Where are you? (helps me suggest nearby universities or marine facilities)

5. **Prior experience:** Have you worked with data acquisition, mechanical testing, or marine systems before? (helps me scope instructions)

---

## DELIVERABLES I'LL CREATE IMMEDIATELY

Once you confirm facility access, I'll generate:

1. **Exact propeller CAD files** (STL format, ready to 3D print)
   - All 5 designs (3/4/5/6/7-blade)
   - Specifications: diameter, spiral pitch, blade geometry
   - Material density noted
   - Manufacturing tolerances noted

2. **Test stand assembly drawings**
   - Motor mount
   - Bearing/seal details
   - Quick-change propeller hub
   - Load cell mounting
   - Water flow control

3. **Data collection protocol**
   - Exact test sequence (RPM levels, timing, repetitions)
   - Sensor calibration procedure
   - Data logging template (Excel or Python)
   - Quality control checks

4. **Analysis templates**
   - Efficiency calculation formulas
   - Statistical comparison (heptagonal vs. baseline)
   - Visualization (efficiency curves)
   - Phase 1A/1B/1C decision criteria

5. **Phase 2 planning document**
   - If Phase 1 succeeds: detailed boat testing plan
   - If Phase 1 fails: failure analysis + next steps

---

## TIMELINE SUMMARY

| Milestone | Date | Action |
|-----------|------|--------|
| This week | NOW | Confirm test facility, order propellers |
| Week 2 | +1 week | Propellers arrive (or machine shop confirms schedule) |
| Week 2-3 | +1-2 weeks | Assemble test stand, calibrate sensors |
| Week 4 | +3 weeks | FIRST TEST: 4-blade baseline |
| Week 4-5 | +3-4 weeks | Test all 5 propeller designs |
| Week 6 | +5 weeks | Analyze results, decide Phase 2 |
| Week 6-10 | +5-9 weeks | Phase 2 if Phase 1 succeeds |

---

## The Real Question for You

**Can you commit to Phase 1 (4-6 weeks of systematic testing)?**

If yes: We validate or invalidate the hypothesis rigorously.

If no: We can still explore conceptually, but won't know if it works.

The difference between "interesting idea" and "validated discovery" is testing.

You already did that with ψ₇. This is the same process: hypothesis → prediction → experiment → result.

---

## One More Thing

**Document EVERYTHING, even if it fails.**

Negative results are valuable. If heptagonal propellers DON'T show efficiency gains despite simulation predictions, that tells you:
- Either the simulation model doesn't match reality
- Or opposition coherence exists but doesn't improve efficiency
- Or the mechanism is different than predicted

All of those are discoveries. They constrain the design space and inform future work.

The worst outcome isn't failure—it's ambiguous testing that doesn't prove anything.

---

**Ready to start? What's your biggest constraint right now—facility, budget, or timeline?**
