Failed Login Detection — Beginner SOC Project

1. Objective

The objective of this project is to understand how a SOC Analyst identifies repeated failed login attempts that may indicate a brute-force attack.

2. What Is a Failed Login?

A failed login occurs when a user cannot authenticate successfully. Multiple failures in a short period may indicate incorrect passwords or a possible attack.

3. Sample Log Data

Time| Username| Source IP| Result
10:01| admin| 192.0.2.10| Failed
10:02| admin| 192.0.2.10| Failed
10:03| admin| 192.0.2.10| Failed
10:05| analyst| 192.0.2.20| Success

These are fictional examples using documentation-only IP addresses.

4. Detection

Three failed login attempts for the same username from the same IP within a short period could trigger an alert for investigation.

5. Investigation

A SOC Analyst should:

- Check the number and timing of failed attempts.
- Review the source IP and targeted account.
- Check whether a successful login followed the failures.
- Correlate events with other security logs.

6. Mitigation

- Apply rate limiting and appropriate account lockout policies.
- Enable multi-factor authentication (MFA).
- Monitor authentication logs and alert on suspicious patterns.
- Block a source IP only when justified by investigation and security policy.

7. Learning Outcome

This project demonstrates beginner-level understanding of authentication logs, brute-force indicators, alert investigation, and defensive security controls.

Disclaimer

This is a learning project using fictional sample data. No real systems were accessed or tested.
