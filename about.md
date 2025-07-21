# 🧠 AI Guard Manager - Governance, Security & Compliance System

A complete platform for managing secure, ethical, and compliant AI deployments across enterprises.

---

## 🛡️ 1. AI Guardrail Enforcement Engine

**Purpose:** Prevent risky or non-compliant AI behavior in real time.

**Features:**
- Input and output **guardrails** defined in YAML.
- Support for `regex` and `keyword` triggers with severity levels:
  - `low` (warn), `medium` (fail), `high` (block).
- Modular enforcement flow:
  ```
  Agent → Input Guardrail → Output Guardrail → Compliance Check → LLM Response
  ```
- Support for `privacy_guard` to detect/redact:
  - Emails, SSNs, phone numbers, PII
- Logs violations for audit and trend analysis.
- Optional ML-based PII detection with spaCy.

---

## 🧠 2. Persona and Agent Framework

**Purpose:** Define behavior, tone, and rules for AI agents.

**Features:**
- YAML-based persona definitions (role, tone, intent).
- Agent YAMLs contain enforceable rules and structure.
- Supports dynamic agent composition and reuse.
- Enables roleplay, policy enforcement, or ethical limits.

---

## 🔄 3. Full Stack Testing Framework

**Purpose:** Simulate and evaluate full AI conversations.

**Features:**
- Combines agents, guardrails, compliance, and privacy checks.
- Test prompt flows through all layers.
- Outputs:
  - LLM response
  - Input/output violations
  - Compliance report
- Supports saving and reloading named test cases (versioned).

---

## 🧪 4. Sandbox Simulation Environment

**Purpose:** Test configurations before production deployment.

**Features:**
- Web UI for agent/guardrail selection and live prompt testing.
- Checkbox toggles for:
  - Input Guardrail
  - Output Guardrail
  - Compliance
  - Privacy Guard
- Visual breakdown of results:
  - LLM output
  - Violations
  - Compliance scores
  - Trace steps

---

## 📋 5. AI Compliance Check Module

**Purpose:** Ensure every LLM response meets regulatory standards.

**Features:**
- Supports compliance models: ISO, NIST AI RMF, EU AI Act.
- External service integration for objective scoring.
- Includes:
  - Main compliance score
  - Transparency score
  - Self-assessment output from LLM
  - Category-based scoring (e.g., bias, ethics, safety)
- Option to block/fail based on score thresholds.

---

## 📈 6. AI Analytics & Trend Dashboard

**Purpose:** Monitor system effectiveness and usage.

**Features:**
- Token usage reports
- Violation trends (input/output/compliance)
- Guardrail and agent effectiveness tracking
- Exportable logs

---

## 🛠️ 7. Admin Console & Governance Tools

**Features:**
- Manage users and roles (RBAC)
- Manage LLM connections and models
- SSO, SIEM, WAF, and bug tracker integration
- Guide/document uploads
- Inventory management for AI projects
- Help pages for all features

---

## 📚 8. Documentation & Help System

- Built-in help pages for each component
- Markdown/YAML editor support
- Conformance with enterprise onboarding and audit needs
