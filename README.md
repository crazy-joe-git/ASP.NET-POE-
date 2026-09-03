# Race_System

## Project Overview
RaceDay is a role-based RESTful sports event management platform designed specifically for South African road running, walking, and cycling events. The platform bridges the gap between event management and athlete participation by providing an intuitive system for race creation, category selection, participant enrolments, and official finish-time tracking. Built with strict role separation between **Organisers** and **Participants**, RaceDay ensures secure, streamlined operations for every race day.

---

## Part 1: Architecture & System Design
In Part 1 of the project, we establish the theoretical and structural foundation necessary to build a scalable web application. This phase focuses on domain modeling, database design, API planning, and automated project setup:

* **Domain Requirement Analysis:** Identifying user roles, permissions, and core business workflows.
* **Database Modeling & Scripting:** Designing a normalized relational database schema to support secure authentication, event structures, enrolments, and result logs.
* **REST API Endpoint Planning:** Structuring a clean, RESTful API specification mapping routes, HTTP methods, request payloads, and expected response codes across all system endpoints.
* **Version Control & Repository Setup:** Initializing the GitHub repository with automated workflow checks and standardized documentation.

---

## Database Architecture: ERD & SQL Script
Understanding the data architecture is critical to understanding how RaceDay operates behind the scenes.

* **Entity Relationship Diagram (ERD):** The ERD acts as the visual blueprint of the system. It maps out how different entities—such as `Users`, `Events`, `Categories`, `Enrolments`, and `Results`—relate to one another. It visually demonstrates primary-to-foreign key connections and cardinality, guaranteeing that data integrity is maintained (for example, ensuring an enrolment cannot exist without a valid participant and event race).
* **Database Creation & Seed Script:** The SQL script brings the visual ERD to life by executing the data definition language (DDL) required to build the database tables, enforce constraints, and establish foreign keys. It also includes seed data—pre-populated sample records featuring sample organisers, participants, events, and categories. This allows developers and assessors to immediately spin up, test, and query a working database instance without manual data entry.

---

## Summary & What's Ahead in Part 2
Part 1 successfully completes the architectural blueprint for RaceDay, delivering a verified database schema, a complete API endpoint specification, and a repository ready for development. With a rock-solid data model and clear contract definitions established, the project is prepped for full backend implementation.

In **Part 2**, we will transform these blueprints into a fully functional backend service built with ASP.NET Core and Entity Framework Core. Part 2 will feature:
* Secure authentication and role-based access control.
* Complete implementation of all planned API endpoints.
* Database migration and ORM integration using EF Core.
* Thorough unit testing and endpoint validation to ensure a robust, production-ready REST API.
