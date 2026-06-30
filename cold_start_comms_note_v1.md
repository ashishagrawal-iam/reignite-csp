# Cold Start CSP Communications — Objectives, Boundary Values, Kill Conditions

*Independent objective-and-guardrail definition for CSP communications during the Cold Start program. Objective first, then operate within boundaries. No design references in the body — designs (including the directional MBG comms work already in circulation) are evaluated against this note, not the other way round.*

---

## Scope of this note

What this note is:

- A clean objective for **one-time** comms and a clean objective for **repetitive** comms  
- The boundary values (BVs) every comms surface must operate inside  
- The kill conditions (KCs) that would invalidate the comms approach  
- A note on how this aligns to the broader pull-based model

What this note is **not**:

- A revalidation of existing comms design  
- A retro-fitted justification for work in progress

Any existing design artifacts ([mockups, copy decks, journey diagrams](https://ashishagrawal-iam.github.io/MBG_v1/)) are treated as directional field input. They get evaluated against the objective and BVs *after* this note is locked, not before.

---

## Objective 1 — One-time communications

**Objective:**

To equip the CSP to enter the Mutual Compact: a clear, two-way contractual relationship with Wiom, with full understanding of what each side commits, the duration, the safety net, and the named end-date.

**Why we believe this is the right objective (and not "inform CSPs of the scheme"):**

"Inform" makes the comms a broadcast; "[equip to enter a compact](https://docs.google.com/document/d/1szeqMvFZmeqWmkcb7hzv-C99HbEmFFvG5ksVJarToTU/edit?usp=sharing)" makes the comms an act of mutual contracting. The two sound similar but diverge sharply at the endpoint.

- Informing → the CSP reads, understands, and is then *separately* asked to sign. Sign-up becomes a downstream step disconnected from the comms.  
- Equipping to compact → the comms *is* the contracting act. The endpoint of the journey is the CSP making a mutual commitment with eyes open.

The second framing is what a pull-based model demands. A CSP who pulls themselves into the compact is structurally different from one who was sold the scheme.

**Concrete example of the difference:**

Same content, two framings. Both technically inform the CSP.

- Violates the objective: *"Wiom is launching the Minimum Guarantee Program from July to September. CSPs converting 70%+ of leads will earn at least ₹10,000/month. \[Read more\]"*  
- Honours the objective: *"From July to September, Wiom commits to send you leads weekly. You commit to install ≥xx% of them. If we miss our lead commitment, ₹10,000 protects you. \[Sign the Compact\]"*

The first is an announcement; the CSP is a recipient. The second names both commitments, names the safety net, and ends with the contractual action. The CSP is a counterparty.

**What this objective rules in / rules out:**

| Rules in | Rules out |
| :---- | :---- |
| The compact terms (both sides, side-by-side) | "Welcome to Wiom" / relationship-warming preambles |
| The 3-month window stated up front | Open-ended "we value our partners" framing |
| The make-good (₹10,000 floor) named plainly | The floor presented as Wiom's generosity rather than a make-good |
| One-tap sign-up after terms are seen | Information-only flows that defer signup to a separate channel |

---

## Objective 2 — Repetitive communications

**Objective:**

To give the CSP continuous, passive visibility of where they stand against their commitment, and to surface event-triggered information at moments of consequence — so the CSP can act on their own initiative.

**Why we believe this is the right objective (and not "reinforce milestones"):**

"Reinforce" implies Wiom is reaching out to keep the CSP engaged. That's push, not pull. It is also where the failure mode "too frequent" almost always originates — well-meaning teams scheduling weekly summaries and daily reminders that violate the frequency boundary as soon as the program scales.

The objective splits comms into **two clean categories**:

1. **Passive** — information that is *available* when the CSP opens the app. The home MBG card. The wallet ledger row. The drilldown screen. Wiom puts the information there; the CSP comes to it. ([Why we believe "passive" should be the default — see Appendix A.](#appendix-a-—-passive-vs-active-comms))  
2. **Event-triggered active** — a push, banner, or dialog that fires *only when CSP state has actually changed in a way that requires action*. A lead is 1 day from expiry. The rate gate just got cleared. The payout has hit the wallet.

**What this rules out, hard:** all scheduled or time-driven comms. No weekly summary. No daily nudge. No "haven't seen you in a while" pings. The moment the system sends something on a schedule rather than on an event, it is Wiom pulling the CSP — the inverse of the pull-based model.

**Concrete example of the difference:**

Same information, three framings — only the third honours the objective.

- *"Your install rate is 60%. Please improve to qualify for the guarantee."* — sent at 6 PM daily. Active, scheduled. **Violates.** Wiom is pulling.  
- *"You're failing the guarantee\!"* — sent immediately when rate dips. Active, event-triggered, but blame-loaded. **Violates** (and violates BV3 — see below).  
- *"बस 1 और इंस्टॉल — गारंटी पक्की"* — fires when state crosses into the actionable band, with the specific action quantified. Active, event-triggered, factual. **Honours.**

Plus the home MBG card always showing the current rate against the gate. **Passive. Honours.**

**What this objective rules in / rules out:**

| Rules in | Rules out |
| :---- | :---- |
| Home MBG card (passive, always available) | Daily / weekly summary push or SMS |
| Wallet pending-row for the maturity tail | "We miss you" reactivation pings |
| Push when a lead is hours from expiry | Generic engagement nudges on a schedule |
| Dialog when the gate is cleared or missed at month-end | Active comms that don't correspond to a state change |
| Drilldown screen the CSP opens by tap | Notifications repeating information already on the home card |

---

## Boundary Values — the guardrails every comms surface obeys

Three are inherent in how comms have been framed for this program: factual, non-persuasive, frequency-bounded. Three more from the broader Cold Start work we'd propose elevating to BV level here, because they generalize to any future intervention's comms (Ladder, compensation changes, quality programs) and because they protect the persistence floor that defines Cold Start success.

| BV | Statement | Why it's a BV |
| :---- | :---- | :---- |
| **BV1 — Factual** | Every CSP-facing message states what is true, in plain terms, with named numbers and named dates. No characterization of the relationship, no editorializing. | A factual frame protects against the entitlement framing that destroyed Ola's persistence (see BV4). It also keeps the message verifiable — the CSP can hold Wiom to its own words. |
| **BV2 — Non-persuasive** | The message does not try to convince the CSP. It provides the information needed to act, and the CSP decides. | Persuasion in supplier comms is the on-ramp to "we sold them the scheme" — which then sets up the "Wiom over-promised" backlash when reality differs from the pitch. Non-persuasive comms preserve trust at the cost of a slower opt-in curve. The Cold Start framework already accepts that trade. |
| **BV3 — Frequency-bounded, relevance-driven** | Comms are tied to **CSP-state events** (lead expiring, gate crossed, payout settled), never to a Wiom-side clock. No scheduled cadence. | Scheduled comms are how every well-intentioned program ends up at "too frequent" within 30 days. The only durable defence is to forbid the calendar from being a trigger at all. |
| **BV4 — Sunset, not partnership** | Every message about the scheme reinforces temporariness and the named endpoint. Never frames the scheme as Wiom's investment in the relationship. | The single most expensive lesson from supply-side cold-start history. **Ola 2017 vs Uber 2021 ran nearly identical mechanisms with opposite outcomes; the difference was almost entirely in this framing.** Even one warm-fuzzy "we value your partnership" message can undo dozens of "3-month window" messages because CSPs talk to each other and don't separate formal terms from tone. ([Full Ola vs Uber contrast — Appendix B.](#appendix-b-—-ola-2017-vs-uber-2021)) |
| **BV5 — No-blame, owner-aware** | Every parameter-specific message names the failing parameter *and* identifies its owner. The word "fail" / "असफल" does not appear in any CSP-facing surface, in any language, anywhere. | The scheme has multiple gates (volume floor, install rate, lead maturity) with different owners. Generic "you're failing" messages break trust on the parameters Wiom owns and break pull-coherence by blurring ownership. ([Owner-mapping detail — Appendix C.](#appendix-c-—-owner-mapping-by-parameter)) |
| **BV6 — One-sentence rule** | Any single comms surface — banner, push, dialog, sheet — must be graspable by the CSP in one sentence. If it takes more than one sentence to be understood, the surface is wrong. | The CSP is operating a small business in Hindi, often in a noisy environment, on a phone, between physical jobs. The one-sentence rule forces the comms to do what it is actually trying to do: deliver one piece of decision-relevant information. Multi-sentence surfaces are nearly always trying to do two jobs and end up doing neither. |

---

## Kill Conditions — what would invalidate the comms approach

These are the failure modes that, if observed, mean the comms layer is undermining the intervention rather than enabling it. Distinct from BVs (which are designed-in guardrails) — these are observed-outcome triggers.

| KC | Trigger | Action |
| :---- | :---- | :---- |
| **KC1 — Entitlement signal** | CSP-side language in support tickets or field reports starts characterising the floor as "Wiom's commitment to me" rather than as a temporary make-good. | Review every active surface for BV4 compliance. Tighten or pull surfaces that have drifted. |
| **KC2 — Frequency creep** | The per-CSP push/SMS rate trends upward over the program (instead of staying flat or declining as state changes get rarer). | Hard cap and audit. The trigger logic is generating false positives or BV3 is being violated by adjacent systems. |
| **KC3 — Blame attribution** | Field signal (support, CSP voice) that CSPs are reading non-qualification due to Wiom's non-adherence as their own failure. | BV5 violation somewhere in the surface set. Find and fix. |
| **KC4 — Comms-driven opt-in** | Opt-in rate is high but conversion-during-program is materially lower than baseline among opt-ins. | Indicates BV2 was violated upstream — CSPs were persuaded in but didn't actually understand what they signed. Strengthen Objective 1 surfaces. |
| **KC5 — Surface count creep** | The number of distinct active surfaces (pushes, SMS, banners, dialogs) trends upward over the program. | Almost always a BV3 failure dressed up as "more is better." Cap and prune. |

---

## Alignment to the pull-based model

Both objectives operationalize the pull-based architecture in the same way: they assume the CSP comes to the system on their own initiative, and shape comms to support that.

- **Objective 1** ends in a *mutual commitment* the CSP signs, not a scheme they accept. Pull-coherent.  
- **Objective 2** keeps the default *passive* and reserves active comms for state changes the CSP must act on. Pull-coherent.  
- **BV3** forbids the calendar as a trigger — calendars are how systems re-engage suppliers who would otherwise drift, which is push by definition.  
- **BV4** keeps the framing structural (a window, a commitment, an endpoint) rather than relational ("we value you") — the latter creates dependence, which is the opposite of pull.

If the comms layer holds these objectives and BVs, it actively builds the pull-model. If it drifts on any of them, it actively erodes the pull-model. There is no neutral middle.

---

## Next step

Once this note is approved, the directional MBG comms work already in circulation can be evaluated against it. Surfaces that hold up are kept; surfaces that drift on any BV are reworked or removed before launch.

---

# Appendix

## Appendix A — Passive vs Active comms {#appendix-a-—-passive-vs-active-comms}

The same information can be passive or active depending on how it reaches the CSP. Same content, very different relationship.

| Same information | Active version | Passive version |
| :---- | :---- | :---- |
| Current install rate | SMS at 6 PM: *"Your install rate is 60% — improve it"* | Home MBG card showing current rate when CSP opens the app |
| ₹10,000 floor status | Push: *"You're at risk of missing the floor\!"* | Card on home reading *"गारंटी जोखिम में"* with current numbers |
| 14-day lead expiring | Daily WhatsApp reminder for each open lead | Lead card on the home feed with a countdown timer |

**Default state \= passive.** The CSP comes to the information.

**Allowed exceptions \= event-triggered active.** Only when CSP state has actually changed in a way that requires action *now*:

- A lead is hours from 14-day expiry (cannot be deferred)  
- The gate has just been cleared or missed (the consequence is final)  
- The payout has settled (the wallet has a new entry the CSP would want to know about)

**Forbidden \= scheduled active.** Anything that fires on a Wiom-side clock — daily, weekly, monthly — is push. Push is the inverse of pull.

The discipline that prevents drift: every proposed active surface must be defensible by naming the CSP state change that triggers it. If the trigger is "every Monday at 9 AM," the surface is wrong by construction.

---

## Appendix B — Ola 2017 vs Uber 2021 {#appendix-b-—-ola-2017-vs-uber-2021}

The single most useful real-world contrast for BV4 (Sunset, not partnership), because the *mechanism was nearly identical* between the two companies. The difference was almost entirely in comms framing and sunset discipline.

**The setup — both companies.** Ride-hailing cold-start. Drivers needed to be on the road in volume for the marketplace to clear. Both companies introduced earnings guarantees (income floor if you complete X trips / drive Y hours). Both committed real money to it. Same instrument category.

**Ola, 2015–2017:**

- Guarantees framed as **partnership and investment**. Internal and external messaging emphasized *"we value our driver-partners"* and *"we are committed to your success."* Sunset was either unstated or vaguely future-tense.  
- Drivers, as a result, **internalised the guarantee level as their compensation**. The high earnings became "what driving for Ola pays" in their mental model — not "what driving for Ola pays during a temporary acquisition phase."  
- Capital structure followed: drivers took loans to buy cars based on guarantee-level earnings. Family budgets were built around it. The numbers anchored as the new normal.  
- From early 2017, Ola began progressively cutting incentives. From the driver's point of view, this was **a pay cut, not a scheme ending**. No promise had ever been made about an end-date.  
- Driver protests across Mumbai, Bengaluru, Hyderabad, Delhi-NCR. Asset finance defaults. Wave of drivers exited to Uber, then to Rapido, and (years later) to Namma Yatri's zero-commission model. The reputational damage on the platform-driver relationship persists today; much of the current "platforms exploit drivers" narrative in Indian ride-hailing traces to this window.  
- **The mechanism worked. The framing destroyed the persistence.** Drivers were on the road in volume during the guarantee period — exactly as intended. Behaviour did not survive removal because the framing had never set up removal as a thing that would happen.

**Uber, 2021 (US post-COVID):**

- Guarantees framed as **a temporary window during recovery**. The public language: *"earnings are at all-time highs right now"* / *"drivers can take advantage of this while it lasts"* / *"as more drivers return, earnings will normalize."*  
- Sunset named explicitly: a **$250M stimulus** with a stated duration. Press releases, in-app messaging, earnings calls all said the same thing. CFO statements reinforced that the stimulus would taper as supply recovered.  
- Drivers internalised the guarantee as **a window they were choosing to walk through**. The high earnings were not "what driving for Uber pays" — they were "what driving for Uber pays during a known, temporary phase."  
- Q3–Q4 2021: as drivers returned and the stimulus tapered (exactly as communicated), earnings normalised toward pre-pandemic levels. **No large-scale protests.** Some grumbling, normal at any compensation change, but no organised backlash and no major driver exodus.  
- **Supply held through the Omicron surge in Q4 2021 without a re-stimulus.** Behaviour had persisted. The persistence floor cleared in real-world conditions.

**The asymmetry that matters for our BV:**

Same instrument. Same money order-of-magnitude (relative to the business). Same supplier population type. Outcome differed by orders of magnitude.

The single biggest difference was the comms framing — what the supplier was told about what the scheme was *for*.

Ola told drivers *"we value you, we're invested in you."* Uber told drivers *"this window is open, while it lasts."*

Both were true. Only one survived contact with the sunset.

---

## Appendix C — Owner mapping by parameter {#appendix-c-—-owner-mapping-by-parameter}

The scheme has three parameters that can fail. Each has a different owner. Comms must name both the parameter and its owner explicitly.

| Failing parameter | Owner | What the CSP sees | Why this attribution |
| :---- | :---- | :---- | :---- |
| **Volume floor** — fewer than 3 leads in the month | **Wiom** | *"गारंटी इस महीने लागू नहीं — हम और लीड भेजने पर काम कर रहे हैं"* (the guarantee doesn't apply this month — we're working on sending more leads) | Low lead volume is a demand-side shortfall. Blaming the CSP for leads Wiom didn't send breaks trust and the pull-model ownership boundary. |
| **Install rate gate** — install rate below xx% | **CSP (actionable)** | *"बस X और इंस्टॉल — गारंटी पक्की"* (just X more installs — guarantee secured) | The CSP can act. The comms quantifies the action and the unlock, never characterises the state as failure. |
| **Lead maturity** — lead approaching 14-day expiry | **CSP (actionable) \+ Wiom (informed)** | *"2 लीड 3 दिन में पूरी करें, वरना दर पर असर पड़ेगा"* (complete 2 leads in 3 days, or your rate will be affected) | Explains the consequence before it bites. Turns an invisible rule into an actionable reminder. |

**The non-negotiable.** The word "fail" / "असफल" does not appear in any CSP-facing surface, in any language, anywhere. A parameter not met is *always* paired with either (a) an action the CSP can take, or (b) an explicit statement that Wiom owns the shortfall.

Generalises beyond MBG: any future scheme with multiple parameters needs the same discipline. Encoding it as a BV means we don't relearn it on the Ladder, on compensation changes, or on any quality program.

---

