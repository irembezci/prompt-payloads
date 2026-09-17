# LLM Security Payloads & Techniques

A practical cheat sheet for testing LLM applications from a black-box security testing perspective.

This repository focuses on common LLM attack techniques, example payloads and the indicators that can help identify vulnerabilities during security assessments.

The goal is not to provide a universal payload for every target. Instead, the examples demonstrate different attack patterns that can be adapted based on the application's behavior, architecture and attack surface.

## Attack Categories

| #  | Category                           |
| -- | ---------------------------------- |
| 01 | Prompt Injection                   |
| 02 | Indirect Prompt Injection          |
| 03 | Jailbreaking                       |
| 04 | System Prompt Extraction           |
| 05 | RAG Injection / RAG Poisoning      |
| 06 | Data Exfiltration                  |
| 07 | Tool / Agent Injection             |
| 08 | Excessive Agency                   |
| 09 | Insecure Output Handling           |
| 10 | MCP Security                       |
| 11 | Memory / Context Poisoning         |
| 12 | Model / Application Fingerprinting |
| 13 | Model DoS / Resource Exhaustion    |

## How to Use This Cheat Sheet

The testing approach follows a simple black-box workflow:

`Discover → Establish Baseline → Identify Attack Surface → Select Technique → Test Payload → Observe Behavior → Escalate / Pivot`

For each category, the cheat sheet covers:

* **Definition** — What the vulnerability or attack technique is
* **Attack Flow** — How the attack moves through the application
* **Payload Examples** — Example inputs that can be adapted during testing
* **What to Look For** — Indicators of vulnerable behavior
* **Black-Box Approach** — How to identify and test the attack without internal access

A payload should not be treated as a guaranteed exploit. LLM behavior can vary depending on the model, system prompt, guardrails, context, temperature, application logic and backend architecture.

## Scope

These techniques are intended for authorized security testing, CTFs, labs and controlled environments.

Do not test systems you do not have permission to assess.

## Disclaimer

This repository is intended for educational purposes, security research, CTFs and authorized security testing only.

The techniques and payload examples provided here are designed to help security practitioners understand and assess vulnerabilities in LLM-powered applications. They should only be used against systems where you have explicit permission to conduct security testing.

The author is not responsible for any misuse, damage, data loss, service disruption or unauthorized activity resulting from the use of the information in this repository.

Always define the testing scope, rules of engagement and appropriate safety limits before conducting security assessments.
