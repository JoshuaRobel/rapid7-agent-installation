# Rapid7 Agent Installation & Endpoint Onboarding

## Project Overview

This project demonstrates installation and onboarding of a Rapid7 Insight Agent on a Windows virtual machine endpoint for ingestion into Rapid7 InsightIDR.

The objective was to validate endpoint telemetry collection and confirm successful asset visibility within the SIEM.

---

## Objectives

- Generate an Insight Agent installation token
- Deploy Rapid7 agent to a Windows VM
- Verify agent installation and background services
- Confirm endpoint visibility in Rapid7
- Validate asset metadata collection

---

## Technologies Used

- Rapid7 InsightIDR
- Windows VM
- Windows Task Manager
- Windows File Explorer
- Endpoint Monitoring

---

## Demo Video

▶️ Add video here

---

## SOP / Walkthrough

### Step 1 — Navigate to Asset Management

1. Log into Rapid7 InsightIDR
2. Navigate to:

```txt
Assets & Endpoints → Download Agent
```

---

### Step 2 — Generate Installation Token

1. Select installer
2. Generate a token
3. Copy token for onboarding

Purpose:
This token authenticates the endpoint with Rapid7.

---

### Step 3 — Download Appropriate Agent

Selected:

```txt
Windows ARM Agent
```

Reason:

The environment was running a Windows ARM virtual machine.

---

### Step 4 — Transfer Installer to Endpoint

The installer was moved into the VM shared folder and executed inside the Windows VM.

---

### Step 5 — Install Insight Agent

Installation steps:

1. Launch installer
2. Paste generated token
3. Complete installation wizard

---

### Step 6 — Validate Local Installation

Verification methods:

#### Task Manager Validation

Confirmed Rapid7 background services were running:

- Rapid7 Insight Agent
- Endpoint Broker
- IR Agent

#### Program Files Validation

Verified installation directory existed:

```txt
Program Files\Rapid7
```

---

### Step 7 — Validate Endpoint in Rapid7

Navigated to:

```txt
Assets & Endpoints
```

Validated:

- Endpoint appeared successfully
- Agent status visible
- Host details populated
- OS information collected
- Internal IP visible

---

## Outcome

The Rapid7 Insight Agent was successfully deployed to a Windows endpoint and validated through both local system verification and Rapid7 asset visibility.

---

## Skills Demonstrated

- Endpoint onboarding
- Rapid7 administration
- Windows troubleshooting
- Asset validation
- Security telemetry ingestion
