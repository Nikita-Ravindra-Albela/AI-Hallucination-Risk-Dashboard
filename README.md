# AI-Hallucination-Risk-Dashboard
<img width="559" height="80" alt="image" src="https://github.com/user-attachments/assets/612bf1a6-3baa-488e-870f-aaf56a8b34ea" />

## Overview

As organizations increasingly adopt AI tools for business decision-making, a critical risk emerges: AI hallucinations confident but incorrect or incomplete outputs that can silently influence high-impact decisions.

This project focuses on AI Governance from a business perspective, not a technical one.
Instead of asking “Is the AI model accurate?”, it asks:

“When does AI become dangerous for business decisions?”

Using simulated enterprise-scale data, this analysis quantifies:

AI hallucination risk

Overconfidence in AI-generated insights

Business and revenue exposure due to risky AI usage

The outcome is an AI Risk Scoring framework that leadership teams can use to define safe vs unsafe AI usage boundaries.

## What Is AI Governance? (Business View)

AI Governance refers to the frameworks, policies, and controls that ensure AI systems are used responsibly, safely, and in alignment with business objectives.

From a business analytics lens, AI governance answers questions like:

Should AI be used for strategic decisions?

Which decisions require human review?

How much revenue is exposed to AI errors?

Where does AI confidence exceed reliability?

This project demonstrates how data analysts can actively contribute to AI governance, even without building AI models themselves.

## Problem Statement

AI tools are increasingly used across departments such as Finance, Sales, HR, and Operations.

However:

AI responses often sound confident

Decision-makers may not validate assumptions

High-impact decisions may rely on flawed AI insights

This project measures and visualizes AI hallucination risk across business decisions.

## Dataset

Type: Synthetic enterprise data

Rows: 50K AI usage records

Key fields:

Department

Decision type (Strategic / Operational)

Decision impact value (₹)

AI confidence score

Date of decision

Synthetic data was intentionally used to:

Avoid template datasets

Enable realistic risk simulations

Model scenarios not commonly tracked in organizations

🧩 Business Definition of Hallucination

This project intentionally avoids a technical definition.

Hallucination (Business Definition):

An AI response is considered a hallucination if:

The AI is highly confident AND

The answer is factually incorrect OR

Key business assumptions are missing

This allows risk to exist even when the AI is partially correct.

## Methodology
1️. Data Modeling (SQL)

Created a canonical SQL view: v_ai_hallucination

Simulated:

Factual correctness

Missing assumptions

Derived a business-level hallucination_flag

2️. Core Risk Metrics

Hallucination Rate

Overconfidence Index

Assumption Gap Score

All metrics were normalized and combined into a single AI Risk Score (0–100).

3️. Risk Segmentation

Risk was analyzed by:

Department

Decision type (Strategic vs Operational)

Decision impact buckets

Time trends

4️. Policy Simulation (What-If Analysis)

Simulated a governance policy:

“Introduce mandatory human review for strategic decisions above ₹10L.”

Measured:

Reduction in hallucination exposure

Reduction in revenue at risk

## Dashboard Highlights (Power BI)

Key dashboard sections:

Overall AI Hallucination Rate

AI Risk Score

Revenue at Risk (₹)

High-risk departments and decisions

Impact bucket analysis

Before vs After governance policy simulation

This dashboard is designed for executive decision-making, not just reporting.

## Key Insights

~35% of AI-influenced decisions showed hallucination risk

High-impact strategic decisions had the highest risk concentration

Finance and Sales contributed the majority of revenue exposure

Introducing a ₹10L human-review policy reduced hallucination exposure by ~80–90%

Potential risk reduction value exceeded ₹200+ Cr (simulated)

## Tools & Skills Used

SQL (SQL Server)

Views

CASE logic

Risk aggregation

Python

Risk modeling

Scenario simulation

Metric validation

Power BI

DAX measures

Policy simulation

Executive dashboards

Business Analytics

Metric design

Risk modeling

AI governance thinking

## How This Project Can Be Extended

Add real AI output evaluation data

Introduce department-specific risk thresholds

Build automated AI usage policy alerts

Integrate with MLOps or AI monitoring systems

## About the Author

Nikita Albela
MBA (HR & Business Analytics)
Aspiring Data Analyst with a strong focus on:

Business-first analytics

Risk modeling

AI governance & decision intelligence
