# Constitutional Auditing of Pre-trained Models

**Team:** Leeuwenhoek

---

## Overview

This project implements **constitutional auditing** for large language models (LLMs). The goal is to define and enforce organizational policies ("constitutions")—for example, no profanity, no disclosure of sensitive employee information, SSNs, etc. —across various LLM deployments.

## Motivation

Organizations often have internal rules and policies beyond 3H (Helpful, Healthy and Honest). Enforcing these constitutions consistently in LLM-powered applications is crucial for enterprises and non compliance may be linked to high fines or loss of reputation.

Possible methods to implement constitutions are:

- System prompts (eg custom GPTs)
- Hard-coded rules 
- control over organizational context as in RAG or external data stores

By developing a testing framework around a formalized constitution, we can evaluate and compare how well different LLMs adhere to policy in diverse environments.

## Key Concepts

- **Constitution**: A formal specification of policies (e.g., prohibited content, privacy rules).
- **Auditing**: Automated testing of LLM outputs against the constitution.
- **Environment**: The interface through which users interact (e.g., browser proxy, direct API, or low-resource model).

## What’s Been Achieved (as of April 30, 2025)

- Initial prototype for launching test prompts via Python scripts.
> _Having fun! Probably not ready by the end of the hackathon._

## Work To Be Done

1. **Define a testing constitution**: Create a structured format (e.g., YAML or JSON) for policy rules.
2. **Evaluate enforcement techniques**: Compare system prompts, rule-based filters, and external data controls.
3. **Benchmark multiple LLMs**: Test models of varying sizes (e.g., SLM, 0.5B parameters, GPT-4).
4. **Assess environment impact**:
   - Browser-mediated (user-facing via web UI)
   - Alternative UIs (e.g., voice, specialized client)
   - Direct API integration
5. **Quantitative analysis**: Use Python to automate prompt execution and gather compliance statistics.

## Project Structure

```plaintext
├── constitutions/       # Sample constitution files (YAML/JSON)
├── src/                 # Python scripts for testing and data collection
├── data/                # Raw and processed results
├── requirements.txt     # Python dependencies
└── README.md            # This document
```

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

_Developed by Team Leeuwenhoek during Hackathon 2025_

