# Detection_SOC-Lab
Simulated failed SSH login attempts from a Windows 10 VM to a Linux Logger VM. Wazuh monitored /var/log/auth.log and detected the authentication failures using Rule ID 5503, mapping them to MITRE ATT&amp;CK T1110.001 (Password Guessing). Alerts were successfully analyzed in the Wazuh Dashboard in real time.
