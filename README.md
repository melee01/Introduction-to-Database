# SC2207 Database Project – Property Management System  

This repository contains the database project developed as part of **SC2207 / CZ2007: Introduction to Databases** at **Nanyang Technological University (NTU)**.  
The project implements a **Property Management System** for **MProps Digital Pte Ltd**, a platform where property agents can post listings, customers can browse properties, initiate chats, book appointments, and complete property transactions:contentReference[oaicite:0]{index=0}.  

---

## Project Overview  

The system was designed and implemented through several lab sessions:  

- **Lab 1 – ER Diagram**  
  - Constructed the conceptual **Entity-Relationship (ER) diagram**.  
  - Defined key assumptions about properties, agents, agencies, and customers:contentReference[oaicite:1]{index=1}.  

- **Lab 3 – Normalized Database Schema**  
  - Converted the ER diagram into relational schemas.  
  - Applied **3NF normalization**, ensuring removal of redundancy.  
  - Documented functional dependencies (FDs) and decompositions:contentReference[oaicite:2]{index=2}.  

- **Lab 5 – Final Implementation & Queries**  
  - Implemented the database in **SQL Server** using **DDL commands**.  
  - Populated tables with realistic test data (via SQL + Python scripts).  
  - Developed **SQL queries** to support real-world scenarios (e.g., listing searches, engagement tracking, top agents).  
  - Created **triggers** to update engagement statuses dynamically:contentReference[oaicite:3]{index=3}.  

---

## Features  

- **Property Listings**  
  - Supports sales and rental listings.  
  - Rental properties include short-term and long-term options.  

- **Users & Roles**  
  - Customers, Agents, and Owners with unique attributes.  
  - Agencies with managers and multiple affiliated agents.  

- **Engagement & Interaction**  
  - Customers can initiate chats, schedule appointments, and leave reviews.  
  - Engagements evolve from *New* → *Viewed* → *In Discussion* → *Purchased*.  

- **SQL Queries Implemented**:contentReference[oaicite:4]{index=4}:contentReference[oaicite:5]{index=5}  
  - Properties for sale in *Ang Mo Kio* with tenure ≤ 20 years.  
  - Property statistics grouped by type & furnishing status.  
  - Annual sales reports by agency & manager.  
  - Customer follow-ups for unfinished rental deals.  
  - Top 3 engaging agents per year.  
  - Automatic **trigger-based engagement updates**.  

---

## Tech Stack  

- **Database:** Microsoft SQL Server  
- **Modeling:** ER diagrams (Canva)  
- **Normalization:** 3NF applied to all relations  
- **Languages:** SQL, Python (for data population):contentReference[oaicite:6]{index=6}  

---

## Setup Instructions  

1. Clone this repository:  
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
2. Import the SQL DDL scripts from Lab 5 (ddl/ folder if separated).
3. Run the data population scripts (scripts/ folder).
4. Execute the queries (queries/ folder) to test functionality.

---

## Contributors
- Denzel Elden Wijaya
- Dosi Veer
- Lionel Owen Wijaya
- Melisa Lee
- Vannes Wijaya
- Wang Min-Jen
