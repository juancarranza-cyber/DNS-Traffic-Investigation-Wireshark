# DNS Traffic Investigation with Wireshark

## Introduction

This project demonstrates the investigation of DNS traffic using Wireshark.

The objective of the lab was to capture DNS communications, analyze DNS queries and responses, identify domain resolution activity, and understand how DNS traffic can be monitored from a defensive cybersecurity perspective.

DNS is one of the most important protocols analyzed by SOC analysts because it provides visibility into domains accessed by systems and can help identify suspicious or malicious network activity.

## Lab Environment

* Windows 10
* Wireshark
* Web Browser
* Local Network Environment

## Investigation Objectives

* Capture DNS traffic
* Analyze DNS queries and responses
* Identify domain resolution activity
* Review source and destination communication

## 1. Wireshark Setup

The investigation began by launching Wireshark and selecting the active network interface used for Internet connectivity.

Wireshark is a widely used packet analysis tool that provides visibility into network communications and allows analysts to inspect protocols, monitor traffic, and investigate network activity in real time.

Selecting the correct interface is an important first step because it ensures that relevant traffic is captured during the investigation.

![Wireshark Interface](Wireshark/01_Wireshark_Interface.PNG)

---

## 2. DNS Traffic Capture Configuration

After selecting the network interface, packet capture was initiated and a DNS display filter was applied.

Filter used:

```text
dns
```

Applying protocol filters helps analysts focus on specific types of traffic and reduces the amount of unrelated network activity displayed during an investigation.

This approach is commonly used in SOC environments when analyzing DNS communications, HTTP traffic, authentication protocols, and other network activity.

![DNS Filter](Wireshark/02_DNS_Filter.PNG)

---

## 3. DNS Traffic Generation

To generate DNS activity, several websites were accessed through a web browser while Wireshark was actively capturing packets.

Example domains visited included:

* github.com
* google.com
* microsoft.com
* wikipedia.org

As the browser attempted to access these domains, DNS queries and responses were generated and captured by Wireshark.

The resulting packet capture provided the evidence required for further analysis of domain resolution activity.

![DNS Traffic](Wireshark/03_DNS_Traffic.PNG)


















* Understand DNS monitoring techniques
* Develop network traffic analysis skills
