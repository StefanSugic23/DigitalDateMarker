# Digital Date Marker for Coffee Shops and Restaurants

## Overview

**Digital Date Marker** is an APL-based tool designed for coffee shops and restaurants to calculate and display the expiration date or recommended use-by time of prepared food and beverages.

The idea is simple: instead of manually writing production and expiration information on labels, the user selects the product, enters the required information when necessary, and the program automatically calculates the expiration date and time.

> **A small idea with a practical purpose — a digital alternative to the traditional analogue date marker.**

This project can be seen as a concept for **one of the first digital date-marker systems built specifically with APL for coffee-shop and restaurant use.**

---

## Features

To start the Digital Date Marker, run the `PowerOn` function in Dyalog APL:

```text
      PowerOn
================================
  Digital Date Marker for Coffee Shops and Restaurants
================================
1. One Day
2. Two Days
3. Three Days
4. Foccacia
5. Thirty Days
6. Thirty Days-Custom Date
7. Custom Date
8. Bryggkaffe
9. Frapino
0. Power off
⎕:
```

The program provides several predefined expiration periods as well as custom date and time calculations.

### 1. One Day

Select **One Day** to calculate an expiration date **one day after production**.

### 2. Two Days

Select **Two Days** to calculate an expiration date **two days after production**.

### 3. Three Days

Select **Three Days** to calculate an expiration date **three days after production**.

### 4. Foccacia

Select **Foccacia** to automatically calculate an expiration date **three days after production**.

### 5. Thirty Days

Select **Thirty Days** to calculate an expiration date **thirty days after production**.

### 6. Thirty Days – Custom Date

Select this option to enter a **custom production date** and automatically calculate the expiration date **thirty days later**.

### 7. Custom Date

Select **Custom Date** when a different expiration period is required.

The user enters:

1. The number of days for the expiration period.
2. The production year.
3. The production month.
4. The production day.

The program then calculates and displays the correct expiration date.

### 8. Bryggkaffe

Select **Bryggkaffe** for brewed coffee.

The program calculates an expiration time **1 hour and 45 minutes after production** and displays both the production time and expiration time.

### 9. Frapino

Select **Frapino** to automatically calculate an expiration date **three days after production**.

### 0. Power off

Select **Power off** to exit the Digital Date Marker.

---

## Why Digital Instead of Analogue?

Traditional date markers require employees to manually calculate or write production and expiration information. This can introduce unnecessary mistakes, especially during busy periods.

A digital date marker can:

* **Reduce human calculation errors**
* **Automatically calculate expiration dates**
* **Automatically calculate expiration times**
* **Handle different expiration periods**
* **Allow custom dates and durations**
* **Make labels easier and faster to prepare**
* **Provide consistent results**
* **Reduce repetitive manual work**
* **Be used repeatedly without manual date calculations**

For example, instead of an employee manually calculating:

```text
Produced: 21/08/2026
+ 3 days
= 24/08/2026
```

the system performs the calculation automatically.

For time-based products such as brewed coffee:

```text
Produced: 12:00
Duration: 1 hour 45 minutes
Expires: 13:45
```

---

## The Concept

The main idea behind the project is to turn a simple everyday task into a small automated system.

A traditional marker answers:

> **"What date should I write?"**

The Digital Date Marker answers:

> **"What is the correct expiration date and time?"**

This makes the project more than just a date calculator. It demonstrates how APL can be used to create a practical business-oriented application from a real-world problem.

---

## Built for Long-Term Date Accuracy

The Digital Date Marker is designed to work **indefinitely**, rather than being limited to a specific year.

The date calculations account for:

* Different numbers of days in each month
* February having 28 or 29 days
* Leap years
* Year changes
* Month changes
* Correct date rollover when adding days
* Time calculations that cross into the next hour or day

Leap years and the different calendar rules have been taken into consideration so that the system can continue calculating dates correctly far into the future.

The system is therefore **not based on fixed assumptions such as "every month has 30 days."** Instead, it takes the actual calendar structure into account when calculating expiration dates.

### Example

If a product is produced near the end of February during a leap year, the system correctly handles February 29 and continues into March.

```text
Production date: 2028-02-28
Duration: 3 days

Expiration date: 2028-03-02
```

The same logic applies across month and year boundaries.

**The Digital Date Marker is designed to remain reliable regardless of the date on which it is used.**

---

## Example

A user selects **Custom Date**:

```text
Enter number of days: 5

Enter production date:
Year: 2026
Month: 8
Day: 21

Expiration date:
2026-08-26
```

For brewed coffee:

```text
Produced: 12:00
Expiration: 13:45
Duration: 1 hour 45 minutes
```

The user does not need to manually perform the calculations.

---

## APL

The project is written entirely in **Dyalog APL**.

The project demonstrates the use of:

* Functions
* Variables
* Conditional logic
* User input
* Date and time handling
* Date arithmetic
* Time arithmetic
* Custom calculations
* Menu-driven program structure
* Automatic expiration calculations
* Calendar and leap-year handling

---

## Purpose

The purpose of this project is to demonstrate how programming can be used to automate a small but repetitive task in the food and beverage industry.

It also demonstrates how **APL can be applied to practical business problems**, particularly where calculations, dates, times and data processing are involved.

The project focuses on taking a real-world process that is normally handled manually and turning it into a **simple, reliable and reusable digital solution**.

---

## Author

**Stefan Sugic**

Built with **Dyalog APL**.

> **Digital Date Marker — replacing manual date calculations with a simple digital solution.**
