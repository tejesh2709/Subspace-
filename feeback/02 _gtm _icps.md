# Feedback #2 — GTM & ICPs

## 🔴 Group Splitting Has a Cold-Start Problem Nobody Talks About

---

### (a) Observed

When you open the Groups / bill-splitting section on Subspace, you're prompted to invite friends to split costs. But there is:

- No pre-existing network of contacts already on Subspace
- No nudge showing "X of your contacts already use this"
- No frictionless way to onboard a friend in under 30 seconds
- No viral loop built into the splitting action itself

Compare this to **Splitwise** — the app's entire growth came from forced acquisition. When someone adds you to a group expense, you *have* to download Splitwise to settle. Every transaction is an acquisition event. Subspace has no equivalent mechanism.

---

### (b) Problem

**Who is the ICP here?**
Young urban Indians (22–32) sharing rent, OTT costs, or trip expenses — people splitting ₹5,000–₹50,000/month across 2–6 people.

**Why this is a GTM problem, not just a product problem:**

This exact ICP is already owned by Splitwise. Subspace is asking this user to:
1. Abandon an app their entire friend group already uses
2. Convince those friends to also switch
3. Do all this for a *secondary* feature in an app they downloaded for subscription savings

The GTM message compounds the problem — Subspace leads with "save on subscriptions." New users don't even know splitting exists until they're already inside the app. There's no external surface that communicates the splitting value prop.

**The cold-start trap:**
The feature is only valuable when your friends are on it. But nobody joins Subspace just for splitting. So the feature never reaches critical mass, and the network effect never kicks in.

---

### (c) Ship Instead

| Solution | What it does | Effort |
|---|---|---|
| **Shareable split link** | Works for non-users too; recipient downloads to settle = instant acquisition | Medium |
| **Flatmate-targeted GTM campaign** | "Split Netflix, Hotstar & rent — all in one place" — a message Splitwise cannot match | Low |
| **Social proof nudge on onboarding** | "3 of your contacts already save with Subspace" reduces cold-start anxiety | Low |

**Tradeoff to consider:** The shareable link approach requires building a lightweight web experience for non-users — some engineering effort. But it's the only mechanism that creates organic, transaction-driven acquisition. Without it, the splitting feature will always be a secondary feature that never compounds.

---

### ICP Mapping

| ICP Segment | Current Reach | Gap |
|---|---|---|
| Solo subscription savers | ✅ Well served | None — core product |
| Flatmates splitting rent + OTT | ⚠️ Partially served | Cold-start kills adoption |
| Trip groups splitting expenses | ❌ Underserved | No viral loop, Splitwise wins |
| Families sharing subscriptions | ⚠️ Partially served | Official group plans needed first |
