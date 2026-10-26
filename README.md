# Cybersecurity-CTF-Labs-Collection-Advanced-Cross-Site-Scripting-XSS-CSP-Bypass
A curated, searchable index of hands-on CTF labs covering DOM XSS, Stored XSS, Blind XSS, Mutation XSS, Polyglot payloads, CSP bypass, and framework escapes from Learn SecByte.
# Advanced Cross-Site Scripting (XSS) & CSP Bypass CTF Labs Collection

A structured, searchable index of hands-on cybersecurity labs focusing on Cross-Site Scripting (XSS) filter evasion, Content Security Policy (CSP) bypasses, DOM-based sources and sinks, Stored XSS persistence, Blind XSS beaconing, Mutation XSS (mXSS), Polyglot payloads, and framework-specific template/sandbox escapes hosted on Learn SecByte.

This collection is designed for application security engineers, penetration testers, CTF competitors, security researchers, and front-end web developers aiming to master client-side script execution risks and browser rendering defenses.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
  - [XSS Core Mechanics & Client-Side Execution](#xss-core-mechanics--client-side-execution)
  - [Filter Evasion, Encoding & CSP Bypasses](#filter-evasion-encoding--csp-bypasses)
  - [Format-Specific & Framework XSS Attacks](#format-specific--framework-xss-attacks)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Cross-Site Scripting (XSS) remains one of the most widespread client-side web application vulnerabilities. Modern browsers and security controls like Content Security Policy (CSP) and HTML sanitizers aim to prevent unauthorized script execution, but complex parser behaviors, DOM sinks, template engines, and unsafe image formats often create injection vectors.

This repository organizes hands-on cybersecurity labs from Learn SecByte into structured learning paths covering client-side security, payload crafting, and modern browser defense mechanisms.

---

## Lab Collection & Index

| Lab Title | Primary Category | Vulnerability / Focus | Access Link |
| :--- | :--- | :--- | :--- |
| **XSS Filter Evasion** | Client-Side Security | WAF & Filter Bypass | [Access Lab](https://learn.secbyte.org/ctf/xss-filter-evasion-lab) |
| **CSP Bypass** | Browser Security | Content Security Policy Evasion | [Access Lab](https://learn.secbyte.org/ctf/csp-bypass-from-policy-basics-to-real-world-exploitation) |
| **Template XSS** | Client-Side Security | Client-Side Template Injection | [Access Lab](https://learn.secbyte.org/ctf/template-xss-from-templating-logic-to-exploitation-and-defen) |
| **AngularJS Sandbox Escape** | Framework Security | Client-Side Sandbox Escape | [Access Lab](https://learn.secbyte.org/ctf/angularjs-sandbox-escape) |
| **JSON XSS** | Data Parsing | Unsafe JSON Processing Boundaries | [Access Lab](https://learn.secbyte.org/ctf/json-xss-parsing-trust-boundaries) |
| **Markdown XSS** | Content Rendering | Unsafe Markdown Parsing to Script Exec | [Access Lab](https://learn.secbyte.org/ctf/markdown-xss-from-unsafe-rendering-to-browser-controlled-exp) |
| **SVG XSS** | Media Parsing | Vector Graphic Payload Weaponization | [Access Lab](https://learn.secbyte.org/ctf/svg-xss-weaponizing-safe-looking-vector-images) |
| **Polyglot XSS** | Payload Crafting | Context-Agnostic Executable Payloads | [Access Lab](https://learn.secbyte.org/ctf/polyglot-xss-from-curious-payloads-to-reliable-exploitation) |
| **Mutation XSS (mXSS)** | Browser Parsing | HTML Sanitizer & DOM Mutation Abuse | [Access Lab](https://learn.secbyte.org/ctf/mutation-xss-when-safe-html-becomes-dangerous) |
| **Blind XSS** | Client-Side Security | Out-of-Band Callback & Beaconing | [Access Lab](https://learn.secbyte.org/ctf/blind-xss-from-injection-to-beaconing) |
| **DOM XSS** | Client-Side Security | Unsafe DOM Source to Sink Tracking | [Access Lab](https://learn.secbyte.org/ctf/dom-xss-from-source-to-sink) |
| **Stored XSS** | Client-Side Security | Persistent Injection & Execution | [Access Lab](https://learn.secbyte.org/ctf/stored-xss-from-persistence-to-impact) |

---

## Categories

### XSS Core Mechanics & Client-Side Execution
Hands-on CTF labs exploring persistent storage, client-side data flows, and out-of-band execution:

* **Stored XSS:** Injecting persistent script payloads into database layers to target application users and administrators.
  * Lab Link: https://learn.secbyte.org/ctf/stored-xss-from-persistence-to-impact
* **DOM XSS Source-to-Sink Tracking:** Tracing untrusted user inputs (`location.hash`, `document.referrer`) into execution sinks (`eval()`, `innerHTML`).
  * Lab Link: https://learn.secbyte.org/ctf/dom-xss-from-source-to-sink
* **Blind XSS & Beaconing:** Injecting payloads into non-visible administrative consoles and collecting out-of-band HTTP/DNS callbacks.
  * Lab Link: https://learn.secbyte.org/ctf/blind-xss-from-injection-to-beaconing

### Filter Evasion, Encoding & CSP Bypasses
Practical security labs demonstrating browser parsing quirks, sanitizer bypasses, and policy misconfigurations:

* **XSS Filter Evasion:** Bypassing Web Application Firewalls (WAF) and blacklists using alternative encodings, tags, and execution contexts.
  * Lab Link: https://learn.secbyte.org/ctf/xss-filter-evasion-lab
* **CSP Bypass:** Evaluating Content Security Policy directives (`unsafe-inline`, `script-src`, JSONP endpoints) to execute unauthorized scripts.
  * Lab Link: https://learn.secbyte.org/ctf/csp-bypass-from-policy-basics-to-real-world-exploitation
* **Polyglot XSS:** Constructing universal polyglot payloads that execute across multiple HTML, attribute, and JavaScript contexts.
  * Lab Link: https://learn.secbyte.org/ctf/polyglot-xss-from-curious-payloads-to-reliable-exploitation
* **Mutation XSS (mXSS):** Abusing browser innerHTML parsing and DOM mutation behavior to bypass HTML sanitization libraries.
  * Lab Link: https://learn.secbyte.org/ctf/mutation-xss-when-safe-html-becomes-dangerous

### Format-Specific & Framework XSS Attacks
Security labs covering client-side template engines, vector images, document parsers, and data serialization:

* **Template XSS:** Exploiting Client-Side Template Injection (CSTI) within modern JavaScript templating logic.
  * Lab Link: https://learn.secbyte.org/ctf/template-xss-from-templating-logic-to-exploitation-and-defen
* **AngularJS Sandbox Escape:** Breaking out of legacy AngularJS template sandboxes to invoke arbitrary window objects.
  * Lab Link: https://learn.secbyte.org/ctf/angularjs-sandbox-escape
* **Markdown XSS:** Bypassing Markdown parsers and converters to inject raw HTML and script elements.
  * Lab Link: https://learn.secbyte.org/ctf/markdown-xss-from-unsafe-rendering-to-browser-controlled-exp
* **SVG XSS:** Weaponizing XML-based Scalable Vector Graphics (SVG) using embedded `<script>` tags and event handlers.
  * Lab Link: https://learn.secbyte.org/ctf/svg-xss-weaponizing-safe-looking-vector-images
* **JSON XSS Parsing Boundaries:** Exploiting unsafe JSON data handling and dynamic DOM construction from API responses.
  * Lab Link: https://learn.secbyte.org/ctf/json-xss-parsing-trust-boundaries

---

## Learning Path

Follow this structured roadmap to master Cross-Site Scripting exploitation and browser defenses:

1. **XSS Fundamentals & Source-to-Sink Analysis**
   - Study Stored XSS persistence and analyze DOM XSS execution sinks.
   - Practice Blind XSS injection and set up out-of-band listener beacons.
2. **Filter Evasion & Advanced Payload Crafting**
   - Practice character encoding tricks, alternative tags, and context-agnostic polyglot payloads.
   - Analyze browser DOM mutations to execute Mutation XSS (mXSS).
3. **Browser Policy Bypasses & Framework Exploitation**
   - Audit Content Security Policies (CSP) and exploit misconfigured directives.
   - Master Client-Side Template Injection (CSTI) and AngularJS sandbox escapes.
4. **Media & Document Parser Auditing**
   - Test SVG image uploads, Markdown document processing, and JSON API rendering boundaries.
   - Implement context-aware output encoding, strict CSP nonces, and safe DOM manipulation methods (`textContent`).

---

## How to Use the Labs

1. Select a practice scenario from the index table or category breakdown above.
2. Access the interactive target lab environment directly on Learn SecByte.
3. Utilize web proxies (e.g., Burp Suite) and browser developer consoles to trace DOM sources/sinks, bypass WAF filters, and construct custom payloads.
4. Review defensive controls to learn how context-aware output encoding, strict CSP policies, and DOMPurify sanitization secure applications.

---

## Disclaimer

This repository is strictly intended for educational research, authorized security testing, and defensive engineering training. All concepts, techniques, and lab environments are provided to help cybersecurity practitioners identify vulnerabilities and harden modern front-end applications. Unsanctioned testing or attacks against external systems without prior written authorization are strictly illegal.
