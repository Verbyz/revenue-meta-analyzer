# Revenue Meta Analyzer

A lightweight tool to experiment with revenue pricing and effective revenue multipliers
for crypto and DeFi tokens.

## Goal
Compare direct fee-sharing models vs buyback-based revenue models.

## Run
```bash
npm install
npm start

---

## ✅ Commit 3 — `Add revenue multiplier calculator`

**`calculator.js`**
```js
function revenueMultiplier(marketCap, annualRevenue) {
  if (annualRevenue === 0) return Infinity;
  return marketCap / annualRevenue;
}

module.exports = { revenueMultiplier };
