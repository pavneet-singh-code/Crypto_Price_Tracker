# 📊 Crypto Price Tracker (Next.js)

A modern **Crypto Price Tracking web application** built with **Next.js** that helps users track real‑time cryptocurrency prices, market trends, and key statistics using public APIs.

This project is intentionally designed as a **learning-first project** to break out of tutorial hell and gain hands‑on experience with:

* API consumption
* Async data handling
* State management
* Error & loading states
* Clean project structure

---

## 🚀 Live Demo

> (Add Vercel link here once deployed)

---

## 🧠 Why this project exists

This project is part of a **month‑by‑month learning roadmap**.

**February focus:**

* Learning how real‑world applications consume APIs
* Handling loading, errors, and edge cases
* Understanding how data flows in a Next.js app

No authentication. No database. Just **pure fundamentals done right**.

---

## 🛠 Tech Stack

* **Framework:** Next.js (App Router)
* **Language:** JavaScript / TypeScript
* **Styling:** CSS / Tailwind (mention what you use)
* **API:** CoinGecko Public API
* **Charts:** Chart.js / Recharts
* **Deployment:** Vercel

---

## 📂 Project Structure

```
/app
 ├── page.tsx        → Home page (crypto list)
 ├── coin/[id]/      → Dynamic route for individual coin details
 ├── loading.tsx     → Global loading UI
 ├── error.tsx       → Error handling UI
/components
 ├── CoinCard.tsx    → Displays basic coin info
 ├── SearchBar.tsx   → Search and filter coins
 ├── PriceChart.tsx  → Historical price graph
/lib
 ├── api.ts          → API utility functions
/public
 └── favicon.ico
```

---

## 🧭 Application Flow & Routes

### 🏠 `/` – Home Page

**What it shows:**

* List of top cryptocurrencies
* Current price, market cap, 24h change

**What happens behind the scenes:**

* Fetches data from CoinGecko API
* Shows loading spinner while data loads
* Displays error UI if API fails

---

### 🔍 Search & Filter

* Search crypto by name or symbol
* Filter based on price change

**Learning focus:**

* Controlled inputs
* Client‑side state management
* Performance‑friendly filtering

---

### 📈 `/coin/[id]` – Coin Detail Page

**What it shows:**

* Coin name & symbol
* Price trends (graph)
* Market stats

**Learning focus:**

* Dynamic routing
* URL parameters
* Fetching data based on route params

---

## ⚙️ API Handling Strategy

* API calls isolated inside `/lib/api.ts`
* `async/await` used for clarity
* Graceful fallback UI for:

  * Network failures
  * Rate limits
  * Empty responses

---

## ⏳ Loading & Error States

Handled using **Next.js App Router features**:

* `loading.tsx` → Shown while data is fetching
* `error.tsx` → Shown when API fails

This ensures a smooth user experience.

---

## 🌱 Environment Variables

```
NEXT_PUBLIC_API_BASE_URL=https://api.coingecko.com/api/v3
```

Keeps sensitive config out of the codebase.

---

## 📸 Screenshots

> Add screenshots of:

* Home page
* Search results
* Coin detail page

---

## 🧪 What I Learned

* How real APIs behave (latency, errors, limits)
* Difference between server & client components
* Writing reusable fetch utilities
* Designing clean UI for async data

---

## 🔮 Future Improvements

* Dark mode
* Pagination
* Favorites/watchlist
* Currency conversion

---

## 📌 How to Run Locally

```bash
npm install
npm run dev
```

Open `http://localhost:3000`

---

## 👤 Author

**Pavneet Singh**
Computer Science Student
Building projects month‑by‑month to master full‑stack development.

---

⭐ If you find this project useful, give it a star!

