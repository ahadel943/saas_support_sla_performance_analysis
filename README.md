# **SaaS Support SLA Performance Analysis**
## **One Question Projects — Project 06**

## **Project Overview**
This project analyzes customer support ticket resolution performance in a simulated SaaS environment, focusing on Service Level Agreement (SLA) compliance.

Using a dataset of 3,000 support tickets, the analysis examines resolution outcomes against defined SLA targets to identify patterns in SLA breaches across issue categories and operational dimensions.

The project follows a structured analytics workflow, from data quality assessment and transformation using Excel Power Query to KPI development and analysis using the Excel Data Model, Power Pivot, and PivotTables.

## **Business Problem**
SaaS companies rely on customer support teams to resolve issues within defined service targets. However, differences in issue complexity, ticket priority, and operational workload may contribute to inconsistent resolution performance.

Without a structured analysis of support ticket data, management may struggle to identify which issue categories experience the highest rates of SLA breaches and where further operational investigation is needed.

This limits the ability to prioritize improvement efforts and investigate the factors contributing to delayed ticket resolution.

## **Project Goal**
The goal of this project is to evaluate customer support resolution performance by measuring SLA compliance and comparing breach rates across issue categories.

The analysis aims to identify the categories that warrant further investigation, supported by ticket volumes and relevant operational indicators, to help management prioritize potential areas for improvement.

The analysis will focus on resolved tickets when calculating the primary SLA breach rate, while open and cancelled tickets will be handled separately according to their status.

## **Project Business Question**
**Which customer support issue categories have the highest SLA breach rates, and where should management prioritize further investigation?**

## Executive Summary
**No Summary Yet — To Be Completed After Analysis.**

## **Dataset Description**
The dataset contains **3,000** support tickets simulated for a SaaS company operating in the software services industry. It consists of **13** columns covering ticket creation and resolution timestamps, issue categories, ticket priorities, support channels, support teams, customer subscription plans, response and resolution times, and Service Level Agreement (SLA) compliance status.

The dataset supports the analysis of SLA Breach Rate across different support issue categories, helping identify categories with elevated breach rates and determine where management should prioritize further operational investigation.

| Column | Description |
| ------ | ----------- |
| ticket_id | Unique identifier assigned to each support ticket. |
| created_at | Date and time when the support ticket was created. |
| resolved_at | Date and time when the ticket was resolved, where applicable. |
| issue_category | Category of the issue reported, such as billing and payments, login and access, or bugs and errors. |
| priority | Priority level assigned to the ticket, ranging from P1 (highest priority) to P4 (lowest priority). |
| channel | Channel through which the ticket was submitted, such as email, live chat, web form, or in-app support. |
| support_team | Support team responsible for handling the ticket. |
| customer_plan | Subscription plan associated with the customer, such as Free, Basic, Professional, or Enterprise. |
| status | Current ticket status, recorded as Resolved, Open, or Cancelled. |
| first_response_minutes | Time elapsed, in minutes, before the support team provided the first response. |
| resolution_minutes | Time elapsed, in minutes, between ticket creation and resolution, where applicable. |
| sla_target_hours | Target resolution time, in hours, assigned to the ticket based on its priority level. |
| sla_status |	SLA compliance classification of the ticket, indicating whether it was resolved within the target, breached the target, remains open and overdue, is pending within the target, or was cancelled. |

## **EDA & Baseline KPIs**
An initial exploratory analysis was conducted to validate the dataset structure, review SLA status distributions, and establish baseline performance metrics. Out of **3,000** support tickets, **2,491** were resolved, with **622** breaching their SLA targets, resulting in an **overall SLA breach rate of 24.97%**. A preliminary comparison across issue categories identified Bugs & Errors and Integrations as the categories with the highest SLA breach rates and the largest numbers of breached tickets, highlighting them as priority areas for further investigation.


