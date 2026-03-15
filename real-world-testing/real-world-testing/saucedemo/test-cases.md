# Test Cases – SauceDemo Login

Application: https://www.saucedemo.com  
Module: Authentication  
Test Type: Functional Testing  

---

## TC01 – Login with valid credentials

**Precondition**
User is on the login page.

**Test Data**

| Username | Password |
|--------|--------|
| standard_user | secret_sauce |

**Steps**

1. Open the SauceDemo login page
2. Enter username `standard_user`
3. Enter password `secret_sauce`
4. Click **Login**

**Expected Result**

User should be redirected to the inventory page.

---

## TC02 – Login with invalid password

**Precondition**
User is on the login page.

**Test Data**

| Username | Password |
|--------|--------|
| standard_user | wrong_password |

**Steps**

1. Enter username `standard_user`
2. Enter password `wrong_password`
3. Click **Login**

**Expected Result**

System displays error message:


---

## TC03 – Login with empty username

**Steps**

1. Leave username empty
2. Enter password `secret_sauce`
3. Click **Login**

**Expected Result**

Error message should appear indicating username is required.

---

## TC04 – Login with empty password

**Steps**

1. Enter username `standard_user`
2. Leave password empty
3. Click **Login**

**Expected Result**

Error message should appear indicating password is required.

---

## TC05 – Login with both fields empty

**Steps**

1. Leave username empty
2. Leave password empty
3. Click **Login**

**Expected Result**

System prevents login and displays validation message.
