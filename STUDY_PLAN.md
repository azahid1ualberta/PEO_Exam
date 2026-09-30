# PEO Exam Prep: A6 and B7 in 45 Days

This plan comes from an analysis of all 28 unique past papers in this repo
(2013–2019) and a chapter-by-chapter check of *Principles of Highway Engineering
and Traffic Analysis* (Mannering & Washburn, 5th ed.). For formulas to memorize
or put on an aid sheet, see [`FORMULA_SHEETS.md`](FORMULA_SHEETS.md). For every
past question grouped by type, with repeat counts and what to read, see
[`QUESTION_BANK.md`](QUESTION_BANK.md).

---

## 1. First, a problem with how the papers are sorted

**The course codes swapped between the 1998 and 2016 syllabi.** Each folder mixes
two different courses:

| File in repo | Code on the paper | Actual course | Use it to study for |
|---|---|---|---|
| `A6/AE-*-2013…2016-98-Civ-A6.pdf` (8 papers) | 98-Civ-**A6** | Transportation Planning & Engineering | **B7** (current) |
| `A6/AE-*-2017…2019-16-Civ-A6.pdf`, `A6/16-Civ-A6.pdf` (6 papers) | 16-Civ-**A6** | Highway Design, Construction & Maintenance | **A6** (current) |
| `B7/AE-*-2013…2016-98-Civ-B7.pdf` (8 papers) | 98-Civ-**B7** | Highway Engineering | **A6** (current) |
| `B7/AE-*-2017…2019-16-Civ-B7.pdf` (6 papers) | 16-Civ-**B7** | Transportation Planning & Engineering | **B7** (current) |

Other notes on the files:
- `B7/1. New Pattern Questions/` is a byte-identical copy of the 2017–2019 B7 papers.
- `A6/AE-May-2019-16-Civ-A6.pdf` is password-protected, but `A6/16-Civ-A6.pdf`
  holds the same May 2019 paper and its appendix, so nothing is missing.

**Action for Day 1:** check the course code **and title** on your PEO exam notice.
The rest of this plan assumes the current (2016) syllabus:
- **A6 = Highway Design, Construction & Maintenance**
- **B7 = Transportation Planning & Engineering**

If your notice says otherwise, swap the two halves of this plan.

### Exam formats, as printed on the past papers

| | A6 Highway Design (16-Civ, 2017–19) | B7 Transportation Planning (16-Civ, 2017–19) |
|---|---|---|
| Duration | 3 h | 3 h |
| Questions | 5 of 7 (May 2017, Dec 2017, May 2018, Dec 2019) or 4 of 5 (Dec 2018, May 2019) | 5 of 7, every paper |
| Book policy | Closed book. Formula and table appendix provided. Dec 2017 also allowed one hand-written 8.5×11 aid sheet (both sides). | Closed book, **one two-sided aid sheet** |
| Calculator | Casio or Sharp approved model | Casio or Sharp approved model |
| Marking | Only the first N answers in the booklet are marked | Only the first 5 answers in the booklet are marked |

The old 98-Civ-B7 Highway Engineering exams were **open book**. The current A6 is
**closed book**, so formulas have to be memorized or put on the aid sheet if you
are allowed one. Your exam notice has the final word on format (paper or online,
aid sheet, number of questions). Check it.

---

## 2. B7 Transportation Planning: the most predictable exam you'll write

All **14** papers (8 × 98-Civ-A6 + 6 × 16-Civ-B7) use **the same 7-question
template**, probably from the same examiner. Many questions are repeated almost
word for word.

