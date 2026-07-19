# Engineering Methodology

## Purpose

This document defines the engineering methodology used throughout OpsForge.

Every troubleshooting module follows the same structured approach regardless of the technology involved.

The goal is to solve problems using evidence, logical reasoning, and the least invasive solution rather than assumptions or guesswork.

---

## The OpsForge Engineering Process

### Step 1 – Understand the Problem

Clearly define the issue before attempting any repairs.

Questions include:

- What is happening?
- When did it begin?
- Is the issue reproducible?
- Has anything recently changed?

Never assume two similar symptoms have the same cause.

---

### Step 2 – Collect Evidence

Gather only the information required to make the next decision.

Examples include:

- Error messages
- Event logs
- System version
- Disk space
- Network connectivity
- Service status

Evidence should guide every troubleshooting decision.

---

### Step 3 – Build a Theory

Based on the evidence collected, determine the most likely cause.

Avoid jumping directly to repairs without first forming a logical explanation.

---

### Step 4 – Test the Theory

Perform the smallest, safest action capable of confirming or disproving the theory.

Start with low-risk actions before moving to more invasive repairs.

---

### Step 5 – Verify Resolution

Confirm that the original issue has been resolved.

A repair is only successful when the user can complete the original task without error.

---

### Step 6 – Document the Outcome

Record:

- Root cause
- Evidence collected
- Actions performed
- Verification results
- Lessons learned

Documentation prevents repeated investigations and improves future troubleshooting.

---

## Core Principles

OpsForge follows these engineering principles:

- Evidence before action.
- Least invasive first.
- One change at a time.
- Verify every repair.
- Never assume.
- Understand before fixing.
- Document every meaningful finding.
