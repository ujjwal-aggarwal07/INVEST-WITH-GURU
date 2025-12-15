# 🚀 Invest With Guru

## 📌 Project Overview

**Invest With Guru** is a fully functional, end-to-end **ServiceNow enterprise application** designed to showcase advanced platform capabilities beyond traditional ITSM use cases.

The project focuses on building a **secure, scalable, and integration-driven investment platform** that aligns with real-world business workflows.

This application demonstrates hands-on expertise in:
- Secure third-party integrations
- PayPal payment processing
- OTP-based user verification
- Role-based ACL security
- Server-side architecture best practices
- Date and time handling across workflows

The solution delivers a complete user journey — from onboarding and request submission to secure payment confirmation and reporting — following **ServiceNow production standards**.

---

## 🎯 Business Use Case

**Invest With Guru** simulates a real-world **investment and subscription management platform**.

### User Capabilities
- Submit investment requests via Service Portal  
- Verify identity using OTP-based authentication  
- Complete secure payments using PayPal  
- Track investment status in real time  
- View historical investment and transaction records  

### Administrator Capabilities
- Control access using role-based ACLs  
- Monitor payments and investment activity  
- Manage integrations and configurations  
- View operational dashboards and reports  

---

## 🏗️ Application Architecture

The application follows a **layered enterprise architecture** to ensure scalability, maintainability, and security.

### Client Layer
- Service Portal widgets  
- UI Policies for dynamic behavior  
- Client Scripts limited to UI logic  

### Server Layer
- Script Includes for business logic  
- Business Rules for automation  
- ACL scripts for access enforcement  

### Integration Layer
- REST Messages for API communication  
- External integrations with PayPal  

### Security Layer
- Role-based access control  
- OTP validation for critical actions  

### Data Layer
- Custom tables for investments  
- Payment transaction records  
- OTP and audit logs  

All sensitive business logic is handled strictly on the **server side**.

---

## 🔐 Security & Access Control

Security is a foundational aspect of **Invest With Guru**.

### Role-Based Security
- Separate roles for users and administrators  
- Table-level, field-level, and scripted ACLs  
- Record-level access restrictions  

### Security Best Practices
- No sensitive logic exposed on the client side  
- Server-side validation for all critical actions  
- Controlled access to financial and personal data  

---

## 🔑 OTP-Based Verification

OTP-based verification is implemented to secure high-risk operations such as:
- Payment confirmation  
- Sensitive workflow transitions  

The OTP mechanism includes:
- Secure server-side generation  
- Time-bound expiration  
- Validation before allowing protected actions  

---

## 💳 PayPal Integration

The application integrates **PayPal** to enable secure and reliable payment processing.

Key integration features:
- Server-side REST-based communication  
- Secure credential handling  
- Real-time payment status validation  
- Support for success, failure, and retry scenarios  

---

## ⏰ Date & Time Handling

Date and time management is handled carefully across the application, including:
- OTP expiry tracking  
- Subscription start and end dates  
- Payment timestamps  
- Workflow and SLA timing  

The platform ensures time-zone-safe processing for all users.

---

## 📊 Reporting & Dashboards

The application includes reporting and analytics capabilities such as:
- Investment status distribution  
- Payment success vs failure trends  
- User-wise investment summaries  
- Time-based analytical views  

Dashboards provide real-time visibility into platform activity.

---

## 🏁 Conclusion

**Invest With Guru** is a production-ready ServiceNow application that demonstrates strong expertise in secure platform design, payment integrations, OTP-based authentication, and enterprise-grade access control.

The project serves as a comprehensive portfolio showcase for ServiceNow development and real-world business application design.

## ⚙️ Application Functionalities

The **Invest With Guru** application is designed around core investment workflows that closely reflect real-world trading and portfolio management systems. Each functionality is implemented with strong security controls, validation, and a user-friendly experience.

---

### 💰 Buy Module

The **Buy** functionality allows users to place investment or purchase requests in a controlled and secure manner.

Key characteristics:
- Users can select investment instruments or plans through the Service Portal
- Input validation ensures correctness of investment amount and selection
- OTP verification is triggered before final submission for security
- Payment is initiated only after successful OTP validation
- PayPal integration handles the financial transaction securely
- Buy requests follow a defined lifecycle (Requested → In Progress → Completed)

Business value:
- Ensures controlled investment entry
- Prevents unauthorized or accidental transactions
- Maintains accurate financial records

---

### 📉 Sell Module

The **Sell** functionality enables users to exit or redeem existing investments.

Key characteristics:
- Users can view only their eligible investments for selling
- System validates holding period and business rules before allowing sell
- OTP verification is required for sell confirmation
- Sell requests are processed securely on the server side
- Status tracking is available throughout the sell lifecycle

Business value:
- Protects against invalid or premature sell requests
- Ensures compliance with business and financial rules
- Maintains transactional integrity

---

### 💼 Funds Module

The **Funds** module provides users with complete visibility and control over their financial balances.

Key characteristics:
- Displays available, invested, and blocked funds
- Real-time updates after buy or sell operations
- Server-side calculations prevent data manipulation
- Restricted access using role-based ACLs
- Historical fund movement tracking

Business value:
- Provides transparency to users
- Prevents overspending or invalid transactions
- Maintains accurate account balances

---

### 📊 Reports Module

The **Reports** module offers detailed analytical insights for both users and administrators.

Key characteristics:
- User-specific investment and transaction reports
- Admin-level dashboards for system-wide monitoring
- Filters based on date range, status, and investment type
- Time-based analytics using accurate date and time handling
- Drill-down capabilities for deeper analysis

Business value:
- Supports data-driven decision-making
- Enhances operational visibility
- Enables audit and compliance tracking

---

### 🔐 Security Across All Modules

Each functionality is protected by:
- Role-based ACLs
- Server-side validations
- OTP-based verification for sensitive actions
- Secure integration handling
- Time-zone-aware date processing

---

### 🔄 End-to-End Flow Summary

1. User logs in and accesses the Service Portal  
2. User performs Buy or Sell action  
3. OTP verification is triggered  
4. Payment or fund adjustment is processed  
5. Records are updated securely  
6. Reports and dashboards reflect real-time data  

---

### 🏁 Functional Coverage Summary

| Module | Purpose |
|------|--------|
| Buy | Secure investment placement |
| Sell | Controlled investment exit |
| Funds | Balance and fund management |
| Reports | Analytics and visibility |

---

These functionalities together make **Invest With Guru** a complete, secure, and enterprise-ready ServiceNow investment application.
