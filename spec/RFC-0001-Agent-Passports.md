# RFC-0001 Agent Passports

Status: Accepted

## Abstract

Agent Passports provide a cryptographically verifiable identity for autonomous systems operating within the Agentic Provenance Protocol.

An Agent Passport establishes identity, ownership, lifecycle status, capabilities, and federation trust relationships.

## Motivation

Autonomous systems require a standardized identity mechanism analogous to digital certificates on the traditional internet.

Without a common identity layer:

* Ownership cannot be verified
* Actions cannot be attributed
* Trust cannot be established
* Federation becomes unreliable

Agent Passports solve this problem.

## Passport Structure

A passport contains:

```json
{
  "agent_id": "agt_xxx",
  "owner_id": "org_xxx",
  "public_key": "...",
  "agent_class": "enterprise",
  "status": "active",
  "created_at": "...",
  "expires_at": "...",
  "capabilities": [],
  "federation_level": "trusted"
}
```

## Agent Classes

APP defines the following agent classes:

### Personal

Agents operating on behalf of individuals.

### Enterprise

Agents operating on behalf of organizations.

### Service

Infrastructure or platform agents.

### Marketplace

Agents acting as brokers or intermediaries.

### Government

Agents operated by government entities.

## Passport States

A passport may exist in one of the following states:

### Active

Valid and operational.

### Suspended

Temporarily restricted.

### Revoked

Permanently invalid.

### Expired

Validity period has ended.

## Ownership

Each passport MUST have a verifiable owner.

Ownership transfers MUST be recorded through the APP Ownership Framework.

## Federation

Passports MAY participate in federation networks.

Federated verification enables trust across independent APP nodes.

## Revocation

Revoked passports MUST NOT:

* Record provenance
* Issue attestations
* Participate in federation actions
* Exercise delegated authority

Revocation events MUST be recorded permanently.

## Security Considerations

Private keys MUST remain under the control of the passport holder.

Public keys MAY be distributed through APP federation mechanisms.

Compromised passports SHOULD be revoked immediately.

## Conclusion

Agent Passports form the foundational identity primitive of the Agentic Provenance Protocol and serve as the basis for trust, ownership, provenance, authorization, and federation.
