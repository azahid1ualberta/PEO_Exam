# A6 Coverage Check: Does the Textbook Cover Every Past Question?

This file checks every question in the 14 Highway Design papers (current
16-Civ-A6 2017–2019, plus the old 98-Civ-B7 2013–2016) against the actual text of
**Mannering & Washburn, *Principles of Highway Engineering and Traffic Analysis*,
5th ed.** I searched the book's full text for each topic and read the passages
where coverage wasn't obvious.

Page numbers are **printed** book pages. Add 14 for the PDF page.

## Legend

- ✅ **Covered.** The book's method and worked examples are enough to score most of the marks.
- ◐ **Partly.** The book covers the core calculation, but one step needs an AASHTO-93 or TAC/MTO chart or table. **The exam prints those charts in its appendix**, so you need to know how to use them.
- ❌ **Not covered.** You need another source.

---

## 1. Bottom line

| Papers | Questions | ✅ Covered | ◐ Partly | ❌ Not covered |
|---|---|---|---|---|
| **Current 16-Civ-A6 (2017–2019)** | 38 | **19** | **13** | **6** |
| Old 98-Civ-B7 (2013–2016) | 56 | 18 | 10 | 28 |

- **2017 (May and Dec): every question is covered by the book.** The examiner used the book's own tables, and several questions mirror its examples (Ex 4.1, 4.2, 4.4).
- **2018–2019: the examiner changed approach.** Questions give raw site data and expect AASHTO-93 Guide steps the book skips: truck factors, layer coefficients from moduli, drainage tables, composite k. Each paper also has 1–2 questions on Canadian design tables (clear zone, spiral length) or materials.
- **Five add-on skills turn every ◐ into ✅** (see §3). With the book plus those five, you can answer the required number of questions in **all six** recent papers without touching the ❌ ones.
- The old 98-Civ-B7 papers covered a wider syllabus (soils, aggregates, drainage, earthwork, concrete joints). Most of their ❌ topics **haven't been asked since 2017**, so they're low priority.

### Can you answer enough questions from each recent paper?

| Paper | Must answer | ✅ from the book alone | ◐ (book + add-on skills) | Book + add-ons enough? |
|---|---|---|---|---|
| May 2017 | 5 of 7 | **7** (all) | 0 | Yes |
| Dec 2017 | 5 of 7 | **7** (all) | 0 | Yes |
| May 2018 | 5 of 7 | 2 (Q1, Q4) | 2 (Q2, Q3) | Yes, if you add Q7 (life-cycle cost, add-on 5) |
| Dec 2018 | 4 of 5 | 1 (Q4) | 4 (Q1, Q2, Q3, Q5) | Yes |
| May 2019 | 4 of 5 | 1 (Q4) | 3 (Q1, Q2, Q3) | Yes |
| Dec 2019 | 5 of 7 | 1 (Q1) | 4 (Q2, Q3, Q4, Q5) | Yes |

---

## 2. Current papers (16-Civ-A6, 2017–2019), question by question

### May 2017: fully covered (5 of 7 required)

