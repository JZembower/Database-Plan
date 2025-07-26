# Database System Modernization for Flix2You

This project outlines a comprehensive proposal by Griffin Tech Innovations to modernize Flix2You's outdated technology infrastructure, particularly its database system. The goal is to enhance data collection, storage, and reporting capabilities to improve competitiveness in the evolving movie-viewing industry.

## Authors

Jonah Zembower, Daniel Cavanaugh, Jimmy Baxter, Niko Apodiakos

## Date

April 20, 2023

## Executive Summary

Flix2You, a company in the competitive movie-viewing industry, is currently facing challenges due to outdated technology and inefficient data management. Griffin Tech Innovations proposes an organized, efficient, and sustainable database system that leverages modern technologies to provide actionable insights into consumer behavior. This solution is designed for cost-effectiveness, timely implementation, and a high return on investment, aiming to transform Flix2You into a competitive streaming service.

## Project Overview

The project addresses Flix2You's inability to keep pace with market trends, such as the shift from DVDs to online streaming and digital services (apps, games). The current data infrastructure hinders timely and accurate reporting, impeding the company's ability to understand and appeal to consumers, leading to a plateau in customer acquisition.

Our solution focuses on:
* Improving database administration to ease end-user access while restricting information to necessary users.
* Implementing a new database management software package to enhance speed, protection, and data backup.
* Restructuring the website for administrative viewing and implementing an e-commerce platform for consumers.

## Database Administration

A full-time Database Administrator (DBA) is recommended, proficient in MySQL, Oracle, and DB2. The DBA's responsibilities include:
* Managing the Database Management System (DBMS) and ensuring proper functionality.
* Maintaining privacy and security standards.
* Performing server backups.
* Promoting DBMS sustainability through updates and employee training.

The new database will be managed with Microsoft SQL Server 2022 and utilize Microsoft Azure for cloud capabilities, ensuring data fluency and secure storage. The migration from the existing Microsoft SQL Server 2008 will be a smooth transition, planned to minimize impact on operations.

## Data Organization and Normalization

The existing Flix2You database suffers from unnecessary results and redundancies. Griffin Tech Innovations proposes updating the table structure to the Third Normal Form (3NF). This involves:
* Converting initial tables from First Normal Form (1NF).
* Removing all partial dependencies to achieve Second Normal Form (2NF).
* Eliminating transitive dependencies to reach 3NF.

This normalization guarantees data integrity and consistency by removing insertion, update, or deletion anomalies, leading to a more reliable and effective database interaction.

## Database Backup and Recovery

A robust three-factor backup and recovery plan is proposed:
1.  **Secure Storage**: Utilizing Microsoft SQL Server 2022 and Microsoft Azure for scalable and secure storage of database backups.
2.  **Scheduled Backups**: A full daily backup job at 2:00 AM ET, with daily transaction log backups every two hours from 6:00 AM ET to 12:00 AM ET.
3.  **Disaster Recovery**: Daily backups of Microsoft Azure locations and copies of the Microsoft SQL database server provide options for quick restoration of the entire database server in case of failure.

The DBA will monitor these jobs daily to ensure successful execution and data security.

## Data Access and Security

Data security is a layered approach managed by a collaborative team (DBA, System Administrator, Network Administrator, Webmaster):
* **Website/Network Security**: Implementing firewalls, intrusion detection software, and encryption, along with strict customer user permissions and regular security patches to web servers and applications.
* **System Security**: Managing internal access via Microsoft Windows Active Directory and Group Policies, limiting direct system access to administrator groups only.
* **Database Security**: Restricting read/write access to a select group of users, with no direct access for customers or various internal employee groups. Daily monitoring of database server logs ensures critical patches and updates are applied.

A detailed customer privacy statement is available on the Flix2You website, outlining data collection, use, disclosure, and security measures. Employees with access to customer information undergo background checks and sign disclosures.

## Database Dashboard and Analytics

A Data Mart will be created with new tables specifically designed for reporting. A nightly ETL (Extract, Transform, Load) process will pull data from the operational database into the Data Mart. Microsoft Power BI will be used to create user-friendly, real-time dashboards that provide actionable insights to different user groups based on their specific needs.

## Project Management

The project timeline is flexible and divided into three phases:

* **Phase One: Analysis (Two Weeks)**: Meeting with Flix2You management and employees to discuss business rules and goals, followed by database design and software ordering.
* **Phase Two: Development (Two Weeks)**: Revising database tables, coding, loading test data, writing queries, and generating test reports. This phase includes extensive testing for reliability.
* **Phase Three: Implementation (Three Weeks)**: Installing hardware and software, setting up accounts with Microsoft Azure and SQL, migrating existing data, instituting backup services, and comprehensive system testing. The final week is dedicated to training Flix2You management and employees.

### Budget

The total projected budget for the project is **$163,435**, comprising:
* **Total Labor Budget**: $42,000 (for Research/Writer/Editor, Programmer, Graphic Artist, Data Analyst).
* **Total Supply Budget**: $121,435 (including Microsoft Azure, Microsoft SQL Server 2022, Microsoft Power BI, and HP ZBook Fury 17 G8 workstations).

## Legal Issues

Flix2You maintains a strict Privacy Policy detailing the collection, use, disclosure, and transfer of customer information, accessible on its website. It also has Terms and Conditions for Use, outlining refund policies and consequences for policy violations, with a strong emphasis on security protocols and data integrity.

## Files in the Repository

* `Flix2You Paper.docx`: The comprehensive proposal document detailing all aspects of the database system modernization project.
