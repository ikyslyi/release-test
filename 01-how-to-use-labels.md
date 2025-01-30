# How to Use GitHub Issue Labels Effectively

Applying and managing labels properly in your GitHub repository helps improve issue tracking, prioritization, and overall project management. Here’s how to use them effectively:

---

## **1. Assign Labels When Creating a New Issue**
- When a new issue is created, apply **Issue Type Labels** to categorize it.
- For example:

  - If it’s a bug, assign the **`type/bug`** label.
  - If it’s a feature request, assign the **`type/feature request`** label.
  - If it’s a documentation issue, assign **`type/documentation`**.

**Example:**
_A contributor reports a login error → Assign **`type/bug`** label._

---

## **2. Define the Priority**
- Use **Priority Labels** to indicate the urgency of the issue.
  - **`priority/high`** → Needs immediate attention.
  - **`priority/medium`** → Important but not urgent.
  - **`priority/low`** → Nice to have but not critical.

**Example:**
_A security vulnerability is found → Assign **`type/bug`** + **`priority/high`**._

---

## **3. Track the Status of the Issue**
- As the issue progresses, update its **Status Label**:
  - **`status/needs review`** → Needs input before work begins.
  - **`status/in progress`** → Someone is actively working on it.
  - **`status/blocked`** → Work cannot proceed due to dependencies.
  - **`status/awaiting feedback`** → Waiting for a response from the author or team.
  - **`status/ready for testing`** → Code is complete and needs verification.

**Example:**
_A contributor is fixing a bug → Change from **`status/needs review`** → **`status/in progress`**._

---

## **4. Mark Resolution When Issue is Closed**
- Once an issue is resolved, apply a **Resolution Label** before closing it:
  - **`resolution/fixed`** → The problem was resolved successfully and closed.
  - **`resolution/won’t fix`** → Acknowledged but will not be fixed.
  - **`resolution/duplicate`** → Similar to another reported issue.
  - **`resolution/invalid`** → Incorrect or not an actual issue.
  - **`resolution/works as intended`** → Not a bug; intended behavior.

**Example:**
_A reported bug was fixed → Apply **`fixed`** and close the issue._

---

## **5. Encourage Community Participation**
- Use **Community Labels** to encourage contributions:
  - **`discussion`** → Open-ended brainstorming or planning.
  - **`stale`** → Has been inactive for an extended period.
  
**Example:**
_An feature request that was inactive for a long time → Assign **`type/feature request`** + **`stale`**._

---

## **Example Workflow**
1. A user reports that the login feature is broken.

   - Label: **`type/bug`**, **`priority/high`**, **`status/needs review`**.

2. A maintainer reviews the issue, confirms it, and assigns a developer.

   - Label changes: **`status/in progress`**.

3. Developer completes the fix and submits a pull request.

   - Label changes: **`status/ready for testing`**.

4. The fix is tested and merged.

   - Label changes: **`resolution/fixed`**.

   - Issue is closed.


By consistently applying labels and updating them as issues progress, your GitHub repository will remain **organized, transparent, and efficient** for both maintainers and contributors. 🚀