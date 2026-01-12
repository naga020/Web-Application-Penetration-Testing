# Reflected Cross-Site Scripting (XSS)

## Vulnerability Type
Reflected XSS

## Affected Application
DVWA – Reflected XSS Module

## Input Field
Name

## Vulnerable
Yes

## Payload Used
```html
<script>alert(1)</script>

Steps to Reproduce

Open DVWA → Reflected XSS

Enter the payload in the input field

Submit the request

Alert box is displayed

Expected Result

Input should be sanitized and scripts blocked.

Actual Result

Injected JavaScript executes in the browser.

Proof of Exploitation

Screenshot available at:

screenshots/reflected-xss-proof.png

Impact

Allows execution of malicious scripts in victim’s browser.

OWASP Category

OWASP Top 10 – A03: Injection
