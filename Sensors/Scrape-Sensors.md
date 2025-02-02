# Scrape Sensors

## Home Assistant Past Security Vulnerability

Resource: https://www.home-assistant.io/security/
Method: Get

Name: HA Latest Vulnerability CVE
Select: p em a[href*='nvd.nist.gov']
Attribute: href


Name: HA Latest Vulnerability CVE ID
Select: p em a[href*='nvd.nist.gov']
Value Template: {{ value.split('/')[-1] }}
