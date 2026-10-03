# WhatNext Vision Motors - Salesforce Implementation

![Salesforce](https://img.shields.io/badge/Salesforce-Lightning-00A1E0?style=for-the-badge&logo=salesforce)
![Platform](https://img.shields.io/badge/Platform-Developer%20Edition-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

## 🚗 Project Overview

**WhatNext Vision Motors** is a comprehensive Salesforce-based vehicle management and Customer Relationship Management (CRM) solution. It centralizes vehicle, dealer, customer, and order operations into a single platform. The system leverages Salesforce automation features like Record-Triggered Flows, Apex Triggers, and Scheduled Batch Jobs to automate order processing, dealer assignment, stock validation, and test drive scheduling.

---

## 📌 Problem Statement

Vehicle dealerships face challenges due to fragmented data across spreadsheets, manual order processing, delayed dealer assignments, and stock discrepancies. This manual workflow leads to operational delays, order errors, and customer dissatisfaction.

---

## 💡 Solution & Features

- **Centralized Data Management**: Custom Salesforce objects to track Vehicles, Dealers, Customers, Orders, Test Drives, and Service Requests.
- **Automated Dealer Assignment**: Record-triggered flow automatically assigns the nearest dealer based on customer location upon order placement.
- **Stock Validation & Auto Confirmation**: Apex Triggers and Batch Jobs handle stock verification and update order statuses dynamically.
- **Scheduled Reminders**: Flows send automated notifications and email reminders for upcoming test drives.
- **Dedicated Lightning App**: Custom Lightning App with tailored navigation tabs for seamless operational management.
- **Analytics & Dashboards**: Real-time reporting on vehicle orders, dealer performance, and stock inventory.

---

## 🏗 System Architecture & Technology Stack

| Layer | Technology |
| :--- | :--- |
| **User Interface** | Salesforce Lightning Experience, Custom Lightning App |
| **Business Logic** | Salesforce Flows, Validation Rules |
| **Database** | Salesforce Custom Objects & Fields |
| **Backend Processing** | Apex Classes, Apex Triggers, Batch Apex, Scheduled Apex |
| **Reporting** | Salesforce Reports & Dashboards |

---

## 🗂 Custom Objects & Data Model

- **Vehicle (`Vehicle__c`)**: Stores vehicle models, specifications, pricing, and stock status.
- **Dealer (`Vehicle_Dealer__c`)**: Stores dealership details, locations, contact info, and assigned regions.
- **Customer (`Vehicle_Customer__c`)**: Tracks customer profile data and contact info.
- **Order (`Vehicle_Order__c`)**: Manages customer orders, order dates, status, and linked dealer/vehicle details.
- **Test Drive (`Vehicle_Test_Drive__c`)**: Schedules test drive bookings and tracking statuses.
- **Service Request (`Vehicle_Service_Request__c`)**: Tracks customer maintenance and vehicle service requests.

---

## ⚙️ Core Automation Components

1. **Record-Triggered Flow (`Auto_Assign_Dealer`)**: Triggered on `Vehicle_Order__c` creation to fetch nearest dealer data and assign it automatically.
2. **Apex Trigger Handler (`VehicleOrderTriggerHandler`)**: Validates stock availability before order insertion/update.
3. **Batch Apex (`VehicleOrderBatch`)**: Scans pending orders against replenished inventory and updates status to `Confirmed`.
4. **Scheduled Apex (`VehicleOrderBatchScheduler`)**: Executes the batch job periodically.

---

## 👥 Team Details

- **College**: Alpha College of Engineering, Thirumazhisai, Chennai
- **Team ID**: `SWTID-2026-6852`
- **Team Lead**: Immanuel Luther K (`immanuelk117@gmail.com`)
- **Team Members**:
  - Rishi Kumar R (`rishikumarr2101@gmail.com`)
  - Gowtham (`gkesavankoonar@gmail.com`)
  - Kannan (`kannanrajavelu296@gmail.com`)

---

Team ID

SWTID-2026-6852

Demo Link:https://drive.google.com/drive/folders/1ziI0n8KXHDQ2DM6zWA9wNN3Rs21jEH_4

## 📜 License

This project is created for academic and demonstration purposes as part of the Salesforce Implementation project.
