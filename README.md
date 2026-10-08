# MAHWI-2.0
Mahwi 2.0 is a modern React and Laravel ERP and accounting platform for businesses, connecting factory production, wholesale, distribution, retail, inventory, sales, purchasing, assets, liabilities, equity, and financial reporting through a unified multi-business, double-entry accounting system.
# Mahwi 2.0

**Mahwi 2.0** is a modern, full-featured **ERP and accounting platform** designed to manage businesses from **factory production through wholesale, distribution, retail, and final sales**, while maintaining a complete double-entry accounting system.

> **Factory → Wholesale → Distribution → Retail → Customer**

Mahwi 2.0 is being built with a modern **React frontend** and **Laravel API backend**, with accounting at the core of every business transaction.

---

## 🚀 Vision

Mahwi 2.0 aims to provide businesses with one integrated platform for managing:

* Business operations
* Manufacturing
* Wholesale
* Distribution
* Retail
* Inventory
* Purchasing
* Sales
* Customers and suppliers
* Employees and users
* Assets
* Liabilities
* Equity
* Banking
* Expenses
* Taxes
* Financial accounting
* Business reporting

The goal is to eliminate disconnected systems by connecting operational activities directly to accounting and financial reporting.

---

## 🏗️ Architecture

```text
                           MAHWI 2.0
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
        PLATFORM CORE     OPERATIONS         ACCOUNTING
             │                 │                 │
        Businesses          Factory          Chart of Accounts
        Business Types      Production       Journal
        Users               Wholesale        General Ledger
        Roles               Distribution     Accounts Receivable
        Permissions         Retail           Accounts Payable
        Locations           Inventory        Assets
        Partners            Purchasing       Liabilities
                            Sales            Equity
                               │                 │
                               └────────┬────────┘
                                        │
                                   REPORTING
                                        │
                     ┌──────────────────┼─────────────────┐
                     │                  │                 │
                Balance Sheet       Profit & Loss      Cash Flow
                Trial Balance       General Ledger     Management
```

---

## 🔄 Business Supply Chain

Mahwi 2.0 is designed around a connected business supply chain:

```text
Factory
   │
   ▼
Production
   │
   ▼
Finished Goods
   │
   ▼
Wholesaler
   │
   ▼
Distributor
   │
   ▼
Retailer
   │
   ▼
Customer
```

Each stage can maintain its own inventory, transactions, users, locations, and accounting records.

---

# 💰 Accounting First

Accounting is a fundamental part of Mahwi 2.0, not an afterthought.

The system is based on the fundamental accounting equation:

```text
Assets = Liabilities + Equity
```

Every financial transaction should be represented through **double-entry accounting**.

### Example: Cash Sale

```text
Debit   Cash                 100,000
Credit  Sales Revenue                    100,000
```

If the inventory cost is RWF 60,000:

```text
Debit   Cost of Goods Sold    60,000
Credit  Inventory                          60,000
```

This allows Mahwi to automatically maintain:

* Assets
* Liabilities
* Equity
* Revenue
* Expenses
* Profit and Loss
* Inventory valuation
* Accounts receivable
* Accounts payable
* General ledger

---

# 🏭 Manufacturing

The manufacturing module will support the complete production lifecycle.

```text
Raw Materials
      │
      ▼
Bill of Materials
      │
      ▼
Production Order
      │
      ▼
Material Consumption
      │
      ▼
Work in Progress
      │
      ▼
Finished Goods
```

Planned manufacturing features include:

* Raw materials
* Bill of Materials (BOM)
* Production orders
* Production planning
* Material consumption
* Work in progress
* Finished goods
* Production wastage
* Quality control
* Production costing
* Production reports
* Work centers
* Production locations

---

# 📦 Inventory Management

Mahwi 2.0 will provide centralized inventory management across businesses and locations.

Features include:

* Products
* Categories
* Units of measurement
* Warehouses
* Stock levels
* Stock movements
* Transfers
* Adjustments
* Returns
* Damaged stock
* Opening stock
* Inventory valuation
* Low-stock alerts
* Batch and expiry management where applicable

All stock movements should be traceable and connected to the appropriate business transaction and accounting records.

---

# 🏢 Wholesale Management

Wholesale businesses will be able to manage:

* Wholesale customers
* Retailer relationships
* Wholesale pricing
* Sales orders
* Invoices
* Deliveries
* Credit sales
* Payments
* Accounts receivable
* Customer balances
* Wholesale inventory

---

# 🚚 Distribution

Mahwi 2.0 is designed to support distribution operations between businesses and locations.

Planned features include:

* Distribution orders
* Delivery management
* Routes
* Vehicles
* Drivers
* Delivery status
* Warehouse dispatch
* Delivery confirmation
* Stock transfers

---

# 🛒 Retail & POS

Retail businesses will have access to a modern POS system supporting:

* Product search
* Barcode scanning
* Sales
* Payments
* Discounts
* Returns
* Customers
* Cash management
* Receipts
* Retail inventory
* Multiple payment methods

POS transactions will automatically contribute to inventory and accounting records.

---

# 🏦 Financial Management

Mahwi 2.0 will provide a complete financial management layer.

### Accounts

* Chart of Accounts
* General Ledger
* Accounts Receivable
* Accounts Payable
* Cash
* Bank accounts
* Equity
* Liabilities
* Revenue
* Expenses

### Assets

The system will support fixed assets such as:

* Buildings
* Vehicles
* Machinery
* Computers
* Furniture
* Equipment

Planned asset features include:

* Asset registration
* Asset categories
* Purchase cost
* Useful life
* Residual value
* Depreciation
* Accumulated depreciation
* Asset disposal
* Asset location

---

# 📊 Financial Reports

Mahwi 2.0 is designed to provide professional accounting and management reports.

