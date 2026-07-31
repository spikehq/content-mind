# Angles Log

Tracks concepts and angles used in emails. Skip both draft and sent angles when suggesting ideas — drafts are reserved until sent or rejected.
Same blog or concept can be reused — but the angle must be different.

---

## Drafts

### Why a month is too long to be on-call
- **Blog:** https://spike.sh/blog/why-a-month-is-too-long-to-be-oncall/
- **Angle:** Low incident volume tempts teams into longer rotations, but that's counterintuitive. The real cost isn't how often incidents fire — it's the mental burden of staying ready for 30 days straight.
- **Subject used:** Why a month is too long to be on-call
- **Date:** 2026-07-31

---

## Sent

### Severity-priority matrix
- **Blog:** https://spike.sh/blog/severity-and-priority-based-routing/
- **Angle:** Severity alone isn't enough to route incidents. A low-severity incident for a high-priority customer still needs an immediate response. Routing needs to account for both severity and priority — the matrix maps every combination to a defined response.
- **Subject used:** Severity alone isn't enough to route incidents.
- **Date:** 2026-07-31

---

### Midnight incidents
- **Blog:** https://spike.sh/blog/how-to-handle-midnight-incidents/
- **Angle:** One escalation policy running around the clock treats a midnight incident the same as a noon incident. The fix is two policies — one for office hours (Slack to the team), one for off-hours (direct call to on-call engineer, then backup if no response in 5 minutes). An alert routing rule connects them by checking when the incident triggered and routing to the right policy.
- **Subject used:** A midnight incident should wake one person.
- **Date:** 2026-07-23

---

### Dedicated escalation policy for low-priority incidents
- **Blog:** https://spike.sh/blog/escalation-policy-for-low-priority-incidents/
- **Angle:** Low-priority incidents don't have the same escalation flow as critical ones — a single Slack notification goes out and if nobody responds, nothing follows. A dedicated policy with longer wait times and follow-up steps keeps them moving.
- **Subject used:** Low-priority incidents need a dedicated escalation policy.
- **Date:** 2026-07-02

---

### On-call handoff best practices
- **Blog:** https://spike.sh/blog/oncall-handoff-best-practices/
- **Angle:** A 15-minute conversation before shift changes saves hours of piecing things together. Three questions cover most of it — what to watch, how busy the shift will be, and who to loop in if things escalate.
- **Subject used:** What does a proper on-call handoff look like?
- **Date:** 2026-06-11

---

### Setting up alerts for a new service
- **Blog:** https://spike.sh/blog/setting-up-alerts-for-a-new-service/
- **Angle:** When launching a new service, you don't know what normal looks like yet. Start with low thresholds, treat every early incident as data, and calibrate thresholds after a few weeks of observation.
- **Subject used:** How to get alerts right for a new service?
- **Date:** 2026-06-04

---

### Frequent escalations as an on-call burnout sign
- **Blog:** https://spike.sh/blog/oncall-burnout-signs/
- **Angle:** When engineers escalate more often, it's easy to assume a skill gap — but it's usually alert noise draining their mental bandwidth. Reducing noise gives them their mental space back.
- **Subject used:** Are your on-call responders escalating often?
- **Date:** 2026-05-28

---

### Automating repeated routing decisions
- **Blog:** https://spike.sh/blog/turning-team-knowledge-into-alert-routing-rules/
- **Angle:** If your team keeps making the same manual decision for the same kind of incident, that decision belongs in a routing rule. Four sources help you find these patterns.
- **Subject used:** Let routing rules handle the obvious
- **Date:** 2026-05-21

---

### Critical incident escalation policy
- **Blog:** https://spike.sh/blog/escalation-policy-for-critical-incidents/
- **Angle:** Default escalation policies are too slow for critical incidents. Critical incidents need a different first step — a single phone call to the entire engineering team at once, not a sequential chain.
- **Subject used:** Default escalation policy isn't built for critical incidents
- **Date:** 2026-05-07

---

### Follow-the-work on-call rotation
- **Blog:** https://spike.sh/blog/follow-the-sun-and-other-oncall-models/
- **Angle:** The engineer who shipped a feature should be the first responder for incidents tied to that deploy, for a short window (48 hours to a week). Reduces MTTR because the edge cases are still fresh in their mind.
- **Subject used:** Your on-call is probably paging the wrong person.
- **Date:** 2026-04-30

---

### Payload-based routing
- **Blog:** https://spike.sh/blog/alert-routing-based-on-incident-payload/
- **Angle:** Some incidents should skip the default escalation policy entirely and route straight to the right team based on what the incident payload says. Payload-based routing is one of three conditions routing rules can act on.
- **Subject used:** Which incidents should skip the default escalation policy?
- **Date:** 2026-04-23

---

### Two escalation policies to start
- **Blog:** https://spike.sh/blog/compass-for-setting-up-escalation-policy/
- **Angle:** You only need two escalation policies at the start — one for critical incidents (phone call, short wait times) and one for everything else (Slack message). Add more as incident patterns emerge.
- **Subject used:** How many escalation policies do you need?
- **Date:** 2026-04-16

---

### Quiet Day on-call rotation
- **Blog:** https://spike.sh/blog/offbeat-oncall-rotations/
- **Angle:** Designating one day a week with zero on-call coverage as protected focus time. Started as a two-month experiment for one team, now standard practice.
- **Subject used:** What if no one is on-call for an entire day?
- **Date:** 2026-04-09
