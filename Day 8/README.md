# Amazon Quality Assurance Audit: Black Box Testing

A comprehensive portfolio project demonstrating practical application of core software testing methodologies on Amazon's consumer application features. This repository functions as a standalone exhibit of my manual testing capabilities, test case architecture, and analytical risk assessment.

## 📌 Project Overview
This project focuses on auditing critical components of the Amazon e-commerce engine—specifically the front-end **Cart Quantity Selector** constraints and the back-end **Order Fulfillment Lifecycle**. 

By applying industry-standard black-box design techniques, the scope ensures optimal edge-case coverage and logical validation without needing direct access to the application's underlying codebase.

---

## 🛠️ Core Testing Techniques Applied

### 1. Equivalence Partitioning (EP)
Divided the input domain of the quantity selector (valid range: 1 to 30) into logical equivalence classes to optimize execution efficiency. Tested a single representative value from each partition to validate expected application behavior:
*   **Invalid-Low Class:** Evaluated values `< 1` (Test Value: `0`) to confirm proper error handling or default resetting.
*   **Valid Class:** Evaluated values within bounds (Test Value: `15`) to confirm seamless cart updates.
*   **Invalid-High Class:** Evaluated values `> 30` (Test Value: `35`) to verify quantity capping limitations.

### 2. Boundary Value Analysis (BVA)
Focused execution specifically on the operational limits where software defects most frequently occur (off-by-one errors). Rigorously tested boundaries and their immediate neighboring steps:
*   **Lower Boundary Extremes:** Tested `0`, `1`, and `2` to ensure strict validation at the minimum threshold.
*   **Upper Boundary Extremes:** Tested `29`, `30`, and `31` to check system resilience at maximum threshold capacities.

### 3. Decision Table Testing
Constructed a logical matrix to validate complex business rules driving Amazon's Free Shipping algorithms. Evaluated the cascading behavior of multi-variable conditions:
*   *Condition Variables:* Prime Membership Status, Order Subtotal thresholds ($35), and individual Item Eligibility.
*   *Goal:* Ensure the correct billing logic is systematically applied across all valid and combinations.

### 4. State Transition Testing
Mapped out a complete end-to-end user workflow tracing an order's state changes over time. Verified the sequential execution of the pipeline:
*   **Lifecycle Pipeline:** `Placed` ➔ `Shipped` ➔ `Out for Delivery` ➔ `Delivered` ➔ `Returned`.
*   Tested individual system triggers (e.g., carrier scanning, warehouse hand-offs) to ensure data state integrity is accurately reflected on the client profile.

---

## 🚀 Key Takeaways
*   **Test Optimization:** Reduced the necessity of running 30+ repetitive operational tests down to a highly optimized suite of 9 precise boundary and partition checks.
*   **Business Logic Coverage:** Formulated complete rule coverage for complex checking parameters using structured tabular formats, mitigating the risk of missed logical loopholes.
*   **User Journey Verification:** Ensured e-commerce pipeline stability by tracking backend state changes against expected user notifications.
