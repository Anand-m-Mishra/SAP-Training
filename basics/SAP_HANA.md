# What is SAP HANA?
- High Performance ANalytics Applicance.
- In-Memory Database: Stores data is RAM instead of disk storage.
- column oriented: A column-oriented database stores data column-wise instead of row-wise like traditional relational databases. This structure improves performance for analytical queries that process large amounts of data.
Example:
Row-Oriented Storage:
ID	Name	Amount	Date
1	Alex	100	2024-01-01
2	Bob	200	2024-01-02
Stored as:
1, Alex, 100, 2024-01-01 | 2, Bob, 200, 2024-01-02

Column-Oriented Storage:
ID	Name	Amount	Date
1	Alex	100	2024-01-01
2	Bob	200	2024-01-02
Stored as:
1, 2 | Alex, Bob | 100, 200 | 2024-01-01, 2024-01-02

- Supports both OLAP AND OLTP workloads in a single system: A database system that supports both OLAP (Online Analytical Processing) and OLTP (Online Transaction Processing) is called a Hybrid Transactional/Analytical Processing (HTAP) system. This allows real-time analytics on live transactional data without needing a separate data warehouse.

## SAP HANA Architecture
- Column-based, in-memory storage for high-speed transactions.
- ACID compliance (Atomicity, Consistency, Isolation, Durability).
- Multi-tenancy - Multiple databases share the same system securely:Multi-tenancy is a software architecture where a single instance of an application serves multiple tenants (users, organizations, or customers). Each tenant shares the same infrastructure (e.g., database, application server) but has isolated data, configurations, and access controls.
- Scalability - Supports terabytes of data and distributed processing.
- Data management - Handles hot (frequent), warm (occasional), and cold (rare) data efficiently.