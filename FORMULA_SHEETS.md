# Formula Sheets and Standard Answers

Companion to [`STUDY_PLAN.md`](STUDY_PLAN.md). Everything is in **SI**, the units
the PEO papers use. Your textbook uses US units.

- **B7** allows one two-sided aid sheet. Build it from §B.
- **A6** has been closed book, with a formula appendix. Memorize §A unless your
  exam notice allows an aid sheet (Dec 2017 did).

Write the aid sheet **by hand**, from memory, several times. Writing it out is
itself good revision.

---

## B. B7 Transportation Planning & Engineering

### B1. Traffic stream (Greenshields): Q4 part (a)

- q = k·u
- u = u_f (1 − k/k_j)
- q = u_f·k − (u_f/k_j)·k²
- **Capacity:** q_max = u_f·k_j/4, at k_m = k_j/2 and u_m = u_f/2
- Given capacity and free-flow speed: **k_j = 4·q_max/u_f**
- Given a normal speed u₁: k₁ = k_j (1 − u₁/u_f), and q₁ = k₁·u₁

### B2. Shock waves: Q4 (b)–(d)

**Wave speed between states A and B:**
w_AB = (q_B − q_A)/(k_B − k_A). A negative value means the wave moves upstream.
Always sketch the q–k parabola: each wave speed is the slope of the chord
between two states.

**Stopped queue** (stalled car, rail gate, red light) blocking for time t_b.
The states are: 1 = upstream (q₁, k₁), J = jam (0, k_j), C = capacity (q_m, k_m).

1. Queue rear moves at w_1J = −q₁/(k_j − k₁).
2. Queue length at release: L = |w_1J|·t_b. Vehicles in the queue = k_j·L.
3. After release, the start-up wave moves at w_JC = −q_m/(k_j − k_m), which is −u_f/2 under Greenshields.
4. The queue dissipates after t_d = L / (|w_JC| − |w_1J|).

At a signal, the maximum queue is |w_1J| × red time.

**Moving bottleneck** (slow truck at speed u_T over distance D). The states are:
1 = upstream, 2 = platoon behind the truck (q₂ and k₂ given), C = capacity.

1. Platoon rear moves at w_12 = (q₂ − q₁)/(k₂ − k₁).
2. The truck is on the road for T = D/u_T. Platoon length when it exits: L = (u_T − w_12)·T.
3. After the truck exits, the front discharges at w_2C = (q_m − q₂)/(k_m − k₂).
4. The platoon dissipates after t_d = L / (w_12 − w_2C).

*Worked check, Dec 2016 Q4:* q_m = 2500, k_m = 50, k₁ = 20, q₁ = 1600,
w_12 = −5 km/h, L = 1.333 km, w_2C = −35 km/h, t_d = 2.67 min.

### B3. D/D/1 queuing: Q2

- Plot cumulative arrivals A(t) and departures D(t). **Label the axes and slopes, and mark where the queue clears.**
- Queue length = vertical gap. One vehicle's wait = horizontal gap (FIFO).
- **Total delay = area between the curves.** Split it into triangles and trapezoids.
- Queue clears when A(t) = D(t). For example, λ₁t₁ + λ₂(t − t₁) = μ·t.
- Average delay = total delay ÷ vehicles delayed. State which count you use (usually arrivals until the queue clears).
- **Signal** with ρ = λ/s:
  - Maximum queue = λ·r
  - Queue clears t₀ = ρ·r/(1 − ρ) after green starts
  - Delay per cycle = λ·r² / (2(1 − ρ))
  - Average delay = that ÷ (λ·C)
  - For two cycles, carry any residual queue into cycle 2.
- **Time-varying arrivals** λ(t) = a − b·t: A(t) = a·t − b·t²/2 (integrate).

### B4. Trip generation: Q3

- **Cross-classification:** rate_ij = trips_ij ÷ households_ij from the survey. Forecast = Σ HH_ij × rate_ij.
- **Regression:** rate = b₀ + b₁x₁ + b₂x₂. Use the capped values ("5 or more" = 5). Trips = HH × rate.
- **Interpreting coefficients:** each added person or vehicle adds bᵢ trips, the same amount at every level (a linear, additive assumption).

**Standard "(c) compare" answer:**

