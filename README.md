# 🚀 Invest With Guru

## 📌 Project Overview
**Invest With Guru** is a fully functional, end-to-end **ServiceNow enterprise application** designed to showcase advanced platform capabilities beyond traditional ITSM use cases.  
The project focuses on building a **secure, scalable, and integration-driven investment platform** with real-world business workflows.

This application demonstrates hands-on expertise in:
- Secure third-party integrations
- PayPal payment processing
- OTP-based user verification
- Role-based ACL security
- Server-side architecture best practices
- Date & time handling across workflows

The solution delivers a complete user journey — from onboarding and request submission to secure payment confirmation and reporting — following **ServiceNow production standards**.

---

## 🎯 Business Use Case
Invest With Guru simulates a real-world **investment & subscription platform** where users can:
- Submit investment requests
- Verify identity using OTP
- Complete secure payments via PayPal
- Track investment status
- View historical transactions

Administrators can:
- Control access using ACLs
- Monitor payments and investments
- Manage integrations
- View dashboards and reports

---

## 🏗️ Application Architecture
The application is built using a **layered architecture**:

- **Client Layer**
  - Service Portal widgets
  - UI Policies & Client Scripts
- **Server Layer**
  - Script Includes
  - Business Rules
  - ACL Scripts
- **Integration Layer**
  - REST Messages
  - External APIs (PayPal)
- **Security Layer**
  - Role-based access control
  - OTP validation
- **Data Layer**
  - Custom tables for investments, payments, OTP logs

All sensitive logic is handled strictly on the **server side**.

---

## 🔐 Security & ACL Implementation
Security is a core pillar of Invest With Guru.

### 🔹 Role-Based Access
Custom roles are used to restrict access:
- `x_iwg.user`
- `x_iwg.admin`

### 🔹 Table-Level ACL (Read)
```js
answer = gs.hasRole('x_iwg.user') || gs.hasRole('admin');
