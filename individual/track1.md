# Track 1 — Where does the data come from? (Customer Churn)

## 1) Expected source tables (3–5)

1. **Customer / Account Master**
   - One row = one customer or account.
   - IDs + demographics + account status.

2. **Subscription / Contract History**
   - One row = one customer contract period.
   - Contract term, plan changes, start/end dates.

3. **Billing & Payments**
   - One row = one monthly invoice per customer.
   - Monthly charges, payment method, refunds, late payments.

4. **Product Usage / Service Activity**
   - One row = one customer per time period (daily/weekly/monthly).
   - Usage volume, add-ons, overage events.

5. **Support / Service Tickets**
   - One row = one support interaction or event.
   - Ticket reason, escalation, resolution, service outages.

## 2) Keys to connect the data

- `customer_id` (main customer key)
- `account_id` (connects household/business accounts)
- `subscription_id` or `service_id` (connects contract + usage)
- `invoice_id` + `bill_month` (connects billing and time alignment)

## 3) Two risks + how to reduce them

1. **Data leakage**
   - Risk: Using cancellation or “final bill” info that happens after churn.
   - Fix: Use a strict cutoff date and build features only from prior history.

2. **Duplicates or missing IDs**
   - Risk: Joins can duplicate customers or drop records.
   - Fix: Validate row counts after merges and enforce unique customer records.