| | Cross-classification | Linear regression |
|---|---|---|
| Functional form | None assumed. Captures non-linear effects and interactions. | Linear and additive. Constant marginal effect, no interaction. |
| Data | Needs enough households in *every* cell. Sparse cells are unreliable. | Fewer data. Uses the whole sample. |
| Extrapolation | Impossible outside the categories | Possible but risky. Can give odd values. |
| Statistics | No goodness-of-fit | R², t-tests, confidence intervals |

Both assume **trip rates stay stable over time** and ignore changes in
accessibility and price.

### B5. Gravity model: Q5

- T_ij = P_i · (A_j·F_ij·K_ij) / Σ_x (A_x·F_ix·K_ix). Use K = 1 unless given.
- Friction factors seen on past papers: 1/t, 1/t², 1/d, exp(−0.1·d).
- **Future year:** use the same F and the new P and A, then recompute.
- If attractions must be matched, iterate A_j′ = A_j × (A_j ÷ Σᵢ T_ij).
- **Effect of F:** a steeper friction factor (1/t² rather than 1/t) pushes more trips to nearby zones and intrazonal trips.
- **"Other factors" answer:** cost (tolls, parking, fuel), trip purpose, income and car ownership, the zone's attractiveness and land use, intervening opportunities, physical barriers (rivers, rail lines), jurisdictional or cultural boundaries, transit availability, safety and comfort. These enter through K-factors or a generalized-cost impedance.
- **Assumptions and limits:** trips are proportional to P and A and inverse to impedance. F is calibrated on the base year and assumed stable. The model isn't behavioural. Intrazonal impedance is uncertain.

### B6. Route choice, UE and SO: Q6/Q7

- **UE (Wardrop 1):** every *used* route has the same, minimum travel time. Unused routes have t ≥ t_UE.
- **Linear links** tᵢ = aᵢ + bᵢVᵢ:
  - t* = (Q + Σ aᵢ/bᵢ) / (Σ 1/bᵢ)
  - Vᵢ = (t* − aᵢ)/bᵢ
  - If any Vᵢ < 0, set that route to 0 and re-solve.
  - Check: May 2013 Q6 gives t* = 51.2 min; adding route 3 gives 43.4 min.
- **Non-linear links** (e.g. t = 10 + 20(V/C)²): equate the times and solve with SOLVE or the quadratic formula.
- **SO (Wardrop 2):** minimize Σ Vᵢ·tᵢ(Vᵢ), so the marginal times tᵢ + Vᵢ·tᵢ′ are equal. For linear links, aᵢ + 2bᵢVᵢ are equal.
- **"Does a new route always reduce travel time?"** For separate, non-overlapping routes, UE time can't increase. It stays the same if the new route's free-flow time ≥ t_UE, because nobody uses it. In a general network, adding a link can *increase* everyone's time (the **Braess paradox**), because UE (selfish) ≠ SO.
- **"Drivers know all times / take the shortest path" limitation:** real drivers have imperfect, varying perceptions. Use **stochastic user equilibrium** (logit or probit route choice), traveller information (ATIS), and dynamic assignment.

### B7. Mode choice, multinomial logit: Q7/Q6

- Pᵢ = e^(Vᵢ) / Σⱼ e^(Vⱼ)
- Binary case: P₁ = 1 / (1 + e^(V₂ − V₁))
- **Coefficients:** a negative β means the attribute lowers utility. |β_OVTT| > |β_IVTT| means walking and waiting are disliked more than riding. Value of time = β_time/β_cost (×60 for $/h when time is in minutes).
- **IIA:** P_i/P_j = e^(Vᵢ − Vⱼ), whatever other modes exist. A new or improved mode therefore draws **proportionally** from every mode. This is unrealistic when modes are similar (the **red bus / blue bus** problem, e.g. car-driver vs car-passenger, or bus vs LRT).
- **Fixes:** **nested logit** (put similar modes in one nest), cross-nested or mixed logit, probit, or segmenting the market.

### B8. Q1 theory bank

Write your own 150–200-word bullet answer for each prompt and rehearse them.

1. **Land use and transportation interaction:** better access raises land value and development, which generates more trips, more congestion and pressure for more capacity (a feedback loop). Why it matters for forecasting: land-use forecasts feed trip generation.
2. **Low-density suburbs:** longer trips, more car dependence, transit that is uneconomic, more VKT and emissions.
3. **Residential or commercial development and transit:** density and mixed use support ridership. Transit-oriented development. Accessibility raises commercial value.
4. **Trip-production factors:**
   - Zone: residential density, accessibility
   - Household: size, vehicles, income, workers
   - Person: age, employment, licence
