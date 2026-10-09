# 🛡️ Responding to an ICMP Flood Incident with the NIST CSF

*As a cybersecurity trainee, I applied the NIST Cybersecurity Framework to a Denial of Service (DoS) incident.*

---

## 📋 Scenario Overview

I am a cybersecurity analyst working for a multimedia company that offers web design, graphic design, and social media marketing services to small businesses. The company recently experienced a denial of service (DoS) attack that compromised the internal network for two hours until it was resolved.

During the attack, the organization's network services suddenly stopped responding because of an incoming flood of ICMP packets, and normal internal traffic could not reach any network resources. The incident management team responded by blocking incoming ICMP packets, taking all non-critical network services offline, and restoring critical network services.

The cybersecurity team then investigated and found that a malicious actor had sent a flood of ICMP pings into the network through an unconfigured firewall. This vulnerability allowed the attacker to overwhelm the network.

To address the event, the network security team implemented:

- A new firewall rule to limit the rate of incoming ICMP packets
- Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets
- Network monitoring software to detect abnormal traffic patterns
- An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics

My task is to use this security event to build a plan that improves the company's network security, following the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF).

---

## 🚨 Incident Report

### Summary of the incident

The company experienced a security event when all network services suddenly stopped responding for two hours. The cybersecurity team determined that the disruption was caused by a denial of service attack in the form of an ICMP packet flood. The incident management team blocked the incoming ICMP packets, stopped all non-critical network services, and restored the critical services so that normal operations could resume.

### Analysis of the cause of the incident

The investigation showed that the attack succeeded because the company's firewall was not configured to limit or verify incoming ICMP traffic. A malicious actor took advantage of this gap by sending a flood of ICMP pings that overwhelmed the network and left no capacity for legitimate internal traffic. The new firewall rule, source IP verification, network monitoring, and IDS/IPS system now address that gap, and the NIST CSF gives the company a structure to keep identifying, protecting, detecting, responding, and recovering from similar threats.

## 🧭 NIST CSF Analysis

### Identify

A malicious actor or actors targeted the company with an ICMP flood attack. The entire internal network was affected. All critical network resources needed to be secured and restored to a functioning state.

### Protect

The cybersecurity team implemented a new firewall rule to limit the rate of incoming ICMP packets and an IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics.

### Detect

The cybersecurity team configured source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets and implemented network monitoring software to detect abnormal traffic patterns. 

### Respond

For future security events, the cybersecurity team will isolate affected systems to prevent further disruption to the network. They will attempt to restore any critical systems and services that were disrupted by the event. Then, the team will analyze network logs to check for suspicious and abnormal activity. The team will also report all incidents to upper management and appropriate legal authorities, if applicable.

### Recover

To recover from a DDoS attack by ICMP flooding, access to network services need to be restored to a normal functioning state. In the future, external ICMP flood attacks can be blocked at the firewall. Then, all non-critical network services should be stopped to reduce internal network traffic. Next, critical network services should be restored first. Finally, once the flood of ICMP packets have timed out, all non-critical network systems and services can be brought back online.