| # | Question type (appears in 14/14 papers) | Marks | In your textbook? | Supplement needed |
|---|---|---|---|---|
| Q1 | Theory: land use and transport, TDM, trip-production factors, ITS/CAV, supply- vs demand-side | 20 | Partly: Ch 1, §8.1–8.3, 8.7–8.9 | Prepare a bank of written answers |
| Q2 | **D/D/1 queuing**: incident, toll booth, parking lot, 2-cycle signal, time-varying arrivals | 20 | **Yes**: §5.5.2 (Ex 5.7–5.10, 5.15), §7.5.1 (Ex 7.10–7.12) | No |
| Q3 | **Trip generation**: cross-classification rates, plus a linear regression, plus compare assumptions | 20 | Regression yes (§8.4, Ex 8.1–8.3). Cross-classification no. | Short read |
| Q4 | **Greenshields + shock waves**: stopped queue (stall, rail gate, red light) or moving bottleneck (slow truck) | 20 | Greenshields yes (§5.2–5.3, Ex 5.2–5.3). **Shock waves: not in book.** | **Yes** |
| Q5 | **Gravity model** trip distribution: 2–5 zones, friction factor 1/t, 1/t², exp(−βd), then a future year | 20 | **No** (the book uses logit destination choice) | **Yes** |
| Q6/Q7 | **User equilibrium** route choice: 2 routes, then add a 3rd; sometimes system optimum | 20 | **Yes**: §8.6 (Ex 8.10–8.16) | Braess paradox (a few lines) |
| Q7/Q6 | **Multinomial logit** mode choice, then a policy change, then **IIA** | 20 | Logit yes (§8.5, Ex 8.5–8.6). IIA / nested logit no. | Short read |

### Repeats in the B7 papers (high-value practice)

- **Trip generation, persons × vehicles table (rates 2.6 … 17.2):** Dec 2016 Q3 = Dec 2017 Q3 = Dec 2019 Q3
- **Gravity model, P = 450/550, A = 700/300, d = 10/5 km:** Dec 2015 Q5 = May 2018 Q5 = May 2019 Q5
- **Gravity model, P = 75/75, A = 50/100, t = 5/2:** Dec 2016 Q5 = Dec 2019 Q5
- **UE with t₁ = 22 + 2V₁/225 and t₂ = 12 + V₂/100:** May 2013 Q6, Dec 2016 Q6, Dec 2019 Q6 (adds system optimum)
- **4-mode logit (auto/bus/rail/bike):** May 2017 Q6 = Dec 2017 Q6 = Dec 2018 Q7
- **Auto/bus logit, then light rail added, then IIA:** Dec 2015 Q7 = May 2019 Q7
- **Auto/bus/LRT logit (1.1 − 0.05TT − 0.25TC):** Dec 2016 Q7 = Dec 2019 Q7
- **Freeway incident queue (12/18/6 veh/min):** May 2015 Q2 = May 2019 Q2
- **Shock wave at a signal (45 km/h, 20 veh/km, 30 s red):** May 2015 Q4 = May 2019 Q4
- **Shock wave at a rail crossing:** Dec 2013 Q4, May 2016 Q4, May 2018 Q4
- **Shock wave behind a slow truck or tractor:** May 2014, Dec 2015, Dec 2016, Dec 2017, Dec 2018, Dec 2019 (Q4)
- **Q1 themes that keep coming back:**
  - Low-density suburbs and mode choice (May 2015, May 2016, May 2018, May 2019)
  - Trip-production factors at zonal, household and person level (May 2015, Dec 2016, Dec 2017, Dec 2019)
  - TDM strategies to raise vehicle occupancy (Dec 2013, May 2016, May 2018, Dec 2019)
  - Residential development and transit (Dec 2015, Dec 2019)

### B7 strategy

1. **Master Q2–Q7 until they're mechanical.** That gives you six computational
   questions to pick five from. Each one has a single right answer and follows a
   fixed recipe.
2. Q1 is your spare, and it's predictable too. Write 10–12 model answers in bullet
   form in advance (see Day 10).
3. Every Q3, Q5 and Q7 has a "(c) compare / explain / IIA" part worth 4–8 marks.
   Memorize a short standard answer for each (see `FORMULA_SHEETS.md`).

---

## 3. A6 Highway Design: broader, but the core repeats

Topic frequency in the **six current-syllabus papers** (16-Civ-A6, May 2017 to Dec 2019):

