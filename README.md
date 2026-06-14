# Operations & QA — Document / Receipt Processing

## Overview

This repository contains a complete evaluation task created for the **Kensei Project**.

The task simulates a realistic **document and receipt processing workflow** where mixed operational records, uploaded evidence, workflow artifacts, and distractor information must be analyzed to determine the correct recommendation outcomes.

The objective is to challenge the model with reconciliation, prioritization, policy interpretation, and non-execution constraints.

---

## Task Classification

| Category | Value                         |
| -------- | ----------------------------- |
| L1       | Operations & QA               |
| L2       | Document / Receipt Processing |

---

## Task Objective

Review a mixed batch of:

* Receipts
* Invoices
* Supporting files
* Review notes
* Workflow tracking records

Determine:

* What should move forward
* What requires review
* What must stay blocked
* What requires no action

Constraints:

* Do not approve
* Do not reimburse
* Do not modify records
* Do not change workflow state
* Do not send communications
* Follow-ups must remain draft-only

---

## Repository Structure

```text
task_folder/
│
├── prompt.txt
├── rubric.json
├── test_outputs.py
├── test_weights.json
├── golden_steer_flow.md
├── task.yaml
│
├── data/
│   ├── relevant/
│   └── irrelevant/
│
├── mock_data/
│   ├── gmail-api/
│   ├── google-drive-api/
│   ├── slack-api/
│   ├── notion-api/
│   └── monday-api/
│
└── persona/
```

---

## APIs Used

This task intentionally uses exactly **five APIs**.

1. gmail-api
2. google-drive-api
3. slack-api
4. notion-api
5. monday-api

These APIs are used for retrieval, evidence correlation, workflow awareness, and recommendation generation.

---

## Evaluation Design

The task evaluates:

* Document reconciliation
* Duplicate detection
* Historical overlap detection
* Policy compliance
* Threshold validation
* Workflow awareness
* Evidence prioritization
* Draft-only recommendations

---

## Authority Order

When evidence conflicts:

1. Expense Policy Handbook
2. Receipt Processing SOP
3. Approval Rules
4. Receipt Registry
5. Processing State
6. Reconciliation Records
7. Structured Inputs
8. Workflow Tracking
9. Communications
10. Notes

---

## Included Challenges

* Duplicate receipt traps
* Historical reimbursement overlap
* Missing documentation
* Threshold violations
* Workflow constraints
* Distractor files
* Non-authoritative discussions

---

## Success Criteria

The solution should:

* Prioritize authoritative records
* Detect duplicate submissions
* Respect workflow state
* Avoid execution
* Produce recommendation-only outputs

---

## Distractor Content

The repository intentionally includes unrelated files to increase retrieval difficulty.

Examples:

* Sales exports
* Marketing reports
* Dashboard configs
* Office documents
* Archive summaries
* Newsletters

These files must not drive decisions.

---

## Submission Notes

This repository was created as a complete task package following the required submission structure.

Ensure all files remain unchanged before submission.

---
