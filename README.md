# cvss4
Analysis of the CVSS 4.0 scoring system

The enclosed PDF document (https://github.com/labyrinthinesecurity/cvss4/blob/main/CVSSanomaly.pdf) explains how chatGPT, with the help of automated reasoning, found two anomalies in the new CVSS 4.0 scoring system: 
- a major anomaly comes from vector string CVSS:4.0/AV:N/AC:L/AT:N/PR:N/UI:N/VC:L/VI:L/VA:L/SC:H/SI:H/SA:H, which is rated 7.9 (HIGH) while it should be rated CRITICAL (>= 9.0)
- a minor anomaly comes from vector strings CVSS:4.0/AV:N/AC:L/AT:N/PR:N/UI:N/VC:L/VI:H/VA:H/SC:H/SI:H/SA:H and CVSS:4.0/AV:N/AC:H/AT:N/PR:N/UI:N/VC:L/VI:H/VA:H/SC:H/SI:H/SA:H which are scored 9.3 and 9.2 respectively. The gap is too small (0.1) to reflect the impact of changing attack complexity (AC) from Low to High

The full transcript of the chtGPT conversation may be read here: https://chat.openai.com/share/41774eb6-320c-4a14-867f-32430ce326cf

Here is a screenshot of the major anomaly, take from the online CVSS calculator in Public Preview as of Septemer 26, 2023:
https://www.first.org/cvss/calculator/4.0#CVSS:4.0/AV:N/AC:L/AT:N/PR:N/UI:N/VC:L/VI:L/VA:L/SC:H/SI:H/SA:H

![alt text](https://github.com/labyrinthinesecurity/cvss4/blob/main/CVSS_critical.png)
