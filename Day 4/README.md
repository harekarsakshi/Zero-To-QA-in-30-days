# Day 4
# Hands-On Lab: Identifying Testing Types on Amazon Login
**Target Page:** `amazon.com/ap/signin`

---

### 1. Functional Testing
*   **Scenario:** Verify that entering a valid registered email/phone number and the correct password successfully logs the user into their account dashboard.

### 2. Usability Testing
*   **Scenario:** Verify that pressing the 'Tab' key on the keyboard moves the focus sequentially and logically from the Email field to the 'Continue' button, and then to the password field.

### 3. Performance Testing
*   **Scenario:** Verify that the login authentication process completes, and the homepage or dashboard fully loads, in under 2.0 seconds under a simulated stable 4G connection.

### 4. Security Testing
*   **Scenario:** Verify that characters entered into the password input field are masked (displayed as dots or asterisks) and that the password cannot be copied to the clipboard.

### 5. Compatibility Testing
*   **Scenario:** Verify that the layout renders correctly and the login flow works flawlessly across multiple browsers and platforms (e.g., Safari on iOS, Chrome on Android, Firefox and Edge on Desktop).

### 6. Accessibility Testing (a11y)
*   **Scenario:** Verify that all input fields (Email/Password) and buttons ('Continue', 'Sign-In') have descriptive `aria-label` tags so that screen readers (like NVDA or VoiceOver) can read them accurately for visually impaired users.

### 7. Regression Testing
*   **Scenario:** After a backend deployment or a fix to the password reset flow, re-run existing login test cases to ensure that regular users can still sign in successfully without any new errors.

### 8. Localization Testing (l10n)
*   **Scenario:** Verify that changing the global language selector (e.g., from English to Spanish) accurately translates all text on the login page—including error messages, button text, and placeholder text—without breaking layout alignment or text wrapping.