| Priority | Topic | Papers | Where (A6 papers) | Textbook coverage |
|---|---|---|---|---|
| **Core** | **Vertical curves + SSD** (crest "accident reconstruction", sag headlight, underpass, curve elevations) | **6/6** | May17 Q3, Q7a · Dec17 Q3, Q4 · May18 Q1 · Dec18 Q4 · May19 Q4 · Dec19 Q1 | **Excellent**: §2.9 (Ex 2.8–2.12), §3.3 (Ex 3.1–3.13) |
| **Core** | **AASHTO-93 flexible design** (check a design, remaining life, layered design from moduli) | **6/6** | May17 Q4, Q6 · Dec17 Q5, Q6 · May18 Q2b · Dec18 Q1 · May19 Q3b · Dec19 Q3 | Good: §4.4 (Ex 4.1–4.2). Layer coefficients from moduli and the layered procedure need the supplement. |
| **Core** | **Design ESAL** (vehicle mix × truck factors × split growth rates, or LEF tables) | **6/6** (standalone in 4) | May18 Q2a · Dec18 Q5 · May19 Q3a · Dec19 Q2 (+ LEF in 2017) | LEF tables yes (§4.4.2). Truck-factor method: supplement. |
| **Core** | **Horizontal-curve safety + clear zone + spiral length** (MTO/TAC-style) | **4/6**, every paper since May 2018 | May18 Q3 · Dec18 Q2 · May19 Q2 · Dec19 Q4 | Radius yes (§3.4). Spirals and clear zones: supplement (tables given in exam). |
| **Core** | **AASHTO-93 rigid (JPCP)**: composite k, shallow bedrock, slab thickness | **3/6**, every paper since Dec 2018 | Dec18 Q3 · May19 Q1 · Dec19 Q5 | Equation yes (§4.6, Ex 4.3–4.6). Composite k and rigid foundation: supplement. |
| High | **Horizontal curves**: R_min, sight clearance Ms, speed limit, PC/PT stationing (often ramps) | 3/6 | May17 Q1, Q2 · Dec17 Q1, Q2 · May18 Q4 | **Excellent**: §3.4 (Ex 3.14–3.16) |
| High | Short-answer theory: ESAL concept, LEF vs SN, environment in AASHTO, rigid vs flexible ESALs, AASHTO-ME, performance measures, distresses | 4/6 | May17 Q5 · Dec17 Q7 · May18 Q7c · Dec19 Q2a, Q2c | Partly: §4.7–4.8 |
| Backup | Asphalt materials: Superpave volumetrics, PGAC grading, Marshall vs Superpave | 2/6 | May19 Q5 · Dec19 Q6 | No: supplement |
| Backup | Frost protection, TAC typical sections, Granular Base Equivalency, Asphalt Institute method | 2/6 | May18 Q5 · Dec19 Q7 | No: supplement |
| Low | Life-cycle cost analysis (present worth), plate-bearing/Burmister, sign placement | 1/6 each | May18 Q7 · May18 Q6 · May17 Q7b | No |

**What the core topics buy you:** vertical/SSD, horizontal/spiral/clear zone,
ESAL, flexible and rigid AASHTO would have given you enough questions to answer
in **5 of the 6 recent papers**, and 4 of the 5 needed in the sixth (May 2018).
Build on these first.

The older **98-Civ-B7 Highway Engineering** papers (2013–2016) are good *extra
practice* for vertical and horizontal curves, AASHTO flexible, overlays, HMA
volumetrics and compaction. They also cover earthwork, drainage, aggregate
blending and concrete joints, which haven't appeared since 2017. Treat those
as low priority.

**Good news about your textbook:** the 2017 A6 appendices use Mannering &
Washburn's notation (R_v, M_s, SSD) and tables with the book's exact titles:
"Axle-Load Equivalency Factors for Flexible Pavements…", "Cumulative Percent
Probabilities of Reliability…" and the structural-layer coefficients. The
numbers are off by one from your 5th edition (the exam's "Table 4.2" is your
Table 4.1), so the examiner probably used an earlier metric edition of the
same book. Chapters 2.9, 3 and 4 are directly on target.

**Watch the units:** the 5th edition is in **US customary units only**, but
every PEO paper is in **SI**. Download the free **Metric Units Supplement** from
the book's Wiley site (www.wiley.com/college/mannering), or convert the
constants yourself: crest 2158 ft → **658 m**; sag 400 + 3.5S ft →
**120 + 3.5S m**; a = 11.2 ft/s² → **3.4 m/s²**; eye 3.5 ft → **1.08 m**;
object 2 ft → **0.60 m**. `FORMULA_SHEETS.md` has the SI versions.

---

## 4. What to read beyond your textbook (only these sections)

