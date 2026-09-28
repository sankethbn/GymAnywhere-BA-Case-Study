# GymAnywhere: Business Analyst Case Study

I joined Logic Lumin Software as a Business Analyst in January 2026, working remotely from Shimoga. GymAnywhere was the first product I took from a blank page to launch. This repo is my write-up of that project, along with the BRD and FRD I worked from.

- **Company:** Logic Lumin Software
- **Role:** Business Analyst (Jan 2026 to present)
- **Product:** GymAnywhere, an app to find, book and check in to gyms

## The short version

We shipped the MVP in 12 weeks with 4 partner gyms in Mysuru. In its first quarter it brought in ₹3L. The weekly numbers gave the founders enough confidence to plan a move into 2 more cities.

## The problem we were solving

If you live in Mysuru and want to join a gym, you mostly go by word of mouth. You can't compare prices or facilities in one place. Almost every gym wants a monthly or yearly membership before you've even tried it.

The gyms had their own headache. New members came from walk-ins and referrals, attendance went into a paper register and nobody really knew how busy the place was on a given day.

GymAnywhere was meant to fix both sides. Members could pay per visit and try different gyms. Gyms would get a steady stream of new people plus basic data on who was coming in.

## What I did

**Discovery.** I spoke with the 2 co-founders, all 4 gym owners and more than 50 people who might use the app. The gym owners all said the same thing in different words: footfall was unpredictable. Members mostly wanted to try a gym before paying for a month.

**Requirements.** I wrote the BRD in Confluence and broke it down into 15+ user stories in Jira. The founders wanted loyalty points and class booking at launch. I used MoSCoW to move those to phase 2, which kept us to three flows we could actually ship in a quarter: search, booking with payment and check-in.

**Process design.** I mapped the booking and check-in flows in Miro and worked with our designer on Figma wireframes. We then ran UAT at the gyms themselves. Swapping the paper register for a QR scan cut check-in time by about 70%. Every check-in now shows up in Google Analytics as it happens.

**Partner onboarding.** The first gym took close to 3 weeks to go live because nothing was written down. I turned what we learned into a 5-step SOP in Notion. After that, each gym went live in under a week.

**Reporting.** I built a weekly KPI dashboard in Google Sheets from SQL pulls. It tracks bookings, revenue per gym and how many members book again. The founders used it to make the call on expanding beyond the pilot.

## Documents

- [Business Requirements Document (BRD)](BRD.md): the why and the what. Problem, goals, scope, stakeholders, business requirements, KPIs and risks.
- [Functional Requirements Document (FRD)](FRD.md): the how. User roles, functional requirements, business rules, user stories with acceptance criteria and the UAT plan.

## Results

| What we measured | Result |
| --- | --- |
| Revenue in the first quarter | ₹3L |
| Partner gyms in the pilot | 4 |
| Delivery | 12-week roadmap, on time |
| Check-in time | About 70% faster than the paper register |
| Time to onboard a gym | From about 3 weeks to under 1 week |
| Next step | Expansion into 2 more cities approved |

## What I'd do differently

- I'd write the onboarding SOP before the first gym, not after it. Most of that first 3 weeks was us working out the steps as we went.
- I'd bring front-desk staff into the wireframe reviews earlier. They are the ones using the scanner fifty times a morning. Their feedback in UAT would have been cheaper to act on in week 3 than in week 10.
- I'd push harder for slot capacity limits in the first release. We marked it as a Should, but the busier gyms asked about it within days of going live.

## Tools I used

Jira and Confluence for the backlog and documents, Miro for process maps, Figma for wireframes, Notion for the onboarding SOP, Google Sheets with SQL for the KPI dashboard and Google Analytics for check-in data.
