# Startup Metrics BI Dashboard

This project is a single-page web application designed to demonstrate core Business Intelligence (BI) principles for entrepreneurial decision-making. It provides a real-time view of key startup health metrics, combining historical data with predictive insights.

The application is built entirely using **HTML, embedded CSS, and Vanilla JavaScript** for portability and minimal dependencies.

---

## Key Features

* **Single-Page Architecture:** All code (HTML, CSS, JS) resides within the `index.html` file.
* **Data Persistence:** All metric entries are stored securely using the browser's **`localStorage`** API, ensuring data survives page refreshes.
* **Core KPI Visualization:** Displays the five mandatory Key Performance Indicators (KPIs) required for startup health monitoring:
    1.  **Runway (Months):** A critical **Predictive** metric.
    2.  **Total Revenue:** Sum of all Monthly Recurring Revenue (MRR).
    3.  **Average Monthly Burn:** Average Operating Expenses.
    4.  **Net Revenue Trend:** Visual indicator (Growing/Declining) based on MRR.
    5.  **Customer Growth:** Trend indicator based on new customers acquired.
* **Data Integrity:** Includes robust **form validation** to ensure metric fields are numeric and prevents duplicate entries for the same reporting period.
* **Visual Indicators:** Uses color-coding (Green/Red/Orange) and trend arrows to provide immediate, prescriptive feedback on the health status of the business.

---

## Running the Application

Since this is a single `.html` file, it can be run in two simple ways:

1.  **Local Execution:** Download the `index.html` file and open it directly in any web browser (Chrome, Firefox, Safari, etc.).
2.  **Deployment (GitHub Pages):** Upload the `index.html` file to the root of a GitHub repository and **enable GitHub Pages** in the repository settings to get your live application link.

---

## Data Structure

Data is stored as a JSON array in `localStorage` under the key `startupMetricsData`. Each entry object includes the following fields:

* `period` (String, e.g., "Oct 2025")
* `mrr` (Number)
* `newCustomers` (Number)
* `churn` (Number)
* `operatingExpenses` (Number)
* `cashBalance` (Number)
