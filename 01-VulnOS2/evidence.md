# Screenshot Evidence — All 30 Original Images

[← Lab overview](README.md) · [Technical walkthrough](walkthrough.md) · [← Portfolio](../README.md)

This archive preserves **every screenshot provided for Lab 01**, in order, with its **original filename and original image bytes**. None of the images were excluded, renamed, cropped, or retouched. The first screenshot documents the initial NAT stage; subsequent images capture the switch to Host-Only and the full challenge.

> **Public disclosure warning:** Screenshots **25 and 28** include training-lab account data, full password hashes, and a recovered plaintext password. Other screenshots may show lab-only logins or the final flag. All 30 are included *unredacted* because the complete set was explicitly requested. **Do not publish this repository publicly if any password was reused outside this intentionally vulnerable VM.**

| Range | Focus |
| :-- | :-- |
| 01–04 | VM network, host discovery, service scans |
| 05–19 | VulnOS / JABC, Drupal pages, source disclosure |
| 20–25 | OpenDocMan research, endpoint, SQL injection and data retrieval |
| 26–30 | Hash assessment, SSH access, root flag |

## Phase A — Network and reconnaissance (01–04)

<details>
<summary><strong>01. Initial Kali NAT address, before Host-Only configuration</strong> — <code>lab1.1.png</code></summary>

![Screenshot 01: Initial Kali NAT address, before Host-Only configuration](screenshots/lab1.1.png)

</details>

<details>
<summary><strong>02. Host-Only IP and successful Nmap discovery of four active hosts</strong> — <code>lab1.2.png</code></summary>

![Screenshot 02: Host-Only IP and successful Nmap discovery of four active hosts](screenshots/lab1.2.png)

</details>

<details>
<summary><strong>03. Small port scan of two unidentified addresses</strong> — <code>lab1.3.png</code></summary>

![Screenshot 03: Small port scan of two unidentified addresses](screenshots/lab1.3.png)

</details>

<details>
<summary><strong>04. Service version enumeration: SSH, Apache and IRC</strong> — <code>lab1.4.png</code></summary>

![Screenshot 04: Service version enumeration: SSH, Apache and IRC](screenshots/lab1.4.png)

</details>

## Phase B — Drupal and website exploration (05–19)

<details>
<summary><strong>05. VulnOS 2 landing page and challenge objective</strong> — <code>lab1.5.png</code></summary>

![Screenshot 05: VulnOS 2 landing page and challenge objective](screenshots/lab1.5.png)

</details>

<details>
<summary><strong>06. JABC website discovered at /jabc/</strong> — <code>lab1.6.png</code></summary>

![Screenshot 06: JABC website discovered at /jabc/](screenshots/lab1.6.png)

</details>

<details>
<summary><strong>07. WhatWeb detects Drupal, Apache, PHP and jQuery</strong> — <code>lab1.7.png</code></summary>

![Screenshot 07: WhatWeb detects Drupal, Apache, PHP and jQuery](screenshots/lab1.7.png)

</details>

<details>
<summary><strong>08. CHANGELOG.txt returns 404 from /jabc/</strong> — <code>lab1.8.png</code></summary>

![Screenshot 08: CHANGELOG.txt returns 404 from /jabc/](screenshots/lab1.8.png)

</details>

<details>
<summary><strong>09. Drupal robots.txt and crawler exclusions</strong> — <code>lab1.9.png</code></summary>

![Screenshot 09: Drupal robots.txt and crawler exclusions](screenshots/lab1.9.png)

</details>

<details>
<summary><strong>10. CHANGELOG.txt returns 404 from the web root</strong> — <code>lab1.10.png</code></summary>

![Screenshot 10: CHANGELOG.txt returns 404 from the web root](screenshots/lab1.10.png)

</details>

<details>
<summary><strong>11. Drupal user-login interface</strong> — <code>lab1.11.png</code></summary>

![Screenshot 11: Drupal user-login interface](screenshots/lab1.11.png)

</details>

<details>
<summary><strong>12. Drupal registration form</strong> — <code>lab1.12.png</code></summary>

![Screenshot 12: Drupal registration form](screenshots/lab1.12.png)

</details>

<details>
<summary><strong>13. Documentation node looks visually empty</strong> — <code>lab1.13.png</code></summary>

![Screenshot 13: Documentation node looks visually empty](screenshots/lab1.13.png)

