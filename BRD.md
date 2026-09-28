# GymAnywhere MVP: Business Requirements Document

Logic Lumin Software · Prepared by Basava Sanketh B N (Business Analyst) · Version 1.0, January 2026

See also: [FRD](FRD.md) · [Project overview](README.md)

### Revision history

| Version | Date | Change |
| --- | --- | --- |
| 0.1 | Jan 2026 | First draft after interviews with the founders and gym owners |
| 0.2 | Jan 2026 | Updated scope after engineering review. Loyalty and class booking moved to phase 2 |
| 1.0 | Jan 2026 | Signed off by both co-founders |

---

## 1. Summary

GymAnywhere lets people find a gym in Mysuru, pay for a single visit or a pack of visits and check in with a QR code. For gyms, it brings in new members and replaces the paper attendance register.

This document covers the MVP only. We have 12 weeks and 4 partner gyms, so the scope is kept to three flows: finding and booking a gym, checking in and getting new gyms onboarded.

## 2. Background

People in Mysuru don't have an easy way to compare gyms. Most of it is word of mouth. Nearly every gym asks for a monthly or yearly membership up front. From our user interviews, the most common reason people gave for not joining a gym was not wanting to commit before trying it.

Gyms have the opposite problem. New members come in slowly through walk-ins and referrals. Attendance is written in a register, so owners can't easily tell how busy they are, which hours are packed or whether people are coming back.

We think a pay-per-visit app can help both sides. Starting with one city lets us test whether people will actually pay this way before we spend money on expansion.

## 3. Goals

| # | Goal | How we'll know |
| --- | --- | --- |
| G1 | Launch on time | MVP live in Mysuru within 12 weeks |
| G2 | Get gyms on board | 4 partner gyms live for the pilot |
| G3 | Show that people will pay | ₹3L in bookings in the first quarter |
| G4 | Get rid of paper check-in | Check-in at least 50% faster than the register |
| G5 | Make onboarding repeatable | A new gym goes live in under a week |
| G6 | Give the founders data for the expansion decision | Weekly KPI report running from launch week |

## 4. Scope

**In the MVP**

- Sign-up, gym search and gym profiles (Mysuru only)
- Single-visit and multi-visit passes with online payment
- QR check-in at the gym
- Partner onboarding and a simple partner dashboard
- Admin tools for our team to manage gyms, prices and payouts
- A weekly KPI report for the founders

**Not in the MVP (and why)**

- Loyalty points and a multi-gym pass. The founders were keen on this, but it needs pricing work with every gym. Parked for phase 2.
- Class schedules and trainer booking. Only 1 of the 4 gyms runs regular classes.
- Other cities. We want a quarter of data from Mysuru first.
- Reviews, ratings and chat. Nice to have, not needed to prove the model.
- Wearable integrations. Nobody asked for it in interviews.

## 5. Stakeholders

| Who | What they care about | How they're involved |
| --- | --- | --- |
| Co-founders (2) | Proving the model, keeping to budget | Sign off scope and priorities |
| Gym owners (4) | More members, less admin, getting paid on time | Interviews, UAT, onboarding |
| Front-desk staff | A check-in that doesn't slow them down | UAT and training |
| Prospective members (50+ interviewed) | Finding a good gym and not overpaying | Interviews and usability feedback |
| Engineering team | Clear requirements they can build | Feasibility review, sprint planning |
| Me (BA) | Requirements that are clear and traceable | Own the BRD, FRD, backlog and UAT |

## 6. How things work today vs with GymAnywhere

| | Today | With GymAnywhere |
| --- | --- | --- |
| Finding a gym | Ask friends or walk in | Search and compare in one app |
| Paying | Monthly or yearly, at the counter | Per visit or a pack of visits, online |
| Checking in | Name written in a register | Show a QR code, staff scan it |
| Knowing footfall | Guesswork | Live check-in data |
| Onboarding a gym | No set process | A 5-step checklist |
| Reporting to founders | None | Weekly KPI sheet |

## 7. Business requirements

Priorities use MoSCoW (Must, Should, Could, Won't).

| ID | Requirement | Priority | Goal |
| --- | --- | --- | --- |
| BR-01 | Members can find partner gyms by area, price and facilities. | Must | G3 |
| BR-02 | Members can buy a single-visit or multi-visit pass and pay online. | Must | G3 |
| BR-03 | Gym staff can confirm a booking at the front desk in a few seconds without paper. | Must | G4 |
| BR-04 | Every check-in is recorded and visible to the gym and to us straight away. | Must | G4, G6 |
| BR-05 | We can onboard a new gym through a set process in under a week. | Must | G2, G5 |
| BR-06 | Gyms can see their bookings, check-ins and earnings. | Must | G2 |
| BR-07 | We can work out and pay each gym's share correctly. | Must | G2 |
| BR-08 | Gyms can limit how many people book each slot. | Should | G2 |
| BR-09 | The founders get weekly numbers on bookings, revenue per gym and repeat bookings. | Must | G6 |
| BR-10 | Members can cancel a booking within a set time. | Should | G3 |
| BR-11 | Members get a reminder before their visit. | Could | G3 |
| BR-12 | Loyalty or a multi-gym pass. | Won't (phase 2) | |

The [FRD](FRD.md) breaks each of these down into functional requirements.

## 8. What we'll track

| Metric | How it's worked out | Why we care |
| --- | --- | --- |
| Bookings | Paid bookings per week, per gym | Are people using it at all? |
| Booking-to-visit rate | Check-ins divided by bookings | Do bookings turn into actual visits? |
| Revenue per gym | Booking value per gym per week | Spots gyms that aren't getting traction |
| Repeat-booking rate | Members with 2 or more bookings divided by all members who booked | Our best early sign that people are sticking around |
| Check-in time | Time from arriving to getting in | Is the QR actually faster than the register? |
| Time to onboard | Days from signed agreement to live listing | Is onboarding repeatable? |

## 9. Assumptions, constraints and dependencies

**We're assuming that**

- People in Mysuru will pay per visit if the price feels fair next to a monthly membership.
- Each gym has a phone or tablet with internet at the front desk.
- Gyms are fine with a revenue share on bookings that come through us.

**We're working within**

- 12 weeks for the MVP
- A small engineering team and no dedicated ops person at launch
- One city

**We depend on**

- The payment gateway for payments and payouts
- Signed agreements with all 4 gyms before launch
- Google Analytics being set up before go-live

## 10. Risks

| Risk | Impact | Chance | What we'll do about it |
| --- | --- | --- | --- |
| Front-desk staff don't take to the scanner | High | Medium | Keep it to one screen, train staff on site and have me at the gyms for the first two weeks |
| Not enough demand in a smaller city | High | Medium | Test pricing in 50+ interviews before building and watch bookings weekly |
| Scope creep delays the launch | High | High | Agree the MoSCoW list with the founders and keep a phase 2 list for everything else |
| Overbooking at peak hours annoys gyms | Medium | Medium | Let gyms set slot limits (BR-08) |
| Payout mistakes | High | Low | Calculate earnings automatically and reconcile every week |

## 11. Open questions at sign-off

- What revenue share do we offer gyms that join after the pilot? (Founders to decide before expansion.)
- Do multi-visit passes expire? If so, after how long? (Agreed for MVP: 60 days. To revisit after the first quarter.)

## 12. Sign-off

| Name | Role | Status |
| --- | --- | --- |
| Co-founder 1 | Sponsor | Approved |
| Co-founder 2 | Sponsor | Approved |
| Engineering lead | Delivery | Reviewed |
| Basava Sanketh B N | Business Analyst | Author |
