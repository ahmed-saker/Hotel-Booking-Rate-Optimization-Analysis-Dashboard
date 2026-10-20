# Hotel Booking Rate Optimization & Analysis Dashboard 📊

An advanced data analysis and visualization project built with **Python** and **Dash**. It pulls active hotel bookings via **Juniper SOAP API**, cross-references them with real-time availability, identifies cheaper alternatives using **fuzzy string matching**, and presents the findings in an interactive, user-friendly web dashboard.

---

## 🚀 Features

- 🔄 **Automated Data Fetching** — Pulls upcoming bookings from the Juniper `wsBookings` SOAP endpoint asynchronously.
- 🏨 **Real-time Availability Check** — Queries live room availability for specific hotels, dates, and guest combinations.
- 🧠 **Smart Room Matching** — Uses `rapidfuzz` to intelligently match booked room names with available room types (handling abbreviations like DBL/SGL/TPL).
- 💰 **Rate Comparison & Filtering** — Calculates the price difference (Savings) and filters for alternatives that are significantly cheaper (e.g., saving $20+), refundable, and have a good cancellation policy.
- 📊 **Interactive Dashboard** — Built with `Dash` and `Dash Bootstrap Components` (DBC), providing a clean, card-based UI to browse bookings, original rates, and alternative options.
- ⚡ **Asynchronous Processing** — Uses `asyncio` and `aiohttp` with `tqdm` progress bars to process thousands of booking codes efficiently.

---

## 🧰 Tech Stack

| Layer | Tools |
|---|---|
| **Language** | Python 3 |
| **Data Manipulation** | `pandas`, `numpy`, `json` |
| **Web Framework (UI)** | `Dash`, `Dash Bootstrap Components`, `plotly` |
| **API & Networking** | `requests`, `aiohttp`, `asyncio`, `xmltodict` |
| **String Matching** | `rapidfuzz` |
| **Utilities** | `tqdm`, `retrying`, `datetime` |
| **APIs** | Juniper SOAP API (Bookings & Availability) · EET Global XML API |

---

## ⚙️ How It Works