</details>

<details>
<summary><strong>14. JABS catalog with three model links</strong> — <code>lab1.14.png</code></summary>

![Screenshot 14: JABS catalog with three model links](screenshots/lab1.14.png)

</details>

<details>
<summary><strong>15. MODEL-101 product node</strong> — <code>lab1.15.png</code></summary>

![Screenshot 15: MODEL-101 product node](screenshots/lab1.15.png)

</details>

<details>
<summary><strong>16. MODEL-202 product node</strong> — <code>lab1.16.png</code></summary>

![Screenshot 16: MODEL-202 product node](screenshots/lab1.16.png)

</details>

<details>
<summary><strong>17. MODEL-404 product node</strong> — <code>lab1.17.png</code></summary>

![Screenshot 17: MODEL-404 product node](screenshots/lab1.17.png)

</details>

<details>
<summary><strong>18. SearchSploit research for Drupal 7</strong> — <code>lab1.18.png</code></summary>

![Screenshot 18: SearchSploit research for Drupal 7](screenshots/lab1.18.png)

</details>

<details>
<summary><strong>19. HTML source reveals secondary application clue and demo login</strong> — <code>lab1.19.png</code></summary>

![Screenshot 19: HTML source reveals secondary application clue and demo login](screenshots/lab1.19.png)

</details>

## Phase C — OpenDocMan and SQL injection (20–25)

<details>
<summary><strong>20. OpenDocMan login screen and displayed version 1.2.7</strong> — <code>lab1.20.png</code></summary>

![Screenshot 20: OpenDocMan login screen and displayed version 1.2.7](screenshots/lab1.20.png)

</details>

<details>
<summary><strong>21. SearchSploit research for OpenDocMan</strong> — <code>lab1.21.png</code></summary>

![Screenshot 21: SearchSploit research for OpenDocMan](screenshots/lab1.21.png)

</details>

<details>
<summary><strong>22. Published OpenDocMan advisory viewed in browser</strong> — <code>lab1.22.png</code></summary>

![Screenshot 22: Published OpenDocMan advisory viewed in browser](screenshots/lab1.22.png)

</details>

<details>
<summary><strong>23. Direct browser inspection of ajax_udf.php endpoint</strong> — <code>lab1.23.png</code></summary>

![Screenshot 23: Direct browser inspection of ajax_udf.php endpoint](screenshots/lab1.23.png)

</details>

<details>
<summary><strong>24. SQLmap target invocation and previously detected injection point</strong> — <code>lab1.24.png</code></summary>

![Screenshot 24: SQLmap target invocation and previously detected injection point](screenshots/lab1.24.png)

</details>

<details>
<summary><strong>25. SQLmap dump of two odm_user rows, including lab account hashes</strong> — <code>lab1.25.png</code></summary>

![Screenshot 25: SQLmap dump of two odm_user rows, including lab account hashes](screenshots/lab1.25.png)

</details>

## Phase D — Password, SSH, and root (26–30)

<details>
<summary><strong>26. Hash-identifier results: likely MD5</strong> — <code>lab1.26.png</code></summary>

![Screenshot 26: Hash-identifier results: likely MD5](screenshots/lab1.26.png)

</details>

<details>
<summary><strong>27. John the Ripper dictionary run ending with zero recovered passwords</strong> — <code>lab1.27.png</code></summary>

![Screenshot 27: John the Ripper dictionary run ending with zero recovered passwords](screenshots/lab1.27.png)

</details>

<details>
<summary><strong>28. Known-hash lookup returns a plaintext match for the lab hash</strong> — <code>lab1.28.png</code></summary>

![Screenshot 28: Known-hash lookup returns a plaintext match for the lab hash](screenshots/lab1.28.png)

</details>

<details>
<summary><strong>29. SSH login as webmin and initial operating-system enumeration</strong> — <code>lab1.29.png</code></summary>

![Screenshot 29: SSH login as webmin and initial operating-system enumeration](screenshots/lab1.29.png)

</details>

<details>
<summary><strong>30. Compiled local escalation program, root shell and final flag</strong> — <code>lab1.30.png</code></summary>

![Screenshot 30: Compiled local escalation program, root shell and final flag](screenshots/lab1.30.png)

</details>

---

**Evidence completeness:** 30/30 original screenshots included in `screenshots/`.