With 45 days you can't read another book cover to cover. Read **only** the
sections for the gaps above. Garber & Hoel, *Traffic and Highway Engineering*
(any recent SI edition), covers almost every gap in one place:

| Gap | Course | Garber & Hoel topic (chapter numbers vary by edition) |
|---|---|---|
| Shock waves (stopped queue and moving bottleneck) | B7 | "Fundamental principles of traffic flow", shock-wave section |
| Cross-classification trip generation, gravity model, IIA / nested logit | B7 | "Forecasting travel demand" |
| AASHTO-93 layered flexible design: a₁/a₂/a₃ from moduli, mᵢ, minimum thicknesses | A6 | "Design of flexible pavements" |
| AASHTO-93 rigid: composite k, rigid foundation, loss of support, J, C_d | A6 | "Design of rigid pavements" |
| ESAL from vehicle mix and truck factors, growth factors | A6 | Flexible pavements, traffic-load section |
| Superpave volumetrics, PG grading, Marshall | A6 | "Bituminous materials" |

Also useful, and short:
- **OAPC, "The ABC's of PGAC"** (Ontario Asphalt Pavement Council). The Dec 2019 A6 paper quotes it directly.
- **TAC Geometric Design Guide for Canadian Roads**: only the superelevation/spiral tables and clear-zone tables, to learn how to *use* them. The exam supplies the tables.
- **AASHTO 1993 Guide, Part II, Ch. 2–3**: the charts the exam appendices reproduce (layer coefficients, mᵢ, composite k, rigid nomograph). Practice reading them.

---

## 5. The 45-day plan

**Assumptions:** Day 1 = Oct 1, Day 45 = Nov 14. Budget about 3 h on weekdays
and 6 h on weekend days. If your two exams fall on different dates, run the
mock papers for the earlier exam first.

**Keep two sets of papers apart:**
- **Practice papers** (use while learning):
  - **B7:** the eight 2013–2016 98-Civ-A6 papers, plus May 2017 and Dec 2017 16-Civ-B7.
  - **A6:** May 2017, Dec 2018, May 2019, plus all 98-Civ-B7 papers.
