# ParaBank Automation Testing – Selenium + TestNG (Parallel Execution)

## Project Overview
This project automates key functional test scenarios of the **ParaBank Banking Application** using **Selenium WebDriver, Java, TestNG, and Page Object Model (POM)**.  
The framework supports **parallel execution** across multiple browsers (Chrome, Firefox, Edge) using TestNG.

---

## Tech Stack
- **Language:** Java  
- **Automation Tool:** Selenium WebDriver  
- **Test Framework:** TestNG  
- **Design Pattern:** Page Object Model (POM)  
- **Build Tool:** Maven  
- **Browser Support:** Chrome, Firefox, Edge  
- **Parallel Execution:** TestNG XML  
- **IDE:** Eclipse 

---

## Project Structure

ParaBankAutomation/
│
├── src/test/java
│   ├── bankPOM
│   │   ├── BaseTest.java
│   │   ├── HomepagePOM.java
│   │   ├── RegistrationPagePOM.java
│   │   └── DashboardPOM.java
│   │
│   └── paraBankTesting
│       ├── PO.java
│       ├── AllpageTest.java
│       └── UserManagementTest.java
│
├── testng.xml
├── pom.xml
└── README.md

## Automated Test Scenarios

### 1️⃣ Registration
**Test Scenario:** Verify new user registration  
**Steps:**
1. Navigate to Register page  
2. Enter valid personal and login details  
3. Submit registration form  
4. Verify success message  

**Expected Result:**  
✔ Registration successful and user logged in

### 2️⃣ Login / Logout
**Test Scenario:** Verify login functionality  
**Steps:**
1. Navigate to login page  
2. Enter valid username and password  
3. Click Login  
4. Verify dashboard page  

**Expected Result:**  
✔ Dashboard loads with correct customer name

### 3️⃣ Fund Transfer
**Test Scenario:** Verify fund transfer between accounts  
**Steps:**
1. Log in with valid credentials  
2. Navigate to Transfer Funds  
3. Select source and destination accounts  
4. Enter transfer amount  
5. Click Transfer  

**Expected Result:**  
✔ Fund transfer completed successfully with confirmation message

### 4️⃣ Loan Application
**Test Scenario:** Verify loan request  
**Steps:**
1. Log in to ParaBank  
2. Navigate to Request Loan section  
3. Enter valid loan amount and down payment  
4. Submit application  

**Expected Result:**  
✔ Loan request submitted and confirmation displayed


## ⚡ Parallel Execution
Parallel testing is implemented using **TestNG XML** to run tests simultaneously on:
- Chrome  
- Firefox  
- Edge  

## How to Run the Tests

### Option 1: Using TestNG XML
1. Import the project into Eclipse / IntelliJ  
2. Right-click on `testng.xml`  
3. Select **Run As → TestNG Suite**
