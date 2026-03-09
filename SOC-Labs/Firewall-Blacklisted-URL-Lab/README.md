SOC Incident Investigation
Firewall Blacklisted URL Access

Scenario
A SOC alert was triggered when an internal endpoint attempted to access a blacklisted external URL. The firewall blocked the connection and generated a high severity alert.

Objective
Investigate the alert using SIEM logs, identify indicators of compromise, and determine the appropriate incident response.

Tools Used

Splunk SIEM
Firewall Logs
Threat Intelligence
URL Analysis Tool

Indicators of Compromise

Suspicious URL
http://bit.ly/3sHkX3da12340

Destination IP
67.199.248.11

Internal Source IP
10.20.2.17

SIEM Investigation

Query Used

index=main 67.199.248.11

The SIEM search returned a firewall log confirming a blocked outbound connection attempt.

Result

True Positive

The firewall successfully blocked the malicious outbound connection and prevented the internal endpoint from communicating with the external host.

Skills Demonstrated

Security alert triage
SIEM investigation
Firewall log analysis
Indicator of compromise identification
Incident documentation