- **Mock papers** (don't look at them until mock day):
  - **B7:** May 2018, Dec 2018, May 2019, Dec 2019.
  - **A6:** Dec 2017, May 2018, Dec 2019.

Keep an **error log** (notebook or spreadsheet) with one line per mistake: the
question, what went wrong, and the correct method. Re-read it every Sunday.

### Phase 1: Set up and baseline (Days 1–2)

| Day | Tasks |
|---|---|
| 1 | Confirm course codes, titles, dates and aid-sheet rules on your exam notice. Re-sort the papers using the table in §1. Get the Metric Units Supplement and the Garber & Hoel sections. Learn your approved calculator's equation solver if it has one (the Casio fx-991 series has SOLVE), because you'll need it for the AASHTO equations. **Cold attempt** of B7 Dec 2015 (untimed) to find your baseline. |
| 2 | **Cold attempt** of A6 May 2017 (untimed). Start the error log. Skim Mannering Ch 3 and Ch 4 section headings so you know where things are. |

### Phase 2: Learn the B7 templates (Days 3–10)

Each day: read the section, do the textbook examples, then solve **three or more
past versions** of that question type from the practice set.

| Day | Template | Read | Practice (practice-set papers only) |
|---|---|---|---|
| 3 | **Q2 D/D/1 queuing** | Mannering §5.5.2 (Ex 5.7–5.10, 5.15), §7.5.1 (Ex 7.10–7.12) | May13 Q2, May14 Q2, Dec14 Q2, May15 Q2, Dec16 Q2, May17 Q2. Signals: Dec13 Q2, May16 Q2. Time-varying: Dec17 Q2 |
| 4 | **Q4 shock waves: stopped queue** | Mannering §5.2–5.3 (Ex 5.2–5.3) + G&H shock waves | May13 Q4, Dec13 Q4, Dec14 Q4, May15 Q4, May16 Q4, May17 Q4 |
| 5 | **Q4 shock waves: moving bottleneck** | G&H shock waves | May14 Q4, Dec15 Q4, Dec16 Q4, Dec17 Q4 |
| 6 | **Q3 trip generation** | Mannering §8.4 (Ex 8.1–8.3) + G&H cross-classification | May13 → Dec17 Q3 (pick five) |
| 7 | **Q5 gravity model** | G&H trip distribution | May13 Q5, Dec13 Q5 (5 zones), May15 Q5, Dec15 Q5, May17 Q5 (two friction factors), Dec17 Q5 (exp) |
| 8 | **UE route choice (+ SO)** | Mannering §8.6 (Ex 8.10–8.16) | May13 Q6, Dec14 Q6, Dec15 Q6, May16 Q6, Dec17 Q7 |
| 9 | **MNL mode choice + IIA** | Mannering §8.5 (Ex 8.5–8.6) + G&H IIA / nested logit | May13 Q7, May15 Q7 (binary → 3 modes), Dec15 Q7, May16 Q7, May17 Q6 |
| 10 | **Q1 theory bank** | Mannering Ch 1, §8.1–8.3, 8.7–8.9 | Write bullet-point model answers to every Q1 prompt in the practice set (about 12). Then do **Q2 + Q5 timed in 72 min**. |

### Phase 3: Learn A6 (Days 11–26)

Also do **one timed B7 question each day** (35 min), rotating through Q2–Q7, so B7 stays fresh.

| Day | Topic | Read | Practice |
|---|---|---|---|
| 11 | **SSD + accident reconstruction** (impact speed, grade, friction) | Mannering §2.9.4–2.9.6 (Ex 2.8–2.12), §3.3.2 | May17 Q3, Dec18 Q4, May19 Q4 |
| 12 | **Vertical-curve geometry** (elevations, high/low point, K) | §3.3.1 (Ex 3.1–3.4) | May17 Q7a. 98-B7: Dec13 Q1, May15 Q6 & Q7, Dec15 Q3 (catch basin), May13 Q6 |
| 13 | **Crest, sag, headlight, underpass, comfort** | §3.3.3–3.3.6 (Ex 3.5–3.13) | 98-B7: May16 Q1, Dec16 Q2b, May13 Q4a, Dec15 Q1A |
| 14 | **Horizontal curves** (R_min, Ms, speed limit, stationing) | §3.4 (Ex 3.14–3.16) | May17 Q1 & Q2. 98-B7: Dec13 Q2, Dec16 Q2a, Dec15 Q1B & Q4 |
| 15 | **Spiral, superelevation runoff, clear zone** | G&H or TAC tables | Dec18 Q2, May19 Q2. 98-B7: May16 Q2, Dec16 Q1 (superelevation development) |
| 16 | **Geometry consolidation** | §3.5 (Ex 3.17–3.18) | Timed: two geometric questions in 72 min. Redo anything in the error log. |
| 17 | **Design ESAL** (truck factors, split growth, lane and direction factors) | §4.4.2 + G&H traffic loading | Dec18 Q5, May19 Q3a. 98-B7: May16 Q4a–b |
| 18 | **AASHTO flexible: equation, chart, reliability** | §4.4 (Ex 4.1–4.2) | May17 Q4 & Q6. 98-B7: Dec14 Q3, May15 Q3. Solve SN with the equation **and** the chart. |
| 19 | **AASHTO flexible: layered design from moduli, mᵢ** | G&H flexible design | Dec18 Q1, May19 Q3b. 98-B7: Dec15 Q6, Dec16 Q3. Overlays: May16 Q7b, Dec16 Q7 |
| 20 | **AASHTO rigid: equation, S'c, E_c, k, J, C_d** | §4.6 (Ex 4.3–4.6) | 98-B7: May13 Q7, Dec13 Q6 |
| 21 | **Rigid: composite k, rigid foundation, loss of support** | G&H rigid design + AASHTO charts | Dec18 Q3, May19 Q1 |
| 22 | **HMA volumetrics** (Gsb, Gse, Gmm, Va, VMA, VFA, Pba) | G&H bituminous materials | 98-B7: May13 Q2, May14 Q5c, Dec14 Q7b, May16 Q6a, Dec16 Q4a, Dec15 Q8A |
| 23 | **Superpave gyratory + PGAC + Marshall vs Superpave** | G&H + "ABC's of PGAC" | May19 Q5. 98-B7: May14 Q4, Dec14 Q4a, Dec15 Q8B |
| 24 | **Frost, TAC typical sections, GBE, Asphalt Institute; compaction control** | G&H / TAC notes | 98-B7: May16 Q6b, Dec16 Q6a. Read the concepts behind May18 Q5 and Dec19 Q7 (**don't open those papers**, they're mocks) |
| 25 | **A6 theory bank**: distress mechanisms, environment in AASHTO, LEF vs SN, ESAL concept, AASHTO-ME, IRI and other measures, joints and pumping, LCCA | §4.7–4.8 + G&H | May17 Q5. 98-B7: May16 Q3b, Dec16 Q6b. Write bullet model answers. |
| 26 | **A6 Mock 1: Dec 2017** (5 of 7, 3 h, closed book, strict timing) | | Mark it harshly and log every error. |

### Phase 4: Mock exams and weak areas (Days 27–41)

| Day | Tasks |
|---|---|
| 27 | Review Mock 1. **Aid sheet draft v1** for B7 (and A6 if your notice allows one). |
| 28 | **B7 Mock 1: May 2018** (3 h) + review |
| 29 | A6 weak areas from the error log |
| 30 | **A6 Mock 2: May 2018** (3 h) + review |
| 31 | B7 weak areas + say your Q1 answers aloud or write them from memory |
| 32 | **B7 Mock 2: Dec 2018** + review |
| 33 | A6 weak areas: rigid and layered flexible (the longest questions, so time them) |
| 34 | Redo every error-log question without notes |
| 35 | **B7 Mock 3: May 2019** + review |
| 36 | A6: nomograph practice (flexible and rigid charts), then check each chart answer with the equation |
| 37 | **A6 Mock 3: Dec 2019** (final strict run) + review |
| 38 | **B7 Mock 4: Dec 2019** (final strict run) + review |
| 39 | **Aid sheet v2** (final). Formula recall drill: write both formula sheets from memory. |
| 40 | Mixed drill: one question of each B7 type, 30 min each |
| 41 | Mixed drill: one A6 core question of each type, 35 min each |

### Phase 5: Taper (Days 42–45)

| Day | Tasks |
|---|---|
| 42 | Redo the ten hardest error-log items |
| 43 | Light review of the formula sheets and Q1 / A6 theory bullets |
| 44 | Logistics: ID, approved calculator (fresh battery), ruler for nomographs, pencils, final aid sheet. Early night. |
| 45 | Rest and a light skim only. No new material. |

**If you fall behind,** drop in this order: plate bearing / LCCA / Asphalt
Institute, then earthwork, drainage and aggregate blending (old-syllabus only),
then frost/GBE, then Superpave. **Never drop** B7 Q2–Q7 or the five A6 core topics.

---

## 6. In the exam room

1. **First 10 minutes:** read every question and pick your 5 (or 4). Choose ones
   that are all-calculation over essay-heavy ones where you can.
2. **Budget time:** 3 h ÷ 5 ≈ **32 min per question** plus 10 min at the end
   to check (≈ 40 min each for a 4-of-5 paper).
3. **Only the first N answers in the booklet are marked.** Never start an
   extra question. If you abandon one, cross it out clearly.
4. **State assumptions.** Every paper invites them. For example: perception
   time 2.5 s, drainage quality from time-to-drain, reliability from road class.
   Write them down and justify them in one line.
5. **Parts (a) and (b) often use the same data.** If (a) goes wrong, carry your
   number forward and finish (b) and (c). Method marks are generous.
6. **Nomographs:** draw clean construction lines, write the value you read off,
   and hand the chart in if the paper says to. Check the result with the
   equation if time allows.
7. **Theory parts** ("compare", "explain IIA", "other factors"): use
   bullet points under a one-line heading. The papers say clarity and
   organization are marked.
8. **Sketch every D/D/1 queue diagram and shock-wave q–k diagram.** Those
   sketches are usually worth 8–10 marks on their own.

---

## 7. Your first three actions

1. Check the exam notice (course code, title, date, aid sheet). §1 explains why this matters.
2. Get the Metric Units Supplement and the Garber & Hoel sections from §4.
3. Start Day 1. Tomorrow, begin learning the D/D/1 template.
