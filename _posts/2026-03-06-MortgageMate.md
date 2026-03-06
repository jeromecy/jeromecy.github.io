---
layout: post
title: "Mortgage Mate: A Data-Driven Home Loan Simulator for Australian Buyers"
date: 2026-03-06
categories: [Apps, iOS, Finance]
tags: [mobile-app, mortgage, finance, statistics, Australia, home-loan]
description: "A data-driven personal finance simulator for Australian home buyers — built by a statistician, not a banker."
---

# Mortgage Mate 🏡

**A data-driven personal finance simulator for Australian home buyers.**

Most mortgage calculators give you a single number. Mortgage Mate gives you the full picture — statistically grounded estimates, transparent formulas, and the tools to stress-test your finances before you sign anything.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/mortgagemate_logo.png" alt="Mortgage Mate Logo" width="200"/>
</p>

---

## Why I Built This

As a statistician, I've spent years teaching people how to reason under uncertainty. Most home loan calculators on the market treat your finances as if they were perfectly known — plug in your income, get a number, done.

But that's not how statistics works, and it's not how life works either.

Mortgage Mate applies the same thinking I use in my research: uncertainty should be quantified, not hidden. The result is a simulator that gives you confidence intervals, stress tests, and transparency about every formula used — so you can walk into a broker's office actually understanding your position.

---

## Key Features

### 📊 Borrowing Power Estimator

Most tools give you a single borrowing figure. Mortgage Mate gives you a **95% confidence interval** modelled on ABS Household Expenditure Survey data — a range that honestly reflects real-world variation in living costs.

Factors included:
- **Income mode**: enter annual gross income or monthly post-tax salary
- **Household composition**: adults, children, and pets
- **HECS/HELP debt**: ATO 2025–26 compulsory repayment rates applied to gross income before assessment
- **APRA's 3% serviceability buffer** (APG 223, effective October 2021): your rate + 3% is used for assessment, matching what lenders actually do

The lower bound of the interval is your conservative estimate. The upper bound reflects what's possible with lean living costs. The midpoint is your best single-number guess.

### 🌡️ Stress-O-Meter

A visual **debt-to-income ratio gauge** featuring animated character scenes — *Chilling*, *Jogging*, and *Lifting* — that shift as your financial stress changes.

- Instantly see which "stress zone" your current loan falls into
- Simulate rate rises of **+1%, +2%, or +3%** above your current rate
- Watch how monthly repayments change as rates move
- Great for planning ahead before rate cycles turn

### ⚙️ Offset Engine

Model the impact of an offset account with:
- Sliders for current **offset balance** and **monthly contributions**
- A **dual-trajectory chart** plotting your loan with and without the offset account
- Exact figures for **years saved** and **interest saved**
- Milestone celebrations as you hit offset targets

Uses **true daily interest calculation** — the method Australian lenders actually use — not a simplified monthly approximation.

### 🔢 Repayment Calculator

Standard amortisation calculations for **monthly and fortnightly** repayment schedules.

The fortnightly rate uses the correct compound formula:

$$r_f = (1 + r_{\text{annual}})^{1/26} - 1$$

with 26 payments per year — **not** the common (and inaccurate) monthly ÷ 2 shortcut. This means your fortnightly repayment projection genuinely reflects accelerated payoff, not just a cosmetic repackaging of the monthly figure.

---

## What Makes It Different

| Feature | Mortgage Mate | Typical Calculator |
|---|---|---|
| Borrowing power | 95% CI based on ABS data | Single estimate |
| Living cost model | ABS Household Expenditure Survey | Rule of thumb |
| Serviceability buffer | APRA 3% (APG 223) applied | Often ignored |
| HECS/HELP | ATO 2025–26 rates applied | Rarely included |
| Offset calculation | True daily interest | Simplified |
| Fortnightly rate | Correct compound formula | Monthly ÷ 2 |
| Stamp duty | All states/territories (2025–26) | Often missing |
| Data collection | None | Often tracked |
| Formula transparency | Fully disclosed in-app | Black box |

---

## Built by a Statistician

Every formula in Mortgage Mate is documented in the app. There are no hidden assumptions, no proprietary "estimates", and no black boxes. The borrowing power interval is derived from published ABS data with a modelled standard deviation of 10% of estimated expenses ($\sigma$ = 0.10 × expenses), giving a CI of ±1.96$\sigma$.

---

## Privacy & No Ads

Mortgage Mate is completely private:

- **No login required**
- **No personal data collected or transmitted**
- **No ads, no subscriptions**
- All calculations run entirely on your device

---

## Disclaimer

Mortgage Mate is a statistical simulation tool for **educational purposes**. All results — borrowing power, repayment figures, interest savings, and offset projections — are estimates based on standard mathematical formulas. We are not a financial institution or a licensed financial advisor. These figures do not constitute financial or legal advice.

Always verify results with your lender or a licensed mortgage broker before making any financial decisions.

---

Questions or feedback? [Get in touch]({{ site.baseurl }}/contact) or visit the [Support Page]({{ site.baseurl }}/2026/03/06/MortgageMate-Support).
