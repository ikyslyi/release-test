# GitHub Issue Lifecycle & Labels Guide for Shkeeper.io

## Issue Lifecycle Overview

This document outlines how issues should progress through the lifecycle in the **Shkeeper.io** repository. It provides **status labels**, **priority levels**, and **real-world workflows** for common issue types.

---

## **Issue Type Labels & Example Workflows**

### **1. `type/bug` - A system feature is broken**
**Example:** The **Shkeeper.io authentication service** is failing to validate JWT tokens.

#### **Workflow:**
1. Issue created: **A user reports that authentication is failing on login.**
   - **Labels:** `type/bug`, `priority/high`, `status/needs review`
2. Maintainer reviews and confirms it as a valid bug.

   - **Labels Updated:** `status/in progress`
3. Developer fixes the bug in the authentication service and submits a Pull Request.

   - **Labels Updated:** `status/ready for testing`
4. Reviewer verifies the fix in staging, and it passes tests.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

### **2. `type/enhancement` - Improving an existing feature**
**Example:** The **server dashboard** needs to display real-time CPU and memory usage.

#### **Workflow:**
1. Issue created: **A user requests the addition of real-time monitoring to the dashboard.**
   - **Labels:** `type/enhancement`, `priority/medium`, `status/needs review`
2. Maintainer reviews and confirms the request.

   - **Labels Updated:** `status/in progress`
3. Developer integrates WebSockets for real-time updates and submits changes.

   - **Labels Updated:** `status/ready for testing`
4. Reviewers approve the feature, and it is merged.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

### **3. `type/feature request` - A new feature proposal**
**Example:** A user requests **role-based access control (RBAC)** for admin users.

#### **Workflow:**
1. Issue created: **User submits a request for an RBAC feature to allow granular permissions.**
   - **Labels:** `type/feature request`, `priority/high`, `status/needs review`
2. Maintainer reviews and determines it's a valuable addition.

   - **Labels Updated:** `status/in progress`
3. Developer implements RBAC logic and submits the feature.

   - **Labels Updated:** `status/ready for testing`
4. Feature is tested and merged into the main branch.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

### **4. `type/documentation` - Docs are outdated or missing**
**Example:** The **Shkeeper.io API documentation** does not include Webhook integration details.

#### **Workflow:**
1. Issue created: **A user reports that the API docs are missing Webhook setup instructions.**
   - **Labels:** `type/documentation`, `priority/medium`, `status/needs review`
2. Maintainer reviews and assigns a contributor to update the docs.

   - **Labels Updated:** `status/in progress`
3. Contributor updates the API documentation and submits a PR.

   - **Labels Updated:** `status/ready for testing`
4. Documentation changes are approved and merged.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

### **5. `type/support` - A user needs clarification**
**Example:** A developer asks how **to integrate Shkeeper.io billing API** with Stripe.

#### **Workflow:**
1. Issue created: **User submits a question about Stripe integration.**
   - **Labels:** `type/support`, `status/awaiting feedback`
2. Maintainer responds with a detailed answer.

   - **Labels Updated:** `status/needs review`
3. User confirms they got the information they needed.

   - **Issue closed.**

---

### **6. `type/security` - A vulnerability is reported**
**Example:** A **developer discovers an API endpoint that exposes sensitive user data**.

#### **Workflow:**
1. Issue created: **A security researcher reports the vulnerability privately.**
   - **Labels:** `type/security`, `priority/high`, `status/needs review`
2. Maintainers verify and confirm it as a critical security issue.

   - **Labels Updated:** `status/in progress`
3. A security patch is implemented and tested.

   - **Labels Updated:** `status/ready for testing`
4. Fix is approved and deployed to production.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

### **7. `type/performance` - Speed optimization needed**
**Example:** **The dashboard page loads slowly due to inefficient database queries.**

#### **Workflow:**
1. Issue created: **User reports high latency in dashboard loading times.**
   - **Labels:** `type/performance`, `priority/high`, `status/needs review`
2. Developer optimizes SQL queries and caching mechanisms.

   - **Labels Updated:** `status/in progress`
3. Optimizations are tested under load conditions.

   - **Labels Updated:** `status/ready for testing`
4. Performance improvements are validated.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

### **8. `type/refactor` - Code cleanup without feature change**
**Example:** **Rewriting the authentication module to improve maintainability.**

#### **Workflow:**
1. Issue created: **A developer suggests refactoring authentication logic for better scalability.**
   - **Labels:** `type/refactor`, `priority/low`, `status/needs review`
2. Maintainers approve the refactor and assign it.

   - **Labels Updated:** `status/in progress`
3. Developer refactors the code and submits a PR.

   - **Labels Updated:** `status/ready for testing`
4. Changes are reviewed and merged.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

### **9. `type/design` - UI/UX-related improvements**
**Example:** **Improve the mobile layout of the server management dashboard.**

#### **Workflow:**
1. Issue created: **A user reports UI elements breaking on mobile.**
   - **Labels:** `type/design`, `priority/medium`, `status/needs review`
2. Designer provides mockups for the new UI layout.

   - **Labels Updated:** `status/in progress`
3. Developer implements the design changes and submits a PR.

   - **Labels Updated:** `status/ready for testing`
4. UI updates are reviewed and approved.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

### **10. `type/dependencies` - Updating libraries or packages**
**Example:** **Upgrade to the latest PostgreSQL version for improved database performance.**

#### **Workflow:**
1. Issue created: **A developer suggests upgrading PostgreSQL to the latest stable version.**
   - **Labels:** `type/dependencies`, `priority/low`, `status/needs review`
2. Maintainer confirms and assigns the issue.

   - **Labels Updated:** `status/in progress`
3. Developer upgrades PostgreSQL and tests migrations.

   - **Labels Updated:** `status/ready for testing`
4. Update is merged and verified.

   - **Labels Updated:** `resolution/closed`
   - **Issue closed.**

---

## **Final Thoughts**
By using these structured workflows in the **Shkeeper.io** repository, contributors and maintainers can ensure that issues progress smoothly and efficiently, maintaining project stability and development transparency.

🚀 **Happy Developing!** 🚀
