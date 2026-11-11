# Pizza POS: live demo (no login, no server)

One file: `index.html`. It runs completely in the visitor's browser, so there is nothing on a server that can crash.
No login page: use the **View as** buttons at the top (Cashier, Manager, Owner) to see what each role can do.

## Try it on your PC
Double-click `index.html`.

## Put it on GitHub and Vercel
1. Create an empty repository on github.com, then in this folder run:
```
git init
git add .
git commit -m "Pizza POS demo"
git branch -M main
git remote add origin https://github.com/YOUR-NAME/pizza-pos-demo.git
git push -u origin main
```
(No Git? On GitHub choose Add file, Upload files, and drop `index.html` in.)
2. vercel.com, Add New, Project, import the repository.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Press **Deploy**.

## What the demo shows
- **Cashier:** opening balance, billing (sizes, extras, notes, discounts, hold orders, cash/card/online/split with change, receipts and kitchen slips), live drawer total, closing balance with difference.
- **Manager:** orders and refunds, menu and prices, recipes, inventory (stock-in, wastage, counts), reports, every cashier's shifts.
- **Owner:** everything, plus profit, **Roles and tokens** (tick permission tokens and the screens change immediately when you switch role), settings and the audit log.

## Good to know
- Sample data (one week of sales) is created on first visit and saved in the visitor's own browser. Nothing is sent anywhere.
- **Reset demo** (yellow bar) restores the original data.
- This is a demonstration. The full software with a real database is the separate Python version.
