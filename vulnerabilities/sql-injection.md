# SQL Injection

## Vulnerability Type
SQL Injection

## Affected Application
DVWA – SQL Injection Module

## Input Field
User ID

## Vulnerable
Yes

## Payload Used
```sql
1 OR 1=1

Steps to Reproduce

<<<<<<< HEAD
Open DVWA and navigate to the SQL Injection module
=======
Navigate to DVWA → SQL Injection module
>>>>>>> 2af4d12 (Updated SQL Injection documentation format)

Enter the payload in the User ID field

Submit the request

<<<<<<< HEAD
Observe unauthorized access to database records

Expected Result

The application should not allow SQL query manipulation.

Actual Result

The application returns sensitive user data.

Proof of Exploitation

Screenshot available at:

screenshots/sql-injection-proof.png

=======
Observe unauthorized data disclosure

Expected Result

The application should validate input and prevent query manipulation.

Actual Result

The application returns sensitive user information such as usernames.

Proof of Exploitation

Refer to the screenshot:

screenshots/sql-injection-proof.png
>>>>>>> 2af4d12 (Updated SQL Injection documentation format)
Impact

An attacker can bypass authentication and access confidential data.

OWASP Category

OWASP Top 10 – A03: Injection
<<<<<<< HEAD
=======


>>>>>>> 2af4d12 (Updated SQL Injection documentation format)
