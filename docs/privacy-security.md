# Privacy and security architecture

Updated: 2026-09-23

The design goal is data minimization: a service should learn only what it needs for a specific action.

## Principles

- local-first state;
- end-to-end encryption;
- peer-to-peer transfer where practical;
- explicit capabilities instead of ambient access;
- selective disclosure;
- pairwise identifiers where possible;
- user-held keys with recovery;
- open protocols and portable implementations;
- no requirement for behavioral advertising.

## Identity layers

Keep separate records for:
- device ownership;
- membership credential;
- legal-identity claims when required;
- age or eligibility claims;
- public pseudonyms;
- reputation;
- payment identifiers.

A verifier should receive the minimum claim necessary for the transaction.

## Selective disclosure research

Candidate standards and techniques:
- W3C Verifiable Credentials;
- pairwise identifiers;
- selective-disclosure signatures;
- zero-knowledge proofs for simple predicates;
- hardware-backed keys.

No cryptographic primitive is fixed until interoperability and implementation reviews are complete.

## Recovery

Loss of one AGENT device must not mean loss of identity.

Recovery mechanisms to test:
- multiple personal hardware keys;
- threshold recovery across trusted devices/contacts;
- encrypted offline recovery package;
- optional time-delayed recovery with a revocation window.

## AGENT boundary

The wrist computer may host a Passport wallet, but:
- UWB discovery should be explicit;
- wireless identifiers should rotate where practical;
- camera and microphone capture states should be clear;
- Telekinesis biosignals should be processed locally by default;
- raw biosignal retention should default to off.

## Threat model

Include:
- stolen device;
- compromised merchant or service;
- compromised relay;
- malicious software update;
- supply-chain compromise;
- correlation by network observers;
- credential impersonation;
- lost recovery material;
- coercive access to an unlocked device.

## Evidence

The UN digital-cooperation roadmap emphasizes privacy, agency, consent, and safeguards around digital identity:
https://www.un.org/en/content/digital-cooperation-roadmap/

The UN Global Digital Compact discusses safe, secure, interoperable digital infrastructure and human-rights safeguards:
https://www.un.org/pact-for-the-future/en/annex-i-global-digital-compact
