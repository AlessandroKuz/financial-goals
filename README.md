# Financial Goals

Index: 
1. [Specs](#spec-sheet)
2. [Models](#models)
3. [MVP](#mvp)

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

- [FUTURE] Budgets, ...

- Aggregated Stats + Graphs for each account:
  - For example, how much money you have saved up
    - Globally or by a certain period
    - Graphs, tables & main numbers

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
  1. Have some sort of stable income - keep working on it with time...
  2. Start a separate Savings account
  3. Have 1 month of Savings
  4. Start paying of the smaller debts
  5. Have 3 months of Savings
  6. Have 6 months of Savings
  4. Pay off your other debts (mortgage excluded)
  7. Have 12 months of Savings
  8. Make you first Investment
  9. Have 1k in investments
  10. Have 10k in Savings
  11. Have 5k in investments
  12. (Have a Mortgage on a house)
  13. Have 5k in investments
  14. Have a transportation vehicle (Car / Bike / Scooter, ...)
  15. Buy a House / Finish paying your mortgage

- Have a progress bar for each goal
  - Each financial goal could have an "Estimated Price" and therefore an associated progress-bar

- Could have a "Partner" to contribute to "Shared" Goals (house, car, ...)

## Model

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

