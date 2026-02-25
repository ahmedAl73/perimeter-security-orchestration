# ZT-Policy-Profile.md

---

## 1. ZTA Component Definitions

### Policy Engine (PE)

The Policy Engine (PE) is the part of a Zero Trust Architecture that makes decisions. It checks every access request by looking at security signals such the user's identity, the device's posture, the network location, and the amount of danger. It decides whether to give access, deny it, or ask for more proof based on set organizational rules and the current situation. The Policy Engine doesn't immediately stop or let traffic through; its main job is to make a reasonable, risk-based decision about who can access what.

### Policy Administrator (PA)

The Policy Administrator (PA) is in charge of carrying out the decision made by the Policy Engine. The Policy Engine decides whether or not to allow access, and then the Policy Administrator puts that decision into action. This could mean starting a secure session, giving over credentials, making sure that multi-factor authentication is used, or ending the request. The PA makes ensuring that the system appropriately carries out policy decisions.

### Policy Enforcement Point (PEP)

The Policy Enforcement Point (PEP) is the gatekeeper that keeps the resource safe. It sits between the user and the protected system and makes sure that access control decisions made by the Policy Administrator are followed. The PEP lets or blocks access based only on those instructions. It doesn't make decisions or analyze policies on its own; it just carries out the decision made by the Zero Trust process.

---

## 2. Core Principle Application

### Chosen Principle: Verify Explicitly

The principle of Verify Explicitly says that every request for access must be checked against several security signals before access is given. You should never trust someone just because they are on your network or have logged in before.
The Policy Engine makes sure that this rule is followed at the Golden State Water Treatment Facility when an HR employee tries to get to the Employee PII Database. The Policy Engine looks at the user's role, the security of the device, and where the request is coming from on the network.
The Policy Engine won't let someone in if their device isn't encrypted or completely patched, or if the request comes from an unapproved location, even if they have the right credentials. The Policy Engine makes sure that important HR data stays safe by checking the identity, device compliance, and network context of every request.

---

## 3. Simplified Policy Table

**Target Resource:** HR Employee PII Database  
**Organization:** Golden State Water Treatment Facility  

| Policy Requirement (Signal) | Condition to be Met by User | Action if Condition is Met |
|------------------------------|-----------------------------|----------------------------|
| User Identity | Must authenticate using MFA and have an active HR role | Grant Access |
| Device Posture | Device must be company-managed, encrypted, and fully patched | Grant Access |
| Network Context | Connection must originate within the U.S. using approved secure VPN | Grant Access |
---

## 4. Submission Details

# Git Repository Metadata

Project: Lab 6 - Zero Trust Policy  

Filename: ZT-Policy-Profile.md  

Commit Message: Completed ZT Policy Profile defining PE, PA, PEP and HR PII Zero Trust enforcement - [https://github.com/ahmedAI73/perimeter-security-orchestration](https://github.com/ahmedAl73/perimeter-security-orchestration/blob/main/ZT-Policy-Profile.md)

Due Date: March 2, 2026  
