# Red Team: Summary of Operations

## Table of Contents
- Exposed Services
- Critical Vulnerabilities
- Exploitation

### Exposed Services

Nmap scan results for each machine reveal the below services and OS details:

```bash
$ nmap -sP 192.168.1.*
$ nmap -A 192.168.1.110
$ nmap -sV --script=vulners -v 192.168.1.110


This scan identifies the services below as potential points of entry:
- Target 1 -
  - Open ports:
  22/tcp ssh
  80/tcp http
  111/tcp rpcbind
  139/tcp netbios-ssn
  445/tcp microsoft-ds

  - Exposed Services:
  http://192.168.1.110:80

The following vulnerabilities were identified on each target:
- Target 1
  - List of
  - Critical
  - Vulnerabilities

_TODO: Include vulnerability scan results to prove the identified vulnerabilities._

### Exploitation
_TODO: Fill out the details below. Include screenshots where possible._

The Red Team was able to penetrate `Target 1` and retrieve the following confidential data:
- Target 1
  - `flag1.txt`: `flag1{b9bbcb33e11b80be759c4e844862482d}'
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_
  - `flag2.txt`: `flag2{fc3fd58dcdad9ab23faca6e9a36e581c}`
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_