### Core Accounting Reports

* Balance Sheet
* Income Statement
* Profit & Loss
* Trial Balance
* General Ledger
* Cash Flow Statement
* Accounts Receivable
* Accounts Payable
* Account Statements

### Business Reports

* Sales reports
* Purchase reports
* Inventory reports
* Production reports
* Wholesale reports
* Retail reports
* Expense reports
* Tax reports
* Asset reports
* Profitability reports

---

# 🏢 Multi-Business Architecture

Mahwi 2.0 is designed as a multi-business platform.

A user can potentially work with multiple businesses according to their assigned roles and permissions.

```text
User
 │
 ├── Business A
 │     └── Factory Manager
 │
 ├── Business B
 │     └── Accountant
 │
 └── Business C
       └── Business Owner
```

Businesses can also have multiple locations:

```text
Business
 │
 ├── Factory
 ├── Warehouse
 ├── Branch
 ├── Wholesale Location
 └── Retail Shop
```

---

# 👥 Users, Roles & Permissions

Mahwi 2.0 will use role-based access control.

Example roles include:

* Super Administrator
* Business Owner
* Business Administrator
* Factory Manager
* Production Supervisor
* Wholesale Manager
* Distribution Manager
* Retail Manager
* Storekeeper
* Salesperson
* Cashier
* Accountant
* Finance Manager

Permissions will control access to individual operations and modules.

Example:

```text
production.view
production.create
production.approve
production.complete

inventory.view
inventory.adjust
inventory.transfer

sales.view
sales.create
sales.refund

accounting.view
accounting.post
accounting.close_period

reports.view
reports.export
```

---

# 🧱 Core Architecture

The system is designed around reusable business services rather than allowing each module to implement its own financial logic.

Example:

```text
POS Sale
   │
   ▼
Business Transaction
   │
   ├── Inventory Movement
   │
   └── Accounting Posting
           │
           ▼
        Journal
           │
           ▼
     General Ledger
           │
           ▼
     Financial Reports
```

The same principle applies to:

* Purchases
* Production
* Wholesale sales
* Retail sales
* Expenses
* Payments
* Assets
* Loans
* Transfers

---

# 🛠️ Technology Stack

## Frontend

* React
* Vite
* React Router
* Tailwind CSS
* TanStack Query
* Zustand

## Backend

* Laravel
* Laravel API
* Laravel Sanctum
* MySQL
* Laravel Queues
* Laravel Notifications

---

# 📁 Project Structure

```text
mahwi-2/
│
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   ├── components/
│   │   ├── layouts/
│   │   ├── modules/
│   │   ├── services/
│   │   └── store/
│   └── package.json
│
├── backend/
│   ├── app/
│   │   ├── Models/
│   │   ├── Services/
│   │   ├── Http/
│   │   └── Policies/
│   ├── database/
│   ├── routes/
│   └── composer.json
│
└── README.md
```

---

# 🗃️ Core Domain Models

The initial architecture will include entities such as:

```text
User
Business
BusinessType
BusinessUser
Role
Permission
RolePermission
BusinessLocation
BusinessPartner
BusinessRelationship

Account
AccountType
Journal
JournalLine
FiscalYear
AccountingPeriod

Product
Category
Unit
Warehouse
StockMovement

BillOfMaterial
BillOfMaterialItem
ProductionOrder
ProductionConsumption
ProductionOutput
ProductionWastage

Customer
Supplier
SalesOrder
PurchaseOrder
Invoice
Payment

FixedAsset
AssetDepreciation
BankAccount
Tax
Expense
```

The exact model structure will evolve as development progresses.

---

# 🔐 Security

Security is a core requirement.

Planned security features include:

* API authentication
* Role-based authorization
* Permission-based access
* Business-level data isolation
* Location-level access where required
* Audit logs
* Secure password handling
* Session management
* Financial transaction audit trails

Financial records should be traceable and protected from unauthorized modification.

---

# 🧪 Development Status

> **Status: Active Development**

Mahwi 2.0 is currently being designed and developed.

The initial focus is on building a strong foundation before implementing the complete manufacturing, wholesale, retail, and accounting workflows.

### Current development priority

```text
[ ] Project foundation
[ ] Authentication
[ ] Businesses
[ ] Business Types
[ ] Users
[ ] Roles
[ ] Permissions
[ ] Business Locations
[ ] Business Partners

[ ] Accounting foundation
[ ] Chart of Accounts
[ ] Journal
[ ] Journal Lines
[ ] General Ledger
[ ] Trial Balance

[ ] Products
[ ] Inventory

[ ] Manufacturing
[ ] Wholesale
[ ] Distribution
[ ] Retail
[ ] POS

[ ] Financial Reports
```

---

# 🎯 Long-Term Goal

Mahwi 2.0 aims to become a unified business platform where a business can manage its complete lifecycle from **procurement and production to distribution, sales, and financial reporting**.

```text
PROCUREMENT
     ↓
RAW MATERIALS
     ↓
FACTORY
     ↓
PRODUCTION
     ↓
FINISHED GOODS
     ↓
WHOLESALE
     ↓
DISTRIBUTION
     ↓
RETAIL
     ↓
CUSTOMER
     ↓
ACCOUNTING
     ↓
FINANCIAL REPORTING
```

At every stage, Mahwi 2.0 should know:

* What the business owns
* What the business owes
* What customers owe the business
* What the business owes suppliers
* What inventory is available
* What was purchased
* What was produced
* What was sold
* What was spent
* What was earned
* What the business is worth
* Whether the books balance

---

# 📜 License

License information will be added as the project progresses.

---

## Mahwi 2.0

**ERP • Accounting • Manufacturing • Wholesale • Distribution • Retail**

**One platform. One business view. Complete financial control.**
