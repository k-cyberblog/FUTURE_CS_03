Task 3 - # API Security Risk Analysis

##  Overview

This project presents a basic security analysis of a public API.
The goal is to identify common security risks such as open access, data exposure, and lack of proper controls.

---

##  API Tested

**JSONPlaceholder API**
https://jsonplaceholder.typicode.com

### Endpoints Tested:

* `/posts`
* `/posts/1`
* `/users`

---

##  Tools Used

* **Postman** – for sending API requests and analyzing responses
* **Browser DevTools** – for inspecting network requests and headers
* **Insomnia** – considered as an alternative API testing tool

---

##  Methodology

* Selected a public/demo API for testing
* Sent API requests using Postman
* Observed response data and behavior
* Checked authentication and access control
* Identified potential security risks
* Suggested remediation steps

---

##  Key Findings

### 1. Open / Unauthenticated Endpoints

* API allows access without login
* **Risk:** Unauthorized data access

### 2. Excessive Data Exposure

* API returns full data including IDs and user details
* **Risk:** Information leakage

### 3. Missing Authentication Mechanism

* No tokens or login system implemented
* **Risk:** Anyone can access API

### 4. Authorization Issues

* No restriction on accessing different records
* **Risk:** Users can access all data

### 5. Missing Rate Limiting

* Unlimited requests allowed
* **Risk:** API abuse or server overload

### 6. Input Validation Issues

* Weak validation for incorrect inputs
* **Risk:** Unexpected behavior

---

##  Recommendations

* Implement authentication (API keys or tokens)
* Restrict access using proper authorization
* Limit data exposure in responses
* Add rate limiting to prevent abuse
* Validate all user inputs properly

---

##  Screenshots

Screenshots of API testing using Postman and DevTools are available in the `/screenshots` folder.
