# Advanced Database Management System
## Oracle – SQL Server Migration & Access Integration Project
---
## Project Overview
This project demonstrates the migration, redesign, and integration of a relational database system across multiple platforms:
- SQL Server → Oracle Database
- Oracle backend + MS Access frontend
- ER modeling & relational normalization
- Trigger-based integrity enforcement
- ODBC connectivity configuration

The objective was to simulate a cross-platform enterprise database deployment and integration scenario.

---
## Architecture Overview
**Backend:** Oracle Database (SID: orcl2355)
**Frontend:** MS Access (ODBC-linked)
**Migration Source:** SQL Server schema
**Tools Used:**
- SQL*Plus
- Oracle SQL Developer
- Oracle Data Modeler
- ODBC (32-bit & 64-bit configuration)
---
## 1️⃣ Schema Migration (SQL Server → Oracle)
- Converted DDL scripts from SQL Server to Oracle-compatible syntax
- Modified:
  - Tablespace allocation
  - User roles & privileges
  - Data types (e.g., IDENTITY → SEQUENCE + TRIGGER)
  - Insert syntax differences
- Created and cleaned schema using automated SQL scripts

Demonstrated:
- Cross-platform SQL adaptation
- Database user management
- Schema lifecycle management
---
## 2️⃣ Data Modeling & ER Design
- Reverse-engineered database schema into Oracle Data Modeler
- Generated Physical ER Diagram (PDF included)
- Validated:
  - 7 relational tables
  - 1 dedicated tablespace
  - 1 database user
- Ensured proper primary / foreign key relationships

Demonstrated:
- Relational modeling
- Normalization principles
- Physical schema validation
---
## 3️⃣ Views & Multi-Valued Field Resolution
- Identified multi-valued attributes
- Restructured schema to meet normalization standards
- Created Views to abstract complex joins
- Implemented DML logic via Oracle views

Demonstrated:
- Logical data abstraction
- Schema refinement
- Controlled data manipulation
---
## 4️⃣ Trigger Implementation

Created triggers to:
- Enforce referential integrity
- Automate field updates
- Maintain transactional consistency
- Replace SQL Server auto-increment logic

Demonstrated:
- Event-driven database logic
- Backend automation
- Transaction control
---
## 5️⃣ ODBC & MS Access Integration

Configured:
- 32-bit and 64-bit ODBC connections
- Oracle listener (localhost:1521/orcl2355)
- Linked Oracle tables to MS Access frontend

Result:
- Access UI directly interacts with Oracle backend
- Real-time DML operations via linked tables

Demonstrated:
- Cross-platform integration
- Enterprise-style backend/frontend separation
- Database connectivity configuration
---
## 6️⃣ Transaction & Autocommit Management
- Verified Oracle autocommit behavior
- Managed explicit COMMIT for DML
- Tested rollback & transactional control

Demonstrated:
- ACID transaction understanding
- Operational database management
