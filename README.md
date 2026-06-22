# 🛒 Amazon QA Audit & Test Engineering Portfolio

## 📌 Project Overview
Welcome to my centerpiece QA Portfolio. This repository represents an intensive, hands-on **30-Day Technical Sprint** focused on end-to-end Test Engineering for a high-traffic e-commerce ecosystem based on Amazon.com. 

Rather than focusing on passive theory, this portfolio documents real-world QA engineering artifacts—spanning full-cycle manual testing, layout diagnostics, Agile BDD styling, API validation using Postman, and backend relational database verification using MySQL.

*   **Domain Focus**: Amazon.com Core Commerce Engine (Search, Discovery, Cart, Checkout, and Orders)
*   **Objective**: Ensure zero data-bleeding, complete structural integrity, and perfect frontend-to-backend alignment across transactional workflows.

---

## 📂 Repository Architecture & Artifacts

The deliverables in this repository are categorized systematically by technical testing discipline to match real-world engineering standards:

### 📑 1. Test Plans (`/Day 1` to `/Day 7`)
*   **[Day 1: Visual Regression & Layout Diagnostics](./Day%201)**: Comprehensive audit mapping UI positioning bugs and cross-browser formatting discrepancies.
*   **[Day 2: SDLC Mapping](./Day%202)**: Critical strategic breakdowns contrasting Waterfall execution models against Agile-Scrum testing cycles.
*   **[Day 3: Amazon Search Bar Test Plan](./Day%203)**: Comprehensive Software Testing Life Cycle (STLC) master test plan specifying scope, risks, resources, and pass/fail criteria for search indexing.
*   **[Day 4: Identifying Testing Types](./Day%204)**: Rigorous technical mapping of Functional, Non-Functional, Regression, and Security testing vectors on the Amazon login screen.

### 🧪 2. Test Cases & Bug Reports (`/Day 5` to `/Day 9`)
*   **[Day 5: Test Case Design Patterns](./Day%205)**: Detailed positive, negative, and boundary-value test matrices mapping shopping cart modifications and multi-tier edge checkout interactions.
*   **[Day 6: Defect Management & Bug Reports](./Day%206)**: High-fidelity, engineering-ready bug logs featuring clear steps-to-reproduce, severity/priority triage levels, and expected vs. actual outcomes.
*   **[Day 7: Test Planning & Risks](./Day%207)**: Risk-based manual execution scripts dealing with high-severity purchase workflows.
*   **[Day 8: Black Box Testing Techniques](./Day%208)**: Equivalence partitioning and boundary value analysis applications for input validation.
*   **[Day 9: Exploratory Testing Sessions](./Day%209)**: Real-time, unscripted time-boxed testing charter logs targeting checkout vulnerability scenarios.

### 🏃‍♂️ 3. Agile & User Stories (`/Day-10`)
*   **[Day-10: BDD User Stories & Gherkin](./Day-10)**: Clear product requirements translated cleanly into actionable test documentation using **Given-When-Then** syntaxes for scrum readiness.

### ⚡ 4. API Testing (`/Day-11` to `/Day-12`)
*   **[Day-11: API Discovery & Mapping](./Day-11)**: Mapping backend service structures, request routes, headers, and payload configurations for checkout microservices.
*   **[Day-12: Postman Test Suite](./Day-12)**: Automated execution collections validating HTTP status codes (`200 OK`, `201 Created`, `400 Bad Request`), structural schema assertions, and response times.

### 🗄️ 5. Database Verification (`/Day-13`)
*   **[Day-13: SQL Order Audit Scripts](./Day-13)**: Advanced **MySQL v5.7** script models verifying calculations (totals, prices, quantity aggregations) and hunting orphaned transactions via custom `LEFT JOIN ... IS NULL` queries to secure absolute transactional data integrity.

---

## 💡 Key QA Methodologies Demonstrated
1.  **Boundary Value Analysis (BVA)**: Applied directly on quantities (testing $0$, $1$, max cart constraints) and refund triggers to ensure correct code handling.
2.  **Data Integrity Checks**: Looking beyond what the customer sees on the UI screen to query backend databases, verifying no phantom records hide behind cancelled actions.
3.  **API Automation Layering**: Writing JavaScript test scripts inside Postman collections to instantly validate regression parameters across endpoint chains.

---

## 🔗 Connect with My Journey
*   **Learning Journal & Daily Updates**: [Follow my Progress on Substack / LinkedIn]
