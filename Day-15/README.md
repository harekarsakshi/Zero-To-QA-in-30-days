# Day 15
# Amazon Checkout Flow — QA Automation Strategy & ROI Audit

## 📌 Project Overview
This repository contains a comprehensive Quality Assurance Audit and Test Automation Strategy for the high-volume **Amazon Checkout Flow**. Moving a product flow from a purely manual regression cycle to a strategic automated framework requires a risk-based evaluation of what to automate, where those tests belong, and what business value they return.

This artifact details the exact architectural layers for our regression suite, logs a core test case matrix mapped by feasibility, defines manual edge-case boundaries, and outlines a data-backed Return on Investment (ROI) analysis.

---

## 📐 The Testing Pyramid Architecture
To maximize testing execution speed and reduce maintenance overhead, this strategy abandons the "ice cream cone" anti-pattern (too many slow UI tests) and instead implements a balanced **Testing Pyramid**.

```text
               ▲
              / \
             /E2E\   <-- 10% (Critical Smoke / Full User Journeys)
            /-----\
           /  API  \  <-- 20% (Integration / Backend Endpoints)
          /---------\
         /   Unit    \ <-- 70% (Component / Front-end UI States)
        /_____________\
