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

Open DVWA and navigate to the SQL Injection module

Enter the payload in the User ID field

Submit the request

Observe unauthorized access to database records

Expected Result

The application should not allow SQL query manipulation.

Actual Result

The application returns sensitive user data.

Proof of Exploitation

Screenshot available at:

screenshots/sql-injection-proof.png

Impact

An attacker can bypass authentication and access confidential data.

OWASP Category

OWASP Top 10 – A03: Injection
