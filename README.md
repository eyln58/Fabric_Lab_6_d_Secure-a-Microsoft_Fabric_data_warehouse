# 🔐 Securing a Microsoft Fabric Data Warehouse

This repository documents the completion of a hands-on lab focused on securing data access in a Microsoft Fabric data warehouse using **SQL-based fine-grained security mechanisms**.

## 🎯 Purpose of the Lab

The aim of this lab was to demonstrate how Microsoft Fabric enables **enterprise-grade data governance** by combining **workspace-level roles** with **granular SQL-level security**. This includes controlling access to rows, columns, and even masked values for sensitive data.

## 🧠 What I Learned

Throughout this lab, I worked through various security layers and gained experience in:

- **Workspace Role Assignments**  
  Learned the importance of separating administrative and viewer roles in a Fabric workspace, and how permissions propagate across items like warehouses.

- **Dynamic Data Masking (DDM)**  
  Implemented automatic masking of sensitive fields like names, emails, and phone numbers—ensuring that unauthorized users see obscured values unless explicitly granted unmasking rights.

- **Row-Level Security (RLS)**  
  Built a policy-based access control mechanism where users only see the rows they're allowed to view, using inline table-valued functions and security predicates.

- **Column-Level Security (CLS)**  
  Restricted access to specific columns (such as credit card numbers) by issuing SQL `DENY` statements—ensuring that even if a user can query the table, they cannot view protected fields.

- **SQL Granular Permissions (GRANT, DENY, REVOKE)**  
  Controlled access at the object level:
  - Granted EXECUTE permission on a stored procedure  
  - Denied SELECT access on a table  
  - Observed the different query outcomes for users with different privileges

- **Permission Testing Across User Roles**  
  Repeatedly tested each scenario by switching between admin and viewer roles to validate how each security setting affected visibility and behavior.

## ✅ Outcome

At the end of this lab, I successfully:
- Designed and applied multiple levels of data protection
- Controlled both schema-level and row-level visibility
- Ensured sensitive data was masked or inaccessible without proper permissions
- Established role-based access aligned with real-world data governance requirements

This hands-on experience directly supports secure, compliant, and scalable data warehousing in production environments using Microsoft Fabric.

## 🤝 Let’s Connect

If you're exploring security in Microsoft Fabric or building enterprise-grade analytics systems, I’d be happy to connect and share insights.  
Reach out via [LinkedIn](https://www.linkedin.com/in/eyilan/) — let’s talk Fabric, data governance, and access control!