5. **Trip-attraction factors:** employment by sector, retail floor area, school places.
6. **Work vs non-work trips:** work trips are longer, peaked in the AM/PM, regular and less elastic. Non-work trips are shorter, spread through the day, and more flexible in destination and time.
7. **TDM to raise vehicle occupancy:** HOV lanes, carpool matching, preferential parking, parking pricing, congestion pricing, employer programs, flexible hours. Effects: fewer vehicles, lower travel time and fuel use, peak spreading.
8. **Supply-side vs demand-side:** supply-side adds or improves capacity (new lanes, signal timing). Demand-side manages demand (pricing, TDM, telework).
9. **ATIS, V2V/V2I, CAVs:** route and departure-time guidance, incident management, platooning (higher capacity). Risk: induced demand, since cheaper travel time leads to more and longer trips.
10. **Household-based vs zone-based trip generation:** household models are more behavioural and use less aggregated data, but need survey data and household forecasts.
11. **Why forecast HBW / HBO / NHB separately:** they differ in timing, length, mode and sensitivity.
12. **Capacity factors:** more trucks and buses lower capacity (PCE). More lanes raise it. Steep grades lower capacity for heavy vehicles.

---

## A. A6 Highway Design, Construction & Maintenance

### A1. Stopping sight distance and accident reconstruction

- **SSD** = 0.278·V·t_r + V² / (254·(f ± G))
  - V in km/h, G as a decimal, + for uphill
  - t_r = 2.5 s
  - f from the table in the paper, or a/g = 3.4/9.81 = 0.35
