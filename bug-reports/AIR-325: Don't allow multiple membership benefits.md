
# AIR-325 — Don't allow multiple membership benefits on 1 item

## Test Result Report

**Environment:** Staging  
**URL:** https://staging.airtopiapark.com/pos/dashboard  
**Order:** #10059  
**Order ID:** 69a887dde23e1b395f7e8d0b  

---

## Test Objective
Verify that the POS system does not allow **multiple membership benefits to be applied to a single item** and ensures that only the **benefit with the maximum discount** is applied.

---

## Test Scenario
A customer with an active **Elite Class SkyPass** membership was selected in the POS system.  
Multiple items were added to the order to verify whether more than one membership benefit could be applied to the same item.

---

## Items in Order

| Item | Quantity | Price |
|-----|-----|-----|
| Nachos | 3 | $26.97 |
| Fountain Drink Pitcher | 1 | $9.99 |
| Kids Meal | 1 | $8.99 |
| Tee Shirt - Large | 1 | $15.50 |

---

## Applied Discounts

**Elite Class SkyPass – Free Pucker Powder & Kit**  
- Applied to: Nachos  
- Discount: **-$26.97**

**Elite Class SkyPass – 7.5% off Parties, Eatery, Merchandise**  
- Applied to: Fountain Drink Pitcher, Kids Meal  
- Discount: **-$1.33**

---

## Observed Behavior
- Each item received **only one membership benefit**.
- Discounts were applied to **different items**, not stacked on the same item.
- No cases were observed where multiple membership benefits were applied to a single item.

---

## Expected Behavior
The system should apply **only one membership benefit per item**.  
If multiple benefits are available, the system should apply the **benefit with the highest discount value**.

---

## Result
The issue **was not reproduced during testing**.  
Membership benefits were applied correctly and **no multiple benefits were stacked on the same item**.

---

## Test Evidence

![Test Screenshot](./screenshots/AIR-325-membership-benefits-test.png)

---

## Bug Details

**Status:** Not Reproduced  
**Severity:** Medium  
**Priority:** Low  

---

## Notes / Risks

- Additional validation is recommended for edge cases:
  - Multiple percentage-based benefits
  - Percentage vs fixed discount
  - Equal discount values across benefits
- Potential risk of incorrect discount calculation if stacking logic is not properly restricted

---

## Related Test Cases

- TC_POS_MEMBERSHIP_001 — Verify single benefit per item
- TC_POS_MEMBERSHIP_002 — Validate maximum discount selection
- TC_POS_MEMBERSHIP_003 — Verify no benefits applied without membership
