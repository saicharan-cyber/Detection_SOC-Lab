# Project 01 - Failed SSH Login Detection Using Wazuh

## Objective
Detect failed SSH login attempts on a Linux Logger VM using Wazuh SIEM.

## Lab Environment
- Wazuh Manager
- Wazuh Dashboard
- Wazuh Indexer
- Logger VM (Ubuntu Linux)
- Windows 10 VM
- VirtualBox
- Vagrant

## Attack Simulation
From the Windows 10 VM:

```cmd
ssh vagrant@192.168.56.105
```

Entered an incorrect password multiple times.

## Log Location

```text
/var/log/auth.log
```

## Detection

- Rule ID: 5503
- Rule Level: 5
- Description: PAM: User login failed
- MITRE ATT&CK: T1110.001 – Password Guessing

## Result

Wazuh successfully detected the failed SSH login attempts and displayed real-time alerts in the Security Events dashboard.