- **Braking from V₁ to an impact speed V₂:** d_b = (V₁² − V₂²) / (254·(f ± G))
- **Reconstruction recipe:**
  1. Find the *available* S from the curve geometry, using the **given** eye and object heights (don't use 658 when h₂ = 1.10 m).
  2. Find the distance the driver actually needed: 0.278·V·t_r + d_b.
  3. Compare the two, at both the actual and the design speed.
  4. List other factors: speed above design, reaction time > 2.5 s (fatigue, distraction, alcohol), worn tires or wet pavement (lower f), brakes, night, weather, the downgrade.

### A2. Vertical curves (G and A in %, lengths in m)

**Elevations and stations:**
- y(x) = y_PVC + (G₁/100)·x + (G₂ − G₁)/(200·L)·x²
- Offset from tangent: Y = A·x²/(200L). Middle offset: E = A·L/800.
- High or low point: x = G₁·L/(G₁ − G₂) = K·|G₁|
- K = L/A. PVC = PVI − L/2. PVT = PVI + L/2.

**Crest SSD** with eye h₁ and object h₂. For design, h₁ = 1.08 and h₂ = 0.60 give the constant 658.
- S < L: L = A·S² / (200(√h₁ + √h₂)²) = **A·S²/658**
- S > L: L = 2S − 200(√h₁ + √h₂)²/A
- Available S when S < L: S = √(200·L·(√h₁+√h₂)²/A)
- Available S when S > L: S = L/2 + 100(√h₁+√h₂)²/A
- Always check your S vs L assumption afterwards.

**Crest PSD** (h₁ = h₂ = 1.08): L = A·S²/864 when S < L.

**Sag headlight** (H = 0.60 m, β = 1°):
- S < L: L = A·S²/(200(H + S·tan β)) = **A·S²/(120 + 3.5·S)**
- S > L: L = 2S − (120 + 3.5·S)/A

**Sag comfort:** L = A·V²/395

**Underpass** (clearance C, h₁ = 2.4, h₂ = 0.6):
- S < L: L = A·S² / (800·(C − (h₁+h₂)/2))
- S > L: L = 2S − 800(C − (h₁+h₂)/2)/A

**Stationing:** read the question. "1+234.000" means 1234 m when a station is 1000 m, but some questions use 100 m or 30 m stations.

### A3. Horizontal curves

**Radius:** e + f_s = V²/(127·R), so **R_min = V²/(127·(e_max + f_s,max))**

**Curve elements:**
- T = R·tan(Δ/2)
- L = π·R·Δ/180
- LC = 2R·sin(Δ/2)
- M = R(1 − cos(Δ/2))
- E = R(1/cos(Δ/2) − 1)
- **PC = PI − T, and PT = PC + L** (not PI + T)

**Sight clearance.** R_v is the radius to the centre of the **inside lane**, and angles are in degrees.
- M_s = R_v·(1 − cos(28.65·S/R_v))
- S = (R_v/28.65)·cos⁻¹((R_v − M_s)/R_v)
- Distance from the lane edge = M_s − lane width/2.
- **Speed limit from a clearance:** find S from M_s, then solve SSD(V) = S. This is a quadratic in V.

**Field layout:** deflection angle δ = 28.65·ℓ/R (ℓ = arc length from the PC). At the PT, δ = Δ/2.

### A4. Spirals, superelevation runoff, clear zone (TAC/MTO style)

- Spiral parameter: **A² = R·L_s**
- Comfort (Shortt formula): L_s = V³/(46.7·R·C). With C = 0.6 m/s³ this becomes **L_s = 0.0357·V³/R**, as in the exam appendix.
- Runoff, rotating about the centreline: L_r = w·n·e / Δ, where w = lane width, n = lanes rotated on one side, Δ = relative slope from the table.
- Tangent runout: L_t = (e_NC/e)·L_r
- Adopt the **largest** of the comfort, runoff and table minimum lengths, and round up.
- **"Is the radius safe?":** compare R with R_min for the design speed (posted + 10 to 20 km/h) and e_max, or look up the required e for this R in the TAC table. For a curve on a grade, the up-grade and down-grade lanes differ.
- **Clear zone:**
  1. Take the base width from the table (design speed, AADT, fore/back slope, cut vs fill).
  2. Multiply by the **curve correction factor**. It applies to the **outside of the curve only**, and only when R < 900 m.
  3. Measure from the edge of the travelled lane.

### A5. Traffic loading (ESAL)

- ESAL in year 1 for each class = AADT × %class × TF × DD × LD × 365
  - TF = truck factor for that class and road type (from the table)
  - DD ≈ 0.5
  - LD for 1 / 2 / 3 / 4+ lanes per direction: 1.0 / 0.8–1.0 / 0.6–0.8 / 0.5–0.75
- **Growth factor:** GF = [(1+g)ⁿ − 1]/g
- **Split growth:** GF = [(1+g₁)^n₁ − 1]/g₁ + (1+g₁)^n₁ · [(1+g₂)^n₂ − 1]/g₂
- **Design ESAL** = Σ over classes of (ESAL year 1 × that class's GF)
- With axle data instead: ESAL/day = Σ (axles/day × LEF from the table for the assumed SN), then iterate SN.
- Rule of thumb: LEF ≈ (P/80 kN)⁴

### A6. AASHTO-93 flexible design

**Design equation** (M_R in psi, ΔPSI = p₀ − p_t):

log₁₀W₁₈ = Z_R·S₀ + 9.36·log₁₀(SN+1) − 0.20 + log₁₀[ΔPSI/2.7] / [0.40 + 1094/(SN+1)^5.19] + 2.32·log₁₀M_R − 8.07

**Structural number:** SN = a₁D₁ + a₂D₂m₂ + a₃D₃m₃ (D in **inches**)

**Inputs:**

| Reliability R (%) | 50 | 70 | 75 | 80 | 85 | 90 | 95 | 99 |
|---|---|---|---|---|---|---|---|---|
| Z_R | 0 | −0.524 | −0.674 | −0.841 | −1.037 | −1.282 | −1.645 | −2.327 |

- S₀: flexible 0.40–0.50, rigid 0.30–0.40
- a₁: from the chart (E_AC = 450,000 psi gives about 0.44)
- a₂ = 0.249·log₁₀E_BS − 0.977 (30,000 psi gives 0.14)
- a₃ = 0.227·log₁₀E_SB − 0.839 (15,000 psi gives 0.11)
- **Drainage quality** by time to remove water: excellent 2 h, good 1 day, fair 1 week, poor 1 month, very poor never drains. Read mᵢ from the table using that quality and the % of time near saturation.
- M_R ≈ 1500·CBR (psi)

**Layered design:**
1. SN₁ from the equation with M_R = E_base. Then D₁ ≥ SN₁/a₁ (round up and apply the minimum), and SN₁* = a₁·D₁.
2. SN₂ with M_R = E_subbase. Then D₂ ≥ (SN₂ − SN₁*)/(a₂m₂).
3. SN₃ with the subgrade M_R. Then D₃ ≥ (SN₃ − SN₁* − SN₂*)/(a₃m₃).

**Minimum thicknesses (inches):**

| ESAL | < 50k | 50k–150k | 150k–500k | 0.5M–2M | 2M–7M | > 7M |
|---|---|---|---|---|---|---|
| AC | 1.0 | 2.0 | 2.5 | 3.0 | 3.5 | 4.0 |
| Base | 4 | 4 | 4 | 6 | 6 | 6 |

**Related uses:**
- **Overlay:** SN_ol = SN_future − SN_eff, then D_ol = SN_ol/a_ol.
- **Remaining life:** compute W₁₈ for the actual SN, then find n from the growth factor.
- Use the calculator's **SOLVE** with X = SN, and confirm the result on the nomograph.

### A7. AASHTO-93 rigid design (JPCP)

**Design equation** (D in inches, S′c and E_c in psi, k in pci):

log₁₀W₁₈ = Z_R·S₀ + 7.35·log₁₀(D+1) − 0.06 + log₁₀[ΔPSI/3.0] / [1 + 1.624×10⁷/(D+1)^8.46] + (4.22 − 0.32·p_t)·log₁₀{ S′c·C_d·(D^0.75 − 1.132) / [215.63·J·(D^0.75 − 18.42/(E_c/k)^0.25)] }

**Inputs:**
- **J** (load transfer): 3.2 with dowels and asphalt shoulders; 2.5–3.1 with dowels and tied PCC shoulders
- **C_d:** from the drainage table, used the same way as mᵢ
- E_c ≈ 57,000·√f′c (psi). Modulus of rupture S′c ≈ 7.5 to 10·√f′c (psi).

**k-value:**
- Subgrade alone: k = M_R/19.4
- With a subbase:
  1. Composite k∞ from the chart (M_R, E_SB, D_SB)
  2. **Rigid-foundation correction** if bedrock is within 10 ft
  3. Seasonal effective k
  4. **Loss-of-support** correction: LS 1–3 for unbound granular and 2–3 for fine subgrade
- Flexible and rigid ESALs are **different**, because rigid pavements have their own LEF tables. You can't reuse the flexible ESAL for a rigid design.

### A8. Asphalt mix volumetrics (P in % of total mix)

**Specific gravities:**
- Blend: G_sb = ΣPᵢ / Σ(Pᵢ/Gᵢ). G_sa is calculated the same way.
- Superpave estimate: G_se = G_sb + 0.8·(G_sa − G_sb)
- G_mm = 100 / (P_s/G_se + P_b/G_b), with P_s = 100 − P_b
- G_se = P_s / (100/G_mm − P_b/G_b)
- Measured G_mb = W_dry / (W_SSD − W_water)

**Binder:**
- Absorbed binder (% of aggregate): P_ba = 100·G_b·(G_se − G_sb)/(G_sb·G_se)
- Effective binder: P_be = P_b − P_ba·P_s/100
- Binder by weight of aggregate = 100·P_b/(100 − P_b)

**Voids:**
- **V_a** = 100·(G_mm − G_mb)/G_mm
- **VMA** = 100 − G_mb·P_s/G_sb
- **VFA** = 100·(VMA − V_a)/VMA
- Dust proportion = P₀.₀₇₅/P_be (target 0.6–1.2)

**Gyratory compaction:**
1. G_mb,est(N) = W_m / (π·d²/4 · h_N · γ_w)
2. Correction C = G_mb,measured / G_mb,est(N_max)
3. %G_mm(N) = 100·C·G_mb,est(N)/G_mm

Typical Superpave criteria:
- %G_mm ≤ 89% at N_ini (for 3M ESALs or more), 96% at N_des (V_a = 4%), and ≤ 98% at N_max
- VMA min: 15 / 14 / 13 / 12% for 9.5 / 12.5 / 19 / 25 mm nominal maximum size
- VFA: 65–75% for 3M ESALs or more

**Aggregate tests** (A = dry, B = SSD, C = submerged):
- Bulk RD = A/(B−C)
- SSD RD = B/(B−C)
- Apparent RD = A/(A−C)
- Absorption = 100·(B−A)/A
- Free water = total moisture − absorption

**PG grading:**
- High grade: the highest standard grade (52/58/64/70/76) at or **below** the temperature passed.
- Low grade: the coldest standard grade (−22/−28/−34/−40) the binder actually **meets**.
- Example: passes 68.3 °C and −33.9 °C, so the grade is **PG 64-28**.
- Tests and what they target:
  - RTFO: short-term ageing
  - PAV: long-term ageing
  - DSR G*/sin δ: rutting
  - DSR G*·sin δ: fatigue
  - BBR stiffness and m-value: thermal cracking
  - DTT: low-temperature strain
  - RV: workability

### A9. Soils, earthwork, LCCA, frost

**Compaction:**
- γ_d = γ_wet/(1 + w)
- Relative compaction = γ_d,field/γ_d,max
- If w_field > OMC, dry the soil before compacting.
- Zero-air-voids line: γ_zav = G_s·γ_w/(1 + w·G_s)

**Earthwork volumes:**
- Average end area: V = L·(A₁ + A₂)/2
- Pyramid, when one area is zero: V = L·A/3
- Prismoidal: V = L·(A₁ + 4A_m + A₂)/6
- Shrinkage: cut needed = fill/(1 − s)

**Life-cycle cost:**
- PW = Σ Cₙ/(1+i)ⁿ − Salvage/(1+i)^N
- With unequal analysis periods, compare **EUAC** = PW·i(1+i)^N / ((1+i)^N − 1), or use a common analysis period.

**Frost and GBE:**
- Total thickness must be at least the required % of the frost depth.
- GBE = Σ tᵢ × equivalency factor. Ontario factors: AC 2.0, PC-treated base 1.8, asphalt-treated base 1.5, granular base 1.0, granular subbase 0.67.
- To swap materials, keep the GBE and the frost thickness.

### A10. A6 short-answer bank (bullets to memorize)

- **ESAL concept:** converts mixed axle loads into the equivalent number of 80 kN (18-kip) single-axle passes that cause the same serviceability loss (AASHO Road Test, about a 4th-power law).
- **AASHTO-ME traffic:** uses **axle-load spectra** by axle type, month and hour, not ESALs. Mechanistic responses (stress and strain) feed empirical transfer functions that predict IRI, rutting and cracking.
- **LEF higher at SN 5 than SN 4:** an LEF is *relative* to an 18-kip axle on the *same* pavement. The stronger pavement still carries far more total load, so a higher LEF doesn't mean more absolute damage.
- **Conservative growth rate:** reliability (Z_R·S₀) already covers uncertainty. Stacking conservative inputs over-designs. Use the best estimate and run a sensitivity check.
- **Environment in AASHTO-93:** seasonal effective M_R (relative damage u_f = 1.18×10⁸·M_R^−2.32), drainage mᵢ and C_d, serviceability loss from frost heave and swelling, and temperature effects on E_AC (and so on a₁).
- **Performance measures:** IRI, PSI/PSR, rut depth, cracking, faulting, friction (skid number), FWD deflection, punchouts.
- **Distresses and causes:**

| Distress | Type | Causes |
|---|---|---|
| Fatigue (alligator) cracking | Structural | Tensile strain at the bottom of the AC. Too thin, weak base, poor drainage. |
| Rutting | Structural or mix | Unstable mix (excess binder, rounded aggregate, heat) or deformation in the base/subgrade |
| Low-temperature (transverse) cracking | Mix/climate | Thermal contraction. Binder too stiff or aged. |
| Bleeding | Functional | Excess binder, low air voids |
| Polished aggregate | Functional | Soft aggregate worn smooth by traffic |
| D-cracking (PCC) | Structural | Freeze–thaw of susceptible coarse aggregate |
| Pumping (PCC) | Structural | Water and fines ejected at joints under load on an erodible base |
| Map cracking (PCC) | Surface | ASR, or poor curing and finishing |

- **Frost heave:** needs frost-susceptible soil (silts), freezing temperatures and a water supply, which together form ice lenses. The pavement then weakens on thaw. Fixes: non-frost-susceptible granular cover to the required % of frost depth, drainage or a lower water table, insulation, a capillary break, or replacing or stabilizing the soil.
- **Marshall vs Superpave:**

| | Marshall | Superpave |
|---|---|---|
| Compaction | Impact hammer (75 blows) | Gyratory compactor (N_ini, N_des, N_max) |
| Selection criteria | Stability, flow, volumetrics | Volumetrics, consensus aggregate properties, PG binder for the climate |
| Strengths | Cheap, long experience | Simulates field compaction better. Performance-related, climate- and traffic-specific. |
| Weaknesses | Empirical, poor simulation of field compaction | Costlier equipment. No strength test at the volumetric level. |

- **PGAC vs penetration grading:** PG uses performance properties at the actual high and low pavement temperatures for the climate, including aged binder. Penetration grading is one empirical consistency test at 25 °C.
