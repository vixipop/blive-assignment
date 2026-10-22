# Blive Job Card: Research Brief

Desk research, Oct 2026. Interview answers below are **hypotheses** to test, not real quotes.

---

## 1. Key numbers

| Fact | Number | Source |
|---|---|---|
| Blive rider rent | from ₹1,500/week (~₹214/day), maintenance included | [eMobility+](https://emobilityplus.com/2024/06/11/blive-launches-innovative-ezy-ev-rental-program-to-empower-last-mile-delivery-riders/amp/) |
| Blive's guarantee to franchise partners | ₹5,000–5,500 per vehicle per month | [Automotive Lead News](https://automotiveleadnews.com/2025/11/28/blive-scales-up-its-ev-fleet-with-additional-5000-electric-two-wheelers-in-bangalore/) |
| Rider earnings | ₹102 per logged-in hour, about **₹1,000 per day lost** (10 h) | [Business Today](https://www.businesstoday.in/amp/latest/corporate/story/look-at-the-full-picture-deepinder-goyal-breaks-down-delivery-partner-earnings-with-hard-facts-509252-2026-01-02) |
| Riders who can't afford one day off a week | 48% | [The Quint / PAIGAM–IFAT](https://thequint.com/news/india/gig-workers-cab-drivers-delivery-persons-working-conditions-survey-aggregators-apps) |
| Hub wait (competitor, Yulu) | "at least 2–3 hours" per visit | [ThePrint](https://theprint.in/ground-reports/rental-e-scooters-were-meant-for-office-goers-gig-workers-now-bring-up-to-90-of-business/3070852/) |
| Time in a service event that isn't repair work | over 80% (vendor claim) | [Fleet Maintenance / Decisiv](https://www.fleetmaintenance.com/shop-operations/shop-management/article/11142176/how-srm-technology-can-cut-downtime) |
| Technician time lost to admin | 18% of hours | [Salesforce](https://www.salesforce.com/resources/articles/field-service-trends) |
| Technician pay, Bengaluru | ₹17–25k/month, close to the ₹19.2k legal minimum | [WageIndicator](https://wageindicator.org/en-in/ai/work-in-india/minimum-wage/31024-karnataka/31192-automobile-engineering-incl-manufacturing-assembly-body-building-servicing-repairs/) |
| Bengaluru languages | Kannada 44.5%, Tamil 15%, Telugu 14%, Hindi 6% | [Udayavani](https://udayavani.com/?p=1115277) |
| Workshop noise | most tools above 85 dBA | [CDC/NIOSH](https://stacks.cdc.gov/view/cdc/192865) |

**Cost of one scooter-day in the workshop:** about ₹1,000 lost by the rider plus about ₹214 in rent Blive doesn't collect. My arithmetic from the numbers above.

---

## 2. Pain points by audience

### Technician (main user)
- **Logging is extra work.** Admin already takes 18% of their time, so they back-fill at the end of the day ("pencil-whipping") ([Tractian](https://tractian.com/en/glossary/pencil-whipping)).
- **Waiting looks like slacking.** Technicians can be fast at the work itself yet busy only 60% of the time because of parts waits ([CCC](https://www.cccis.com/news-and-insights/posts/the-labor-efficiency-equation-finding-hidden-capacity)). On paper, that waiting is invisible and gets blamed on them.
- **Double entry.** When WhatsApp and an app run side by side, workers get "digital fatigue" ([PMC, ASHA study](https://pmc.ncbi.nlm.nih.gov/articles/PMC12428105/)).
- **Text and typing.** Text UIs are unusable for first-time low-literacy users ([Medhi et al.](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/ToCHI2711_Medhi.pdf)). About 70% of Indian-language users struggle with English keyboards ([Reverie/KPMG](https://reverieinc.com/?p=1256805)).
- **EV skills gap.** India trains 15–20k EV technicians a year against a need for 100–200k by 2030 ([Punjab Kesari/ANI](https://english.punjabkesari.com/business/how-indias-local-garages-are-quietly-getting-ev-ready/)).

### Service manager
- **Can't see what's stuck.** Status lives in WhatsApp threads with no aging and no reason codes. Hold reasons kept as free text can't be reported on ([MaintainX forum](https://community.getmaintainx.com/product-q-a-6/not-enough-status-372)).
- **Doesn't trust the numbers.** Spurious parts were about 36% of India's aftermarket ([ACMA–SIAM](https://autocarpro.in/news-national/acma-siam-immediate-government-action-contain-growing-menace-counterfeit-2518)). Labour charges are inflated or vague ([WhichCar](https://www.whichcar.com.au/?p=674712)).
- **Late invoices.** Paper tickets take 15–25 days to invoice versus 1–3 days digital (vendor claim) ([FleetRabbit](https://fleetrabbit.com/industry/oil-and-gas/oilfield-fleet-reducing-days-to-invoice)).
- **Alert fatigue risk.** About 73% of alerts get overridden when there are too many ([JAMIA](https://pmc.ncbi.nlm.nih.gov/articles/PMC7646870)).

### Rider
- **Lost income.** About ₹1,000 per day off the road, and 48% can't absorb a single day off.
- **No ETA.** "Uncertain waits feel longer than known waits" ([Maister](https://davidmaister.com/articles/1/52/)). Riders currently call the hub.
- **Disputed damage charges.** Blive promises "zero additional cost" for maintenance. Karnataka's Gig Workers Act 2025 requires transparent deductions and dispute resolution within 14 days ([MediaNama](https://www.medianama.com/2025/08/223-karnataka-gig-workers-welfare-bill-2025-explainer/)).
- **Unreliable replacements.** One rider went through 3–4 faulty scooters in a week ([ThePrint](https://theprint.in/ground-reports/rental-e-scooters-were-meant-for-office-goers-gig-workers-now-bring-up-to-90-of-business/3070852/)).

---

## 3. Interview guide

**Method:** shadow technicians for one shift at the station, in their language. Ask about the *last* job, not hypotheticals, and ask to see their WhatsApp group and paper card. Sample: 5–6 technicians, 2–3 managers, 6–8 riders at the hub.

### Technician
| Ask | Likely answer | What it tells you |
|---|---|---|
| Walk me through the last scooter you fixed. | "Battery issue. I sent a photo to the group, then waited for the controller." | Real steps vs the 6 official statuses |
| When do you fill the job card? | "End of the day, from memory." | Back-filling, so timestamps can't be trusted |
| What happens when a part isn't there? | "I tell sir, start another bike, and forget the first one." | "Waiting for part" needs its own status that alerts the manager |
| Have you been blamed for a delay that wasn't yours? | "Yes, the bike was waiting 2 days for a part." | Accountability that protects the technician |
| Do you send voice notes on WhatsApp? Type? | "Voice notes. Typing in Kannada is slow." | Voice works for notes, not for controlling the app |
| Whose phone is it? | "The station phone. Everyone uses it." | Quick user switching, per-user language |

### Service manager
| Ask | Likely answer | What it tells you |
|---|---|---|
| How do you know a job is stuck? | "When the rider calls me." | Alerts on job age by reason |
| Last cost you didn't trust? | "Two brake pads billed, one used." | Parts picked from a catalog plus photo evidence |
| What delays an invoice? | "Missing part costs. I chase technicians on WhatsApp." | Required fields before "Ready for pickup" |
| What do you do first each morning? | "Scroll 5 WhatsApp groups." | An exceptions-first dashboard |

### Rider
| Ask | Likely answer | What it tells you |
|---|---|---|
| Last time your scooter was in for repair: what did it cost you? | "A full day, about ₹800–1,000. Missed my weekly bonus." | Value of an ETA or a replacement scooter |
| What did you want to know while waiting? | "When will it be ready? Do I get another bike?" | ETA plus replacement status |
| Ever charged for damage you disagreed with? | "Yes. No photo, nothing." | Before and after photos shared with the rider |

---

## 4. Numbers each audience moves and decisions they make

| Who | Records or acts on | Decision it drives |
|---|---|---|
| Technician | Status changes (system-timestamped), blocker reason, parts (item, qty, unit cost), labour estimate vs final, photos, QC pass/fail | Which job to do next, when to ask for help |
| Manager | Job aging by status, waiting-on-parts count, estimate vs actual variance, QC fail / comeback rate, ready → invoiced lag | Reassign, expedite a part, approve a cost overrun, escalate, invoice |
| Rider | Ready-by time, replacement scooter | Plan the day's shifts, take a replacement |

Benchmarks to borrow:
- Age buckets of under 24 h / 24–48 h / over 48 h ([RTA Fleet360](https://docs.rtafleet.com/fleet360-articles-table-of-contents/home-menu-table-of-contents/dashboard-menu-table-of-contents/main-dashboard))
- Comeback rate under 3% ([Oxmaint](https://oxmaint.com/industries/fleet-management/technician-comeback-tracking-kpi))
- First-time fix rate of about 88% for best performers ([PTC/Aberdeen](https://www.ptc.com/en/blogs/service/what-is-first-time-fix-rate))

---

## 5. Who sees what

| Data | Technician | Manager | Rider |
|---|---|---|---|
| Status plus time in status | ✅ own jobs | ✅ all stations | ✅ simplified |
| Blocker reason ("waiting for part") | ✅ | ✅ alert | ✅ "delayed: part" plus new ETA |
| Ready-by time | ✅ | ✅ | ✅ on WhatsApp |
| Parts and labour cost | ✅ | ✅ with variance flags | ❌ unless chargeable to the rider |
| Intake and completion photos | ✅ | ✅ | ✅ when damage is charged |
| Edit history | ✅ own | ✅ | ❌ |

**Rule:** the rider sees *time*, the manager sees *exceptions*, and the technician sees *what's next*.

---

## 6. Accountability without surveillance

Monitoring workers raises stress and doesn't improve performance ([Microsoft Research meta-analysis](https://microsoft.com/research/publication/a-meta-analysis-of-the-effects-of-digital-surveillance-of-workers-a-psychology-focused-approach)). Indian workers have protested punitive tracking, such as GPS watches for Chandigarh sanitation workers ([Undark](https://undark.org/2022/05/02/in-india-digital-snooping-on-sanitation-workers/)). So collect **evidence per job, not tracking per person**:

1. **The system stamps the time.** The app records time at each status tap, so there's no time field to type into and nothing to back-fill.
2. **Photos are the gate.** No "Work started" without intake photos, and no "Ready" without completion photos. Photos come from the live camera only, with a timestamp watermark.
3. **Parts come from the catalog,** with price master unit costs. A quantity or cost above the estimate by more than X% asks for a reason.
4. **Blockers are protected states.** "Waiting for part / technician / approval" pauses the technician's clock and alerts the manager. This works like Toyota's andon: a call for help, not an admission of blame ([IndustryWeek](https://www.industryweek.com/operations/continuous-improvement/article/55394935/andon-is-a-signalbut-leaderships-response-is-the-critical-part)).
5. **A different person does QC** (maker-checker), which is already a dealership norm.
6. **Edits stay visible.** Nothing is deleted, and changes show who and when.
7. **Technicians see their own data and can dispute it.** Use team metrics, not public leaderboards, which breed envy ([JYX](https://jyx.jyu.fi/bitstreams/eca824f1-c9a6-464e-89e3-c2d244dd19c5/download)).

---

## 7. Voice module: is "Wispr Flow for technicians" right?

**Partly.** Voice is good for greasy hands, but a Wispr Flow-style module is the wrong model.

**Why not Wispr Flow itself:**
- Cloud-only, with no offline mode ([Wikipedia](https://en.wikipedia.org/wiki/Wispr_Flow)).
- No stated support for Kannada, Tamil or Telugu. It does support Hinglish ([9to5Google](https://9to5google.com/?p=705136)).
- Its API is approval-only and returns *polished prose*, not structured fields ([Scalekit](https://www.scalekit.com/blog/wispr-flow-mcp-vs-api)).
- Polished prose is a liability on a job card, where "2" versus "12" brake pads matters.
- Licensed per user, which doesn't suit shared phones.

**Speech-to-text accuracy on real code-mixed Indian speech** ([Josh Talks / AI4Bharat](https://elevenlabsreport.ai.joshtalks.com/)), as word error rate (lower is better):

| Model | Hindi | Kannada | Tamil | Telugu |
|---|---|---|---|---|
| **Sarvam Saaras v3** | **3.8%** | **8.8%** | **9.1%** | **13.5%** |
| Amazon Transcribe | 4.9 | 11.1 | 12.5 | 14.1 |
| OpenAI Whisper (realtime) | 10.4 | 32.9 | 23.6 | 30.0 |
| Deepgram Nova-3 | 9.5 | 51.1 | 66.9 | 42.7 |

- South Indian languages show 2–4× more errors than Hindi.
- Holding the phone close to the mouth adds about 30 dB of signal over workshop noise ([USPTO](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12445761)). Nearby voices are the hardest noise to filter ([arXiv](https://arxiv.org/pdf/2312.13873)).
- Users with less than 8th-grade schooling did *better with keypads than speech* ([Patel et al., CHI 2009](https://hci.stanford.edu/publications/2009/chi2009_patel.pdf)). **Voice works for content; taps work for control.**
- Cost for 50 technicians × 10 jobs × 2 min is about ₹13k/month on Sarvam's documented rate of ₹30/hour ([Sarvam pricing](https://docs.sarvam.ai/api-reference-docs/pricing)).

**Recommended design:**
1. **Hold-to-talk** button, thumb-sized or bigger, with a volume-key alternative. No wake word.
2. **Record locally, upload when online.** Transcribe with Sarvam, biased toward a parts vocabulary of up to 50 key terms.
3. **Extract to fields:** part (matched to the catalog), quantity and blocker reason. Show these as **editable chips that need a confirm tap**. Nothing is written into the job card without that tap.
4. **Keep the audio** as a WhatsApp-style voice note for the manager to listen to.
5. **Keep these on taps:** status changes, quantity steppers, frequent parts, blocker icons and sign-off.

Before committing, record about 200 real utterances per language in the actual workshop and measure errors on part names and numbers.

---

## 8. Workshop-floor design rules

- Touch targets: 15 mm or larger for primary actions, about 20 mm for submit and close. Actions go in the bottom third of the screen. No pinch or long-press ([W3C summary](https://www.w3.org/WAI/GL/mobile-a11y-tf/wiki/Summary_of_Research_on_Touch/Pointer_Target_Size)).
- Contrast of at least 7:1. Sunlight can cut effective contrast to about 1.2–3:1 ([GSMArena](https://www.gsmarena.com/gsmarena_labs_announces_sunlit_legibility_display_test-news-4105.php)).
- Test on a ₹7k phone: 600-nit LCD, 3–4 GB RAM, Android 11 or later ([91mobiles](https://www.91mobiles.com/xiaomi-redmi-a5-price-in-india)).
- Save locally first and sync later. Show WhatsApp-style status: 🕓 saved on phone, ✓ uploaded, ✓✓ seen ([Android offline-first](https://developer.android.com/topic/architecture/data-layer/offline-first)).
- Photos: resumable uploads, compressed. Check free storage first, since 62% of users run out of space every 3 months ([Eastern Mirror](https://www.easternmirrornagaland.com/62-indians-run-out-of-smartphone-space-every-three-months)).
- Icon plus native-language label on every action. Western digits for numbers. Leave about 40% room for text expansion (Tamil runs longer).
- Home screen readable in a 4-second glance, because phone attention spans drop to a few seconds in the field ([Oulasvirta, CHI 2005](https://www.interruptions.net/literature/Oulasvirta-CHI05-p919-oulasvirta.pdf)). Resume exactly where the technician left off.
- Shared phone: avatar plus 4-digit PIN switching, with language set per user.

---

## 9. How to test it, and the number that matters

- **Week 1:** clickable prototype on the floor with 5 technicians doing their real jobs. Measure time to log a part (target under 10 s) and voice confirm accuracy.
- **Weeks 2–3:** pilot at one station, compared against a paper station.
- **North-star metric: share of status changes logged *at the time of the event*, not back-filled.** Target over 80%.
- **Supporting metrics:**
  - Ready → invoice lag, target under 24 h
  - Waiting time with a reason code, target 100%
  - Cost disputes per 100 jobs
  - Rider "where's my scooter" calls

---

## 10. Questions to ask Blive

1. Does rider rent pause while the scooter is in the workshop? Is a replacement scooter offered?
2. Can the IoT telemetry (battery, odometer, fault codes) pre-fill the intake?
3. Is there a parts catalog or price master? Who approves overruns?
4. How many technicians are on each station phone? Which languages, per station?
5. Who does QC: a technician or a supervisor?

*Gaps: Blive's uptime, hub count, deposit policy and parts pilferage data are not public. Many repair-industry stats are vendor claims.*
