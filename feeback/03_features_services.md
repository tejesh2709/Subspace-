# Feedback #3 — Features / Services

## 🔴 Auto-Detection is the Hero Feature — But It's a Black Box

---

### (a) Observed

Subspace markets its auto-detection as:
> *"Automatically identifies and categorizes payments, subscriptions, and hidden costs — simply log in, and we'll take care of the rest, no manual input required."*

But when you actually use the app, there is:

- **No transparency** into which accounts or data sources it's reading
- **No permissions explanation** before or after granting access
- **No confidence score** or completeness indicator
- **No "did we miss anything?" prompt** after detection runs
- **No audit trail** showing detected vs. missed subscriptions
- **No way to verify** whether the list is complete or partial

The feature works silently — magic box in, magic box out.

---

### (b) Problem

Auto-detection is Subspace's biggest value hook and the primary reason a user downloads the app. But silent, invisible automation creates two serious problems:

**1. Trust gap**
If detection misses 2 of your 8 subscriptions, you believe you're fully covered — but you're not. You won't catch the miss because there's no audit trail. Users who feel misled by incomplete detection churn silently and leave negative reviews.

**2. Massive missed monetisation**
Every undetected subscription is a missed upsell opportunity. The Negotiate API — Subspace's core competitive moat — can only fire on subscriptions it knows about. If a user pays full price for Spotify because detection missed it, that's lost savings for the user and lost marketplace revenue for Subspace — a compounding loss as the user base scales.

Studies consistently show users underestimate their subscription spend by 2–3x. Detection completeness is the foundational layer that makes the entire business model work.

---

### (c) Ship Instead

| Solution | What it does | Effort |
|---|---|---|
| **Subscription Audit screen** | Post-detection checklist: "We found 5. Did we miss any?" with tap-to-add | Low |
| **Detection source label** | "Detected via UPI · Last charged 12 May" under each subscription | Low |
| **Savings Opportunity flag** | Full-price subscription detected → "Get this 75% cheaper → Save ₹450/month" | Medium |

**Priority:** The Savings Opportunity flag should ship first — it directly connects detection to the Negotiate API and creates an immediate monetisation loop.

**Tradeoff to consider:** More transparency about data sources (SMS, UPI, bank) may raise privacy concerns for some users. The solution is to explain *what* is being read and *why* — users who understand the value exchange are more likely to grant permissions, not less.
