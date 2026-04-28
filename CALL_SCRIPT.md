# 📞 Gold Hands Membership — Call Script (v2, 2026-04-28)

> Source of truth for plan benefits: `index.html` pricing section.
> Last sync: 2026-04-28 (matches live site at mybotbestagent-maker.github.io/gold-hands-membership/).

---

## [OPENING]

> *"Hey [Name]! This is [name] from Gold Hands. We did some work at your place — everything still good at home?"*

> *[Wait for answer]*

> *"Glad to hear. Hey, I'm calling because we just launched something new — only for clients who've already worked with us. Want to take 2 minutes? You'll like it."*

---

## [WHAT IS THE MEMBERSHIP]

> *"We launched a monthly membership for home maintenance — you become one of our regular clients and get benefits regular customers never see. Three plans: Bronze, Silver, Gold. Want me to walk you through them?"*

> *[Wait for "yes"]*

---

## [PLANS — WHAT'S INCLUDED]

> *"Alright, here's the breakdown.*

### **Bronze — $49/mo (or $540/yr — saves you 8%)**
> *One visit per quarter — a tech comes out for 60 minutes, checks plumbing, electrical, doors, windows. 10% off all labor. 24-hour priority response if something breaks. 1-year warranty on every job. And a $5,000 Gold Hands Guarantee — if we damage anything in your home, we cover it. Total annual value of $890, you pay $588 — you save $302. Good if your home's in shape and you just want to stay connected."*

### **Silver — $99/mo (or $1,090/yr — saves 8%) — MOST POPULAR**
> *Tech visits every month — 60 minutes plus small fixes done on the spot. The big one: **your dedicated handyman** — same pro every time, learns your home. 15% off all labor. 12-hour response. Free full-home audit when you sign up. 3-year warranty on all work, $25,000 Gold Hands Guarantee. Plus one emergency visit per quarter — included, no extra charge. Annual value $1,990, you pay $1,188 — saves $802."*

### **Gold — $199/mo (or $2,190/yr — saves 8%)**
> *Two tech visits a month. Dedicated handyman plus a backup so we never miss you. 20% off everything. **4-hour emergency response** — fastest in the industry. $100 service credit every month — applies to any job we do. 5-year warranty, $50,000 Gold Hands Guarantee. Family sharing — covers up to 2 properties (perfect if you've got a rental). VIP 24/7 support line. Annual value $3,780, you pay $2,388 — saves $1,392."*

---

## [CLOSE]

> *"Most clients pick Silver — it's the sweet spot. But it's your call. Which one fits you best?"*

> *[STAY SILENT. Wait for them to choose.]*

---

## [OBJECTIONS]

### "It's too expensive"
> *"I hear you. Look — you've already spent $[CRM amount] with us. With Silver you save 15% on every future job, plus the monthly visit is included. Your last $200 invoice would have been $170. The plan pays for itself after one or two calls. And we've got a 30-day money-back guarantee — try it, don't like it, full refund, no questions. Want me to set you up?"*

### "I don't need it that often"
> *"Then Bronze is your option. $49/mo, one quarterly visit, 10% off when you do call us. Plus the $5,000 guarantee fund kicks in on any job — you get the protection without the heavy use."*

### "What's the tech actually doing every month?"
> *"He runs through your home — checks plumbing, electrical, smoke detectors, water heater, doors, windows, anything that can wear down. Small fixes happen right there during the visit. It's like a tune-up for your home — way cheaper than a $5,000 emergency call later."*

### "I need to think about it"
> *"No problem. I'll text you the link right now — everything's laid out by plan. Mind if I follow up Thursday — morning or afternoon better?"*

### "I already have my own handyman"
> *"Totally fair. We're not replacing anyone. But here's the thing — we've already worked in your home, we know your setup. That's a different level of trust than starting fresh. With Bronze ($49/mo) you keep us as your second line — and use the 10% discount + the $5K guarantee fund any time. Try it for one month?"*

### "I don't want a contract"
> *"Zero contract. Month-to-month. Cancel anytime — one text. No penalties, no calls to retain you."*

### "Why is yours more expensive than [Mr. Handyman / Monty's]?"
> *"Couple reasons. We give you 12 visits a year on Silver — they give you 6. Multi-year warranty (theirs is 90 days). $25,000 damage guarantee fund (they don't have one). And your dedicated handyman every time — they rotate techs. So per visit we're actually cheaper, and the guarantee means you sleep better at night."*

### "Can I use it for my rental too?"
> *"On Bronze and Silver, one property. On Gold — family sharing covers up to 2 properties. So if you've got a rental + your home, Gold actually saves you a lot of headache."*

---

## [FINAL CLOSE]

> *"Here's what I'd do — try Silver for one month. If it's not a fit, we refund 100%. Should I send you the link to set it up right now?"*

> *[STAY SILENT.]*

---

## [POST-CALL SMS — within 60 seconds]

```
Hey [Name]! [name] from Gold Hands here. As promised — your membership link:
https://mybotbestagent-maker.github.io/gold-hands-membership/#pricing

🥉 Bronze $49/mo — quarterly visit · 10% off · $5K guarantee fund
🥈 Silver $99/mo — monthly visit · dedicated handyman · 15% off · $25K guarantee · 1 emergency/quarter
🥇 Gold $199/mo — 2 visits/mo · 20% off · $100 monthly credit · 4-hr emergency · $50K guarantee · 2 properties

Annual plans save 8%. 30-day money-back. Cancel anytime.
Questions? Just text me back.
```

---

## [INTERNAL NOTES — for the rep]

- **Source of truth for benefits**: `index.html` pricing section (lines 1035–1130). If anything changes there, this script must update too.
- **Stripe Payment Links**:
  - Bronze monthly: `buy.stripe.com/7sY8wP27i3MV0sJeab9sk0P`
  - Silver monthly: `buy.stripe.com/eVq6oHbHS5V35N3d679sk0Q`
  - Gold monthly: `buy.stripe.com/9B67sLh2c83bgrH9TV9sk0R`
  - Annual versions: append `8x26oH...0Y` (Bronze), `dRmaEX...0Z` (Silver), `7sY4gz...10` (Gold)
- **CRM Pull (before call)**: client name, last service date, total spent, any open complaints
- **Goal close rate**: 25% on first call (after 1 prior service done)
- **If they choose**: send the *plan-specific* Stripe link, not the general site URL — drop-off is 3× lower
