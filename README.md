# Vulnerability Assessment Report

## Website Tested

demo.testfire.net

## Assessment Type

Passive Vulnerability Assessment

## Scope

Public-facing website analysis only. No exploitation, brute-force attacks, denial-of-service attacks, or unauthorized access attempts were performed.

## Tools Used

* Nmap
* SecurityHeaders.com
* Browser Developer Tools
* OWASP ZAP (Passive Scan)

## Findings

### High Risk

1. SQL Injection
2. Cross Site Scripting (Reflected)

### Medium Risk

3. Missing Content Security Policy (CSP)
4. Absence of Anti-CSRF Tokens

### Low Risk

5. Missing X-Frame-Options
6. Missing X-Content-Type-Options
7. Missing Permissions-Policy
8. Cookie Without SameSite Attribute
9. Server Information Disclosure
10. Open Network Services

## Evidence

Screenshots and scan outputs are included in this repository.

## Recommendations

* Implement Content Security Policy (CSP).
* Use parameterized queries to prevent SQL Injection.
* Sanitize and validate user input to mitigate XSS.
* Implement Anti-CSRF protections.
* Configure missing security headers.
* Hide server version information.
* Review and secure exposed network services.
* Enforce HTTPS and secure cookie settings.

## Conclusion

The assessment identified several security weaknesses across the target application. Implementing the recommended mitigations will significantly improve the overall security posture and reduce potential attack vectors.
