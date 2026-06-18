# API Discovery Portfolio: Amazon Platform Features

Welcome to my API Discovery portfolio project. This repository contains deep-dive architectural analyses, payload breakdowns, and automated testing strategies for core features on the Amazon platform. 

The purpose of this project is to demonstrate strong manual API exploration skills, a solid understanding of backend session logic, and the ability to design comprehensive QA test scenarios for complex web applications.

## 🚀 Features Analyzed

1. **Amazon Cart Feature (Add to Cart)**
   * **Focus:** Resource mutation (`POST`), microservice versioning, and time-bound inventory reservation rules.
2. **Amazon Search Feature (Internal Telemetry)**
   * **Focus:** Asynchronous tracking engines (`POST`), data privacy (PII) compliance, and input sanitization testing.
3. **Amazon Change Quantity Feature (Cart Update)**
   * **Focus:** State replacements (`PUT`), server-enforced business logic, and backend calculations.

---

## 🛠️ Key Technical Concepts Demonstrated

* **Methodology Alignment:** Deep verification of `POST` vs. `PUT` architectural requirements, tracking execution flows, and interpreting HTTP status responses.
* **Contract Validation:** Auditing strict vendor-specific media-type versioning headers (e.g., `application/vnd.com.amazon.api+json`).
* **Asynchronous UX Auditing:** Ensuring that background AJAX traffic (`X-Requested-With: XMLHttpRequest`) executes seamlessly without blocking UI render cycles.
* **Data-Driven Test Design:** Mapping complex testing strategies including Boundary Value Analysis (BVA), Equivalence Partitioning, and Cross-Site Scripting (XSS) input sanitization.

---

## 📋 Detailed Feature Profiles

### Feature 1: Amazon Cart Feature (Add to Cart)
* **Endpoint Type:** Inventory Allocation Mutation
* **HTTP Method:** `POST`
* **Core Logic:** When a user claims a deal, the backend assigns a strict 15-minute (`900000ms`) inventory hold to prevent stock hoarding. 
* **QA Test Focus:** Race conditions during reservation expirations, boundary limitations on unit quantities, and tracking localized error handling (`400 Bad Request`).

### Feature 2: Amazon Search Feature (Internal Telemetry)
* **Endpoint Type:** Telemetry & Performance Metrics Logging
* **HTTP Method:** `POST`
* **Core Logic:** Isolates real-time search string interactions completely out-of-band to safeguard main catalog loading queues.
* **QA Test Focus:** Malformed URL-encoding handling, thread isolation verification under high network latency, and cleartext PII leak prevention.

### Feature 3: Amazon Change Quantity Feature (Cart Update)
* **Endpoint Type:** Basket State Replacement
* **HTTP Method:** `PUT` (Idempotent execution framework)
* **Core Logic:** The pricing model enforces absolute backend authority. The client interface simply displays calculated total responses to block local price injection exploits.
* **QA Test Focus:** Zero-value nullification (testing deletion routing triggers) and inventory cap overrun flags (`availableStockLimitReached: true`).

---

## 🔮 Future Expansion Roadmaps
* [ ] Convert outlined test ideas into fully executable **Postman Collection assertions**.
* [ ] Implement an automated testing pipeline using **RestAssured / Python Requests**.
* [ ] Add automated load and performance testing templates to simulate high-concurrency traffic over the inventory reservation endpoints.

---
