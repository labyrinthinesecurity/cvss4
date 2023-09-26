# cvss4
Analysis of the CVSS 4.0 scoring system

The PDF document explains how chatGPT, with the help of automated reasoning, found two anomalies in thr CVSS 4.0 scoring system: 
- a major anomaly comes from vector string CVSS:4.0/AV:N/AC:L/AT:N/PR:N/UI:N/VC:L/VI:L/VA:L/SC:H/SI:H/SA:H, which is rated 7.9 (HIGH) while it should be rated CRITICAL (>= 9.0)
