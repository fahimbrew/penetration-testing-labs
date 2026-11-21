# Penetration Testing Labs

**Hands-on security research in isolated, intentionally vulnerable environments.**

This repository contains practical penetration-testing labs with concise lab summaries, reproducible technical notes, original evidence, and security recommendations. The goal is to document **what was observed**, **what was verified**, and **what can be improved**—without confusing vulnerability research with proven exploitation.

## Completed labs

| # | Lab | Topics | Result | Documentation |
| :-- | :-- | :-- | :-- | :-- |
| 01 | **VulnOS 2** | Network scanning, Drupal discovery, OpenDocMan SQLi, password analysis, SSH, local privilege escalation | **Root flag obtained** | [Open lab](01-VulnOS2/README.md) |

## Lab 01 at a glance

```text
Windows 11 Host
  └── Oracle VirtualBox (Host-Only network: 192.168.56.0/24)
        ├── Kali Linux   · Attacker · 192.168.56.102
        └── VulnOS 2    · Target   · 192.168.56.101
```

**Attack path:** Host discovery → Service enumeration → Drupal site → Source-code clue → OpenDocMan → SQL injection → Credential exposure → SSH access → Root shell.

[Read the lab overview](01-VulnOS2/README.md) · [Technical walkthrough](01-VulnOS2/walkthrough.md) · [All 30 screenshots](01-VulnOS2/evidence.md)

## Methodology

The labs follow **scope → discover → enumerate → validate → assess impact → document and recommend**. Evidence is labeled separately from interpretation; unsuccessful attempts are recorded rather than hidden.

## Tools used in Lab 01

Kali Linux · Oracle VirtualBox · Nmap · curl · WhatWeb · SearchSploit · SQLmap · John the Ripper · SSH · Linux CLI

---

> **Authorization and spoilers:** Every exercise here was performed against an intentionally vulnerable VM in a locally controlled Host-Only network. These reports contain solution details, including final challenge proof. Do not test devices without explicit permission. Some original training screenshots contain deliberately vulnerable lab credentials and hashes; see the evidence gallery's disclosure notice before making a public fork.