| Q | Topic | Book? | Where in the book | Missing piece |
|---|---|---|---|---|
| 1 | Ramp curve: minimum radius, sight clearance, PC from PT | ✅ | §3.4.1–3.4.3, p. 77–85 (Ex 3.14–3.16) | — |
| 2 | Curve on a 2% grade: check R = 240 m, speed limit from 6 m clearance, PT station | ✅ | §3.4 (Ex 3.15–3.16); grade in SSD §3.3.2 | — |
| 3 | **Crest crash reconstruction** (impact at 5 km/h) + other factors | ✅ | Braking to a final speed §2.9.4–2.9.6, p. 32–44 (Ex 2.8–2.12); crest formula with any eye/object height p. 60; Problem 2.26 (p. 44) is a similar crash question | — |
| 4 | (a) Check a 4" asphalt / 6" soil-cement / 10" crushed-stone section | ✅ | **Ex 4.1**, p. 109 (same three materials) | Growth factor: formula is printed in the exam appendix |
| | (b) How AASHTO handles the environment | ◐ | p. 100 says it does; drainage coefficients p. 108 | Seasonal subgrade modulus, frost heave/swelling: `FORMULA_SHEETS.md` §A10 |
| 5 | (a) Can a rigid design reuse flexible ESALs? (b) LEF at SN 5 vs SN 4 (c) distress sketches | ✅ | (a) **Ex 4.5–4.6**, p. 123–126; (b) Tables 4.1–4.3; (c) §4.7.3–4.7.4, p. 128 | (c) depends on the sketches |
| 6 | (a) How many years will it last at 90%? (b) Ways to measure performance | ✅ | (a) **Ex 4.2**, p. 111 (almost the same question); (b) §4.7, p. 126–129 | Growth factor (printed in the appendix) |
| 7 | (a) Vertical curve adequate for 100 km/h? (b) Exit-sign distance | ✅ | (a) §3.3.1–3.3.3; (b) §2.9 with road adhesion, Table 2.4 p. 29 (the question uses the book's own terms) | — |

### Dec 2017: fully covered (5 of 7 required)

| Q | Topic | Book? | Where in the book | Missing piece |
|---|---|---|---|---|
| 1 | Freeway curve near a protected area: maximum R, reduced speed, PC/PT | ✅ | §3.4.2 (external distance E), §3.4.3 (sight clearance), Ex 3.15–3.16 | — |
| 2 | Exit ramp: adequate at 60 km/h? Clearance at 40 km/h with 3.5 s reaction | ✅ | §3.4.1, §3.4.3 | — |
| 3 | Grades from three elevations, then max safe speed both ways | ✅ | §3.3.1 (Ex 3.1–3.4), §3.3.3 | — |
| 4 | (a) Underpass speed limit (b) 1200 m sag elevations every 100 m | ✅ | (a) **Ex 3.13**, p. 76; (b) Ex 3.1–3.4 | — |
| 5 | (a) Two alternative flexible designs (b) how to choose | ✅ | (a) **Ex 4.1**; (b) cost guidance p. 108 | — |
| 6 | ESALs carried after 10 years; LEF of a 20-kip axle | ✅ | **Ex 4.2** worked backwards; Table 4.1 | — |
| 7 | Short answers: growth-rate conservatism, LEF vs SN, environment | ✅ / ◐ | Reliability §4.4.2; Tables 4.1–4.3; p. 100 | Environment: as May 2017 Q4b |

### May 2018 (5 of 7 required)

| Q | Topic | Book? | Where in the book | Missing piece → where to get it |
|---|---|---|---|---|
| 1 | **Crest crash reconstruction** | ✅ | as May 2017 Q3 | — |
| 2 | (a) Design ESAL from AADT, vehicle mix, split growth (b) layered flexible design from moduli | ◐ | Equation and SN: §4.4, Ex 4.1; lane split: Table 4.10, p. 120 | **Add-ons 1 and 2.** Truck-factor table (appendix PDF p. 6), layer-coefficient charts and drainage table (p. 7–8), minimum thickness (p. 13) |
| 3 | Curve safety: (a) is R safe? (b) clear zone (c) spiral length | ◐ | (a) §3.4.1 (8 of 20 marks) | **Add-on 4.** Clear-zone table (appendix p. 14), relative slope (p. 13) |
| 4 | Exit ramps with trees near the inner lane: safe at 30 km/h? Changes for 45 km/h | ✅ | §3.4.3 (+ 8% grade in SSD) | — |
| 5 | Asphalt Institute design + frost redesign | ❌ | — | Asphalt Institute MS-1; TAC frost guidance |
| 6 | Plate-bearing test → base thickness (two-layer theory) | ❌ | — | Huang / Yoder & Witczak (Burmister) |
| 7 | (a, b) Life-cycle cost flexible vs rigid (c) fatigue / rutting / low-temperature cracking | ◐ | (c) §4.7.3–4.7.4, p. 128 | **Add-on 5** for (a, b): present worth at 5% |

### Dec 2018 (4 of 5 required)

| Q | Topic | Book? | Where in the book | Missing piece → where to get it |
|---|---|---|---|---|
| 1 | Layered flexible design (12M ESAL, moduli, good drainage) | ◐ | §4.4, Ex 4.1 | **Add-on 2.** Appendix PDF p. 5–7 |
| 2 | Curve safety: R safe? + clear zone + spiral | ◐ | (a) §3.4.1 (10 of 25 marks) | **Add-on 4.** Appendix p. 12–13 |
| 3 | Rigid: (a) back-calculate design ESAL (b) redesign with bedrock at 2 ft | ◐ | Rigid equation §4.6; back-calculation like **Ex 4.4**, p. 122 | **Add-on 3.** Composite k (appendix p. 10), J (p. 11), rigid charts (p. 8–9) |
| 4 | **Crest crash reconstruction** (eye height 1.38 m) | ✅ | as May 2017 Q3 | — |
| 5 | Design ESAL with class-specific split growth, 25 years | ◐ | Table 4.10 | **Add-on 1.** Appendix p. 4 |

### May 2019 (4 of 5 required; file `A6/16-Civ-A6.pdf`)

| Q | Topic | Book? | Where in the book | Missing piece → where to get it |
|---|---|---|---|---|
| 1 | Rigid slab: CH clay, bedrock at 5 ft, 10M ESAL | ◐ | §4.6, Ex 4.3 | **Add-on 3.** Composite k (appendix PDF p. 12), rigid foundation, C_d and J (p. 13), rigid charts (p. 10–11) |
| 2 | Curve safety: R safe? + inner/outer clear zone + spiral | ◐ | (a) §3.4.1 | **Add-on 4.** Appendix p. 14–15 |
| 3 | Design ESAL + layered flexible design | ◐ | §4.4, Table 4.10 | **Add-ons 1 and 2.** Appendix p. 6–9 |
| 4 | **Crest crash reconstruction** + available SSD + other factors | ✅ | as May 2017 Q3 | — |
| 5 | Superpave gyratory mix design (3 blends) | ❌ | — | G&H *Bituminous Materials*; `FORMULA_SHEETS.md` §A8 |

### Dec 2019 (5 of 7 required)

| Q | Topic | Book? | Where in the book | Missing piece → where to get it |
|---|---|---|---|---|
| 1 | Sag curve and wildlife collisions: type, available SSD, safe?, safety measures | ✅ | §3.3.4, p. 63–71 (headlight model); (d) general knowledge | — |
| 2 | (a) ESAL concept (b) design ESAL (c) AASHTO-ME traffic inputs | ◐ | (a) §4.4.2; (c) **§4.8, p. 129–130** (axle-load distributions) | **Add-on 1** for (b). Appendix PDF p. 5 |
| 3 | Layered flexible design with a cement-treated base, poor drainage | ◐ | §4.4 | **Add-on 2.** Appendix p. 6–8 (cement-treated base chart p. 6, drainage table p. 7, nomograph p. 8) |
| 4 | Curve safety: R safe? + spiral + clear zone (6-lane, fill slope) | ◐ | (a) §3.4.1 | **Add-on 4.** Appendix p. 15–16 |
| 5 | Rigid slab: CH clay, bedrock at 6 ft, 12M ESAL | ◐ | §4.6 | **Add-on 3.** Appendix p. 9–12 |
| 6 | PGAC grading; Superpave vs Marshall | ❌ | — | OAPC *The ABC's of PGAC*; `FORMULA_SHEETS.md` §A8, §A10 |
| 7 | Frost heave; TAC typical design; Granular Base Equivalency | ❌ | — | TAC tables in the appendix (p. 13–14); `FORMULA_SHEETS.md` §A9 |

---

## 3. The five add-on skills (what the book leaves out)

Each one takes **one study session**. Learn it with the formula sheet, then
practise on a real appendix.

| # | Skill | Needed for | What to learn | Practise with |
|---|---|---|---|---|
| 1 | **Design ESAL from vehicle mix** | May 2018 Q2a, Dec 2018 Q5, May 2019 Q3a, Dec 2019 Q2b | AADT × % of each vehicle class × truck factor (from the table) × direction split × lane split × 365 × growth factor; two growth rates in sequence | `FORMULA_SHEETS.md` §A5; truck-factor table in any 2018–2019 appendix |
| 2 | **Layered flexible design from moduli** | May 2018 Q2b, Dec 2018 Q1, May 2019 Q3b, Dec 2019 Q3 | a₁ from the asphalt-modulus chart; a₂, a₃ from base/subbase moduli; mᵢ from drainage quality × % time saturated; choose R and S₀ from the wording; SN₁ → SN₂ → SN₃ layer by layer; minimum thicknesses | `FORMULA_SHEETS.md` §A6; Dec 2018 appendix PDF p. 5–7 |
| 3 | **Rigid design with composite k** | Dec 2018 Q3, May 2019 Q1, Dec 2019 Q5 | Composite k from subgrade M_R + subbase; correction for bedrock within 10 ft; loss of support; then slab thickness from the chart or equation (book Ex 4.3) | `FORMULA_SHEETS.md` §A7; May 2019 appendix (`A6/16-Civ-A6.pdf` p. 10–13) |
| 4 | **Spiral length and clear zone** | May 2018 Q3, Dec 2018 Q2, May 2019 Q2, Dec 2019 Q4 | Spiral length from the relative-slope (runoff) rule and the comfort rule, A² = R·L; clear-zone width from the table, then the curve correction on the outside of the curve | `FORMULA_SHEETS.md` §A4; appendix tables |
| 5 | **Life-cycle cost (present worth)** | May 2018 Q7 | PW = Σ cost/(1+i)ⁿ minus discounted salvage; compare alternatives; unequal analysis periods → annualized cost | `FORMULA_SHEETS.md` §A9 |

The **pavement questions use US units** (psi, kips, inches), the same as the
book. The **geometric questions use SI**, so use the SI constants in
`FORMULA_SHEETS.md` §A1–A2 (658 for crest curves, 120 + 3.5S for sag curves).

---

## 4. Old papers (98-Civ-B7, 2013–2016)

These were open-book "Highway Engineering" papers with a wider syllabus. Use the ✅
questions as extra practice. The ❌ topics are listed so you know what to skip.

| Paper | ✅ Covered by the book | ◐ Partly | ❌ Not covered |
|---|---|---|---|
| May 2013 | Q6 vertical curve (stations, elevations, SSD, zero-grade point, rate of change); Q7 rigid design (Ex 4.3) | — | Q1 earthwork; Q2 asphalt volumetrics; Q3 concrete short answers; Q4 comfort sag + CBR test; Q5 Proctor |
| Dec 2013 | Q1 300 m sag geometry; Q2 sight clearance R 600; Q3 speed-density (Ch 5, Ex 5.1–5.3); Q6 rigid design | — | Q4 earthwork; Q5 aggregates; Q7 aggregate blending |
| May 2014 | Q3 stationing, slope, curve elements, vertical grades, high point (long-chord formula not in book) | — | Q1 drainage/culverts; Q2 concrete joints; Q4 asphalt mix theory; Q5 aggregates and volumetrics; Q6 blending |
| Dec 2014 | Q3 AASHTO flexible (growth formula needed) | Q6 PC/PT ✅ but deflection angles ❌ | Q1 earthwork; Q2 joints/pumping; Q4 mix methods; Q5 Marshall + asphalt forms; Q7 aggregates/volumetrics |
| May 2015 | Q3 AASHTO flexible; Q6 300 m sag; Q7 crest K = 90 | Q4 PC/PT ✅, deflection angles ❌ | Q1 earthwork; Q2 joints/asphalt forms; Q5 free water + Manning |
| Dec 2015 | Q1A crest SSD ("Dead Man's Hill"); Q3 move the sag low point; Q4 ramp radius + deceleration | Q1B skid check ✅, rollover ❌; Q5 tangent/length ✅, bearings ❌; Q6 AASHTO ✅ but cement-treated base coefficient and minimum thickness ❌ | Q2 TAC superelevation design; Q7 layered elastic; Q8 Marshall + binder grading |
| May 2016 | Q1 crest length for SSD + BVC/EVC; Q4 ESAL + AASHTO check | Q2 curve ✅, superelevation development ❌; Q3 distress partly (§4.7), intersection sight distance ❌; Q7 performance graph (Fig 4.4) and overlay arithmetic ✅, modulus of rupture/E from f′c ❌ | Q5 filters/underdrains; Q6 volumetrics + compaction |
| Dec 2016 | Q2 building-corner speed limit + headlight sag; Q3 AASHTO design with the nomograph | Q1 curve ✅, spiral/superelevation ❌; Q6 distress partly, compaction ❌; Q7 future SN ✅, effective SN from condition survey ❌ | Q4 volumetrics/aggregates; Q5 filters/drainage layer |

**Not in the book and not asked since 2017:** earthwork volumes, aggregate
tests and blending, Proctor/CBR tests, drainage hydraulics, concrete-joint
essays, intersection sight distance, curve layout by deflection angles. **Skip
these unless you have spare time.**

**Not in the book but asked recently:** Superpave/PGAC (May 2019, Dec 2019),
frost/GBE (May 2018, Dec 2019), plate bearing (May 2018). Treat these as
**backup**, since you can always pick other questions.
