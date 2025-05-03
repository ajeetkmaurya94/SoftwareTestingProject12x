## **Software Testing Life Cycle (STLC) **
**Software Testing Life Cycle (STLC)** is a sequence of different activities performed during the software testing process.

![image.png](https://eraser.imgix.net/workspaces/RklhCFoOSNu4Biov8Rqg/WWS31TdyovhjTB1TVo9v2jWpPei1/-6am9pI0gVVezUqIAhJgi.png?ixlib=js-3.7.0 "image.png")

#### **Requirement Analysis**
- Quality assurance team understands the requirements like what is to be tested.
- If anything is missing or not understandable then quality assurance team meets with the stakeholders to better understand the detail knowledge of requirement.
  -> SRS, Google Docs.  





**Test Planning**

- In this phase manager of the testing team calculates estimated effort and cost for the testing work 
- QA Leads 
- [﻿sdet.live/project2](https://sdet.live/project2) 
- https://sdet.live/genai
- Gen via AI - [﻿chatgpt.com/canvas/shared/67c6663548f48191b1bd56807afc93d6](https://chatgpt.com/canvas/shared/67c6663548f48191b1bd56807afc93d6) 


### Task  
1. Before -> Create Manually in Google Docs. You can use this template - [﻿docs.google.com/document/d/1JDF1xfkYxu0gPoyyf_ZstLLOoAgjCxu5/edit](https://docs.google.com/document/d/1JDF1xfkYxu0gPoyyf_ZstLLOoAgjCxu5/edit) 
2. Try this -> [﻿chatgpt.com/share/6815a1e0-067c-8009-944b-8d48a844ab90](https://chatgpt.com/share/6815a1e0-067c-8009-944b-8d48a844ab90) 


**Comprehensive Test Plan for app.vwo.com (A/B Testing SaaS Platform)**

---

**1. Objective**

- To validate the functional, non-functional, and integration quality of app.vwo.com’s A/B testing platform.
- Ensure accurate reporting, stable campaign management, and reliable integrations.
- **Success Criteria:** 95% test pass rate, response time <2s for major workflows, zero Sev1/Sev2 defects in production.
- **Stakeholder Expectations:** Deliver an intuitive, accurate experimentation platform supporting marketing, product, and customer success goals.
---

**2. Scope**

- **In Scope:**
    - Core functionalities: Project creation, Variant creation, Campaign activation, Result reporting.
    - Integrations: Google Analytics, Tag Managers.
    - Device/Browser coverage (see Section 5)
- **Out of Scope:**
    - Backend infrastructure testing (owned by DevOps)
    - Third-party services beyond integration touchpoints
---

**3. Major Workflows**

- User Registration/Login
- Project Setup (Page Targeting)
- Variant Creation and Editor usage
- Campaign Activation/Deactivation
- Report Analysis & Exporting
- Integrations configuration and validation
---

**4. Test Environments**

| Device | OS | Browsers |
| ----- | ----- | ----- |
| Desktop | Windows 10 | Chrome, Firefox, Edge |
| MacBook | macOS | Safari, Chrome |
| Mobile | iOS, Android | Chrome, Safari |
- **Test Data Requirements:**
    - Dummy websites
    - Sample campaigns (A/B, Split URL, Multivariate)
    - Dummy user personas and accounts
---

**5. Defect Reporting Procedure**

- Tool: JIRA
- **Severity & Priority Matrix**
 | Severity | Description | Response | Resolution |
 |----------|-------------|----------|------------|
 | Sev 1 | Critical blocker | 1 hr | 8 hrs |
 | Sev 2 | Major defect | 4 hrs | 24 hrs |
 | Sev 3 | Minor defect | 24 hrs | 3 days |
 | Sev 4 | Cosmetic/Trivial | 48 hrs | Next sprint |
---

**6. Test Strategy**

- **Functional Testing:** Manual (TestRail)
- **Automation Testing:**
    - Selenium (UI)
    - REST Assured (API)
    - Allure (Reporting)
- **Performance Testing:** JMeter (Load Testing 1000 concurrent users)
- **Accessibility Testing:** Axe, WCAG 2.1 compliance
- **Security Testing:**
    - SQL Injection, XSS testing
    - Session management and token expiry tests
---

**7. Test Schedule**

| Task | Start Date | End Date | Owner |
| ----- | ----- | ----- | ----- |
| Test Plan Creation | May 3 | May 5 | Test Lead |
| Test Case Design | May 6 | May 12 | QA Team |
| Test Execution | May 13 | May 25 | QA Team |
| Reporting & Closure | May 26 | May 28 | Test Lead |
---

**8. Test Deliverables**

- Test Plan Document
- Test Cases & Checklists
- Traceability Matrix
- Defect Reports
- Daily/Weekly Status Reports
- Test Summary Report
- Lessons Learned Document
---

**9. Entry and Exit Criteria**

- **Entry:** Signed-off requirements, stable test environment, test data available
- **Exit:** 95% test cases passed, no Sev1/Sev2 open defects, stakeholder sign-off
---

**10. Tools**

- Test Management: TestRail
- Automation: Selenium, REST Assured
- Performance: JMeter
- Accessibility: Axe
- Reporting: Allure, Confluence
- Communication: Slack, Zoom
- Defect Tracking: JIRA
---

**11. Risks and Mitigation**

| Risk | Impact | Mitigation |
| ----- | ----- | ----- |
| Integration downtime | High | Use mock APIs, retries |
| Unstable test environments | Medium | Parallel environments setup |
| Delayed builds | High | Early smoke validation, daily syncs |
---

**12. Traceability Matrix (Sample)**

| Requirement ID | Test Case ID | Defect ID |
| ----- | ----- | ----- |
| REQ-01 | TC-01, TC-02 | BUG-101 |
| REQ-02 | TC-03 | - |
---

**13. Compliance and Standards**

- WCAG 2.1 (Accessibility)
- OWASP Top 10 (Security)
- ISO/IEC 25010 (Quality Model reference)
---

**14. Approvals**

| Name | Role | Approval Date | Signature |
| ----- | ----- | ----- | ----- |
| Pramod Dutta | Test Lead | YYYY-MM-DD | ___ |
| Product Manager | Stakeholder | YYYY-MM-DD | ___ |
| QA Manager | QA Reviewer | YYYY-MM-DD | ___ |
