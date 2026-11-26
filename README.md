# Amazon India Business Dashboard

A single-page, dependency-free dashboard that turns order-level data into KPIs, charts and written insights for management.

**All data is synthetic and for learning only. It is not real Amazon data.**

## What it analyses
| Area | What you see |
|---|---|
| Sales and profit | Net revenue, net profit, margin, monthly trend |
| Products | Top 8 products by profit with units, revenue and margin |
| Orders | Order count, average order value |
| Customer order status | Delivered, Shipped, Pending, Cancelled, Returned |
| Payment methods | Share of orders and share lost to cancel/return |
| Fulfillment | Fulfilled by Amazon vs Seller Fulfilled: delivery rate, days, margin |
| Geography | Top 10 states by net revenue with margin |
| Insights | Auto-written findings that update with the filters |

## Definitions
- **Net revenue** = qty × price for orders not Cancelled or Returned.
- **Net profit** = qty × (price − cost) for the same orders.
- **Margin** = net profit ÷ net revenue.
- **Cancel + return rate** = (Cancelled + Returned) ÷ all orders.

## Run it
Open `index.html` in a browser. No build step.

## Use your own data
Click **Load your CSV**. Required columns (header row, comma separated, no quoted commas):
`date,category,product,state,payment,fulfillment,status,qty,price,cost,delivery_days`
Use **Download sample CSV** to get a ready template. Status values: Delivered, Shipped, Pending, Cancelled, Returned.

## Student tasks
1. Which category earns the most revenue, and which earns the best margin? Are they the same?
2. How much does the festive season (Oct–Nov) lift revenue?
3. Compare payment methods. Should Cash on Delivery be discouraged?
4. Is Fulfilled by Amazon worth its cost? Support your answer with delivery rate and days.
5. Pick one state to invest in and justify it with the geography panel.

## Deploy on GitHub Pages
Settings → Pages → Deploy from branch → main / (root).