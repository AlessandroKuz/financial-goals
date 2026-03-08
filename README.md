# Financial Goals

Index: 
1. [Overview](#overview)
2. [Specs](#spec-sheet)
3. [Models](#models)
4. [MVP](#mvp)
4. [Guide](#guide)

## Overview

The following project is supposed to be a Web App to keep track of one financial status and more importantly their goals and progress.

The main focus is to provide an easy and nice to use way to keep track of ones financial status by setting and **leveraging goals**,
*like saving for a Car or House*, using them as motivation for the future, allowing to realise what you have accomplished and so on.

It is planned to also have a dedicated section with **Stats** both for "lifetime" (when you signed up) and selected periods (weekly, monthly, annually, ...).

## Spec sheet

- A way to keep track of "total money" - Net worth
  - Money + (Estimated possessions - either global amount or detailed one - custom labels)
  - Probably should avoid "spending accounts" - if you have 1k that you know you will spend by the end of the month, they shouldn't count towards net worth
  - Bank account 1
  - Bank account 2+
  - Savings (Probably should be a "check-mark" to each account)
  - Estimated investments
    - Starting investments
    - Estimated actual value
    - For now lets treat all investments as a single big one
      - In the future lets track the "category" (stock, crypto, ...) and details (which company/crypto, ...)
    - For now lets pretend I never sell / sold
      - In the future lets add a way to make it more granular and add a way to track "profit" (selling price - starting price - (taxes? - manual input))
  - Money allocation pool
    - A separate place where you allocate money to reach your goals
  - Loaned money (In or our)
    - Debt (+ progress bar, you could either grow your debt and start paying it off) - **Loan IN**
    - Loans - **Loan OUT**
      - A date when you expect your money (a reminder/notification when the day is close)
      - A way to write off a loan (either because you got paid off or because you decided its not worth it anymore)

- [FUTURE] Non Wealth building money goals (Trips, Gifts, ...) - Find a way to handle them too

- [FUTURE] Budgets, ...

- Aggregated Stats + Graphs for each account:
  - For example, how much money you have saved up
    - Globally or by a certain period
    - Graphs, tables & main numbers
  - Net worth over time (keep in mind it could grow and ALSO go down)

- A way to track financial objectives
  - Static & dynamic ones:
    - Static: "One time purchases" and "Current possessions" and "Others"
      - One time purchases: VR, PC, Steering wheel, Car, Home, ...
        - Global categories (Car, Home, ...)
        - Custom Details (VR, PC and Steering Wheel are not something Everybody wants to have)
      - Track the first time you made the purchase (date)
      - Current possessions (You might have a car now, but sell it in the future and not have it anymore, for any reason)
    - Dynamic: "Reach x amount of money in y category"
      - 1, 3, 6, 12 months of Savings
      - 10k in Savings
      - X k in investments
  - Here too, both global and custom goals should be supported

- A Simple "Standard Financial Goals" Roadmap
  - Each section should also have an explanation section
  - The Roadmap should be used as a guide, not as a pre-requisites list, each situation is different, but a general guideline is always useful to have,
  also the steps are pretty reasonable
  0. Have some sort of housing:
    - This is the basic step of all, research proves that having a stable housing situation is the key to everything in a persons life - That also includes
    the personal finance of somebody
  1. Have some sort of stable income - keep working on it with time...
    - If you are still underage or live with somebody (parents, family, friends, ...) the situation might be slightly different/harder,
    but the first step for one self-confidence is having financial freedom to make your own decisions.
    - Said frankly, if you don't have money and a lot of free time, you have to use (at least some of) the free time [to provide value and be paid](#guide).
  2. Start a separate Savings account
    - Keeping your savings account separate from your "spending" account help to prevent "over-spending" and building the concept that Savings money shouldn't be
    touched unless really necessary, like an emergency or to achieve a financial goal.
  3. Have 1 month of Savings
    - To calculate how much is that, you have to remove all auxiliary expenses and keep only there necessary ones, the ones that you can't live without or that
    will severely hinder your life
  4. Start paying of the smaller debts
  5. Have 3 months of Savings
  6. Have 6 months of Savings
  4. Pay off your other debts (mortgage excluded)
  7. (Have 12 months of Savings)
    - This is optional but very recommended, if not now it is advised to be done between starting investing and having 5k in investments
  8. Make you first Investment
    - It's a good idea to "put" your money to work, not only to work yourself to earn them
  9. Have 1k in investments
  10. Have 10/20k in Savings
    - if your 12 month of savings are worth more than 10k, you should consider the next "round number" step-up after your saved amount, being that 15k or 20k
    if your 12 months of savings are worth more than 20k there *might* be something wrong, maybe you should redefine what is necessary, or maybe think about
    moving to a cheaper place/area (at least while you are still building up your wealth), or maybe you just have a lot of people depending on you, but still
    *be sure that your expenses are truly essential*.
  11. Have 5k in investments
  12. (Have a Mortgage on a house)
  13. Have 10+k in investments
  14. Have a transportation vehicle (Car / Bike / Scooter, ...)
  15. Buy a House / Finish paying your mortgage
  16. Invest in other opportunities
  17. Give back to the community, help others, ...
    - Invest in what you like, get help from a licensed professional, but be sure to invest either in something that you know will likely not fail
    (so your money isn't just wasted)

- Have a progress bar for each goal
  - Each financial goal could have an "Estimated Price" and therefore an associated progress-bar

- User authentication - Each user (naturally) has his own accounts and money

- [FUTURE] Could have a "Partner" to contribute to "Shared" Goals (house, car, ...)

## Models

1. Money Account/Pool
  - Could be a bank account, hard cash, ...
  - Could be of different categories:
    - Savings
    - Investment
    - Goals Allocation pool
  - A basic Transaction History
    - A way to add and remove money
    - [FUTURE] At this point, should I also add a way to track the "main account" (where the salary and main expenses live)
      - Income and Spending categories
        - Macro categories (Income and Outcome)
        - Micro categories (Health, Electronics, ...)

## MVP

### Iteration 1 - First work on goals

- [ ] Start Django project + apps
- [ ] Define basic models
  - [ ] Basic Accounts
- [ ] Define the main sections
  - [ ] Net worth - Accounts (Savings, Investments, Allocation pool) + Debt (In & Out)
    - Sub-sections:
      - [ ] Savings
      - [ ] Investments
      - [ ] Allocation pool
      - [ ] Debt (IN)
      - [ ] Loans (OUT)
  - [ ] Stats
    - A simple main numbers page
  - [ ] Objectives
    - [ ] General / Guide
    - [ ] Personal

### Iteration 2 - Work on the details

- [ ] Define better models
- [ ] Define better models
  - [ ] Advanced Accounts...

### Iteration 3 - ...

- [ ] Define "final" models
  - [ ] Accounts...
  - [ ] Sections
    - [ ] Budget

## Guide

General principles:

- To earn money you have to provide value to other people
- To provide value you could either sell your:
  - Time (which you can always do)
  - Knowledge and/or Experience (which you need to acquire first)

### AI Response - Perplexity

[Link to the chat](https://www.perplexity.ai/search/what-are-all-the-ways-to-make-1usUfmlCScCJlgWWc_2pRA?sm=d).

Making money fundamentally involves exchanging value with others, such as your time, skills, knowledge, or assets, for compensation. This can happen through active effort, scalable creation, or leveraged investments.

**Core Ways to Provide Value**
- Sell your time: Trade hours directly for pay via jobs, freelancing, consulting, or gigs like driving, tutoring, or virtual assistance.
- Sell your knowledge/experience: Package expertise into services (coaching, courses), content (blogs, videos, ebooks), or advice (online tutoring).
- Sell your creativity/skills: Offer tangible outputs like writing, design, coding, art, music, or handmade goods through freelancing or marketplaces.
- Solve problems: Create targeted solutions, such as software tools, apps, research services, or efficiency hacks for specific pain points.

**Scalable and Passive Methods**
- Build products/services: Develop digital goods (apps, templates, printables), physical items (e-commerce), or memberships that sell repeatedly with low ongoing effort.
- Invest assets: Use money to generate returns via stocks, real estate rentals, dividends, royalties from intellectual property, or peer-to-peer lending.
- Leverage audiences: Monetize followers through affiliate marketing, ads, sponsorships, or newsletters once you've built a platform.

**Comparison of Approaches**

| Approach | Effort Level | Scalability | Startup Needs | Examples |
| -------- | ------------ | ----------- | ------------- | -------- |
| Time-based | High (ongoing) | Low | Low (skills only) | Job, rideshare, freelancing |
| Knowledge-based | Medium | Medium | Medium (platform) | Courses, coaching |
| Product-based | High upfront | High | Medium (creation tools) | Apps, ebooks |
| Investment-based | Low ongoing | High | High (capital) | Rentals, dividends |

Focus on ethical value creation to build sustainable income, as it leads to referrals and repeat business.

