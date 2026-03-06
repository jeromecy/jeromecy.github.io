---
layout: post
title: "Mortgage Mate — Support & FAQ"
date: 2026-03-06
categories: [Apps, iOS, Finance]
tags: [mobile-app, mortgage, finance, support, FAQ]
description: "Support page and frequently asked questions for Mortgage Mate — the data-driven home loan simulator for Australian buyers."
---

# Mortgage Mate — Support & FAQ 🏡

Thank you for using Mortgage Mate. This page covers frequently asked questions, known limitations, and how to get in touch.

---

## Frequently Asked Questions

### 📊 Borrowing Power

**What does the 95% confidence interval mean?**

The borrowing power range reflects real-world variation in living costs, modelled on ABS Household Expenditure Survey data. Expenses are estimated from your household composition (income, adults, children, pets, HECS/HELP), and a standard deviation of σ = 10% of estimated expenses is applied.

The confidence interval is:

$$\text{Borrowing Power} = \bar{x} \pm 1.96\sigma$$

The midpoint (x̄) is your point estimate. The lower bound is a conservative scenario (higher expenses); the upper bound reflects leaner living costs. This is the same approach used in statistical inference — rather than pretending we know your exact costs, we acknowledge the uncertainty honestly.

---

**What interest rate is used for borrowing power assessment?**

The app uses your entered interest rate **plus 3%** — APRA's mandatory serviceability buffer under APG 223, which came into effect in October 2021. This matches the rate lenders are legally required to use when assessing whether you can afford a loan. Entering a lower rate than your actual rate will overstate your borrowing power.

---

**Are HECS/HELP repayments included?**

Yes. ATO compulsory repayment rates for 2025–26 are applied to your gross income before borrowing power is calculated, reducing assessed borrowing capacity in the same way lenders do.

---

**What states are supported for stamp duty estimates?**

All Australian states and territories are supported, using 2025–26 standard owner-occupier rates. Note that first home buyer concessions are not currently modelled (see Known Limitations).

---

### 🔢 Repayment Calculator

**Why does fortnightly repayment differ from monthly repayment ÷ 2?**

Many calculators (and even some lenders' websites) approximate fortnightly repayments as monthly ÷ 2. This understates the interest-saving benefit of fortnightly repayments.

Mortgage Mate uses the correct compound fortnightly rate:

$$r_f = (1 + r_{\text{annual}})^{1/26} - 1$$

with 26 payments per year. Because you make 26 fortnightly payments instead of 24 "half-monthly" ones, you pay slightly more per year — which accelerates payoff and reduces total interest. The difference compounds significantly over a 25-to-30-year term.

---

### ⚙️ Offset Engine

**How is the offset interest saving calculated?**

Interest is calculated daily on the outstanding loan balance minus the offset balance, matching the method used by Australian lenders. Each day's interest is:

$$\text{Daily interest} = \frac{r_{\text{annual}}}{365} \times (\text{Loan balance} - \text{Offset balance})$$

The dual-trajectory chart runs this computation across the full loan term, with and without the offset account, and reports the resulting difference in total interest paid and years remaining.

---

### 🌡️ Stress-O-Meter

**What do the stress zones mean?**

The Stress-O-Meter displays your debt-to-income (DTI) ratio and assigns it a visual stress zone:

| Zone | Character | Meaning |
|---|---|---|
| Chilling | Relaxed pose | Low DTI — repayments are manageable |
| Jogging | Active pose | Moderate DTI — keep an eye on rates |
| Lifting | Straining pose | High DTI — consider stress scenarios carefully |

The +1% / +2% / +3% rate rise simulation shows how your monthly repayment changes if rates increase, so you can assess your buffer before committing.

---

### 🔒 Privacy

**Does the app store my data?**

No. All calculations run entirely on your device. No data — income, loan amount, expenses, or any other input — is transmitted to any server. There is no account, no login, and no analytics.

---

## Known Limitations

- **First home buyer stamp duty concessions** are not modelled. The app uses standard owner-occupier rates for all states and territories. If you are eligible for a FHOG or stamp duty concession in your state, consult your broker or state revenue office for the accurate figure.
- **Results are estimates**. Always verify borrowing power, repayments, and stamp duty with your lender or a licensed mortgage broker before making financial decisions.
- **Tax calculations use resident rates only**. Non-resident or foreign investor tax obligations are not modelled.
- **Lender-specific policies are not reflected**. Individual lenders may apply stricter income assessment criteria, different expense benchmarks (HEM), or additional fees not captured in this app.

---

## Contact & Feedback

Found a bug, have a suggestion, or just want to say hello?

- **GitHub Issues**: [Report an issue or request a feature](https://github.com/zhanglongcao) *(repository link coming soon)*
- **Email**: [cao.zhanglong@gmail.com](mailto:cao.zhanglong@gmail.com)

If Mortgage Mate saved you time or helped you understand your finances better, an **App Store review** would mean a great deal — it's the best way to help other Australian home buyers find the app. 🙏

---

## Full Disclaimer

Mortgage Mate is a statistical simulation tool for **educational purposes**. All results — borrowing power, repayment figures, interest savings, and offset projections — are estimates based on standard mathematical formulas. We are not a financial institution or a licensed financial advisor. These figures do not constitute financial or legal advice.

Interest rates, tax thresholds, APRA buffers, ATO repayment rates, and stamp duty schedules are based on publicly available information current as of the 2025–26 financial year and are subject to change. The app is not updated in real time to reflect legislative or regulatory changes.

Always consult a licensed mortgage broker, financial advisor, or your lender before making any borrowing or purchasing decision.

---

*Back to [Mortgage Mate App Page]({{ site.baseurl }}/2026/03/06/MortgageMate)*
