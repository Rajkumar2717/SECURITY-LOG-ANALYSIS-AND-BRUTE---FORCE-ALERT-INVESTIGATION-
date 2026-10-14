# SECURITY-LOG-ANALYSIS-AND-BRUTE---FORCE-ALERT-INVESTIGATION-



End-to-end workflow
01

Collect sample logs
Use sample Windows authentication events or a prepared lab dataset. Each event should contain a timestamp, username, source IP and login result.


02

Load logs into Splunk
Import the sample log file into Splunk and verify that the events and their fields are searchable.


03

Detect suspicious activity
Search for repeated failed logins. Group events by source IP and time to identify unusual patterns.


04

Investigate the alert
Check the number of failures, targeted usernames, time interval and whether a successful login followed the failures.


05

Assess and escalate
Determine whether the pattern warrants further investigation. Do not assume an attack is confirmed from failed logins alone.


06

Recommend a response
Document the evidence and recommend actions such as validating the activity with the account owner, blocking the source when justified, and resetting compromised credentials if needed.


07

Prepare an incident report
Summarize the alert, evidence, impact, investigation result and recommendations.


---------------------------------------------------------------------------------------

Collected and analyzed sample authentication logs to identify repeated failed login attempts and suspicious login patterns.
Used Splunk Search Processing Language (SPL) to filter authentication events and summarize failed login attempts by source IP address and username.
Examined timestamps, login outcomes, and event frequency to identify potentially suspicious authentication activity.
Investigated repeated login failures followed by successful authentication to assess potential unauthorized access.
Documented security alerts, investigation evidence, and findings in a structured incident report.
Recommended preventive measures, including account monitoring, multi-factor authentication (MFA), and account lockout policies.
