# SSH Brute Force Detection – Linux (Kali)

## Objective
To simulate and detect an SSH brute-force attack and implement mitigation as part of SOC Level-1 operations.

## Tools Used
- Kali Linux
- Hydra
- SSH
- journalctl
- Fail2Ban

## Attack Simulation
- Created a test user account
- Performed SSH brute-force attack using Hydra
- Generated multiple failed authentication attempts

## Detection
- Analyzed SSH authentication logs using journalctl
- Identified repeated failed login attempts
- Extracted attacker IP address
- Counted failed attempts to confirm brute-force behavior

## Mitigation
- Installed and enabled Fail2Ban
- Automatically blocked attacker IP after repeated failures

## Skills Gained
- Brute-force attack detection
- Log-based investigation
- SOC incident response
- Basic attack mitigation
