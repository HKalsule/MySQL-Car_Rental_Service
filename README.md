# 🚗 Car Rental Management System - SQL Project

This project is a full relational **SQL database** schema for managing a car rental business. It includes entities for customers, cars, bookings, billing, insurance, and more — with data, procedures, views, and triggers to handle the business logic.

---

## 📦 Features

- 👥 **Customer Management** – store and manage personal details and premium membership
- 🚘 **Car Inventory** – manage vehicles with availability, model, make, and mileage
- 🗺️ **Locations** – pickup/drop-off locations with address details
- 📅 **Bookings** – record reservations with car and location details
- 💳 **Billing** – generate bills with discounts, taxes, and late fees
- 💰 **Discounts** – apply promotional offers with expiry dates
- 🛡️ **Insurance Plans** – optional rental car coverage
- ⚙️ **Procedures** – apply discounts, fetch customer booking history
- 👀 **Views** – customer booking and billing summaries
- 🚨 **Triggers** – manage availability and billing totals automatically

---

## 🧱 Schema Overview

| Table               | Description                        |
|--------------------|------------------------------------|
| `Customer`          | Customer details and membership    |
| `Car`               | Car inventory                      |
| `Location`          | Pickup and drop-off points         |
| `CarCategory`       | Categorization of cars             |
| `Booking`           | Booking records                    |
| `Billing`           | Billing and payment information    |
| `Discount`          | Discounts and promo codes          |
| `RentalCarInsurance`| Insurance plans for rentals        |

---

## 🛠️ Procedures & Views

### 📌 Procedures

- `GetCustomerBookings(customer_id)` – returns all bookings by a customer
- `ApplyDiscount(booking_id, discount_code)` – applies a valid discount code to a booking

### 👓 Views

- `View_CustomerBookings` – shows full customer booking info
- `View_BillingSummary` – presents billing data with customer and car details

---

## ⚡ Triggers

- `before_billing_insert` – calculates final billing amount before insert
- `after_booking_insert` – updates car availability after a booking

---

## 🧪 Sample Data Included

Each table is populated with mock entries to help test and demonstrate the schema's capabilities.

---

## 📂 Files

- `schema.sql` – contains all DDL (table creation), DML (data inserts), views, triggers, and procedures

---

