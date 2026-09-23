# Passport and residency

Status: concept

## Passport is a portable credential, not a device lock-in

A Sapio Passport is a cryptographic residency/membership credential.

It may be stored on:
- AGENT;
- a phone or laptop;
- a hardware key;
- another compatible wallet.

Losing AGENT must not mean losing residency or identity.

## Credential layers

A Passport wallet may hold separate verifiable claims such as:
- resident/member status;
- date of membership;
- eligibility for a programme;
- age-over-threshold proof;
- professional credential;
- role/capability in a project;
- payment/reimbursement entitlement.

The verifier should receive only the claims needed for the action.

## AGENT bundle

The proposal is that accepted early residents can receive a base AGENT device through a waitlist programme.

That distribution plan should be separated from legal identity:
- hardware can be replaced;
- users can bring compatible devices;
- credentials are exportable;
- a resident can remain a resident without wearing AGENT.

Optional rings, glasses, camera modules, dive hardware, larger batteries, and specialist sensors can be commercial accessories.

## Enrollment

A future enrollment flow needs separate answers for:
- uniqueness / sybil resistance;
- legal identity, if required for a particular service;
- pseudonymous participation;
- key generation;
- recovery setup;
- terms/consent;
- initial token allocation, if adopted.

The most privacy-preserving proof should be used for each purpose rather than requiring maximal identity for every service.

## Recovery and revocation

Required properties:
- lost-device revocation;
- multiple-device credentials;
- offline recovery;
- optional trusted-contact threshold recovery;
- rotation of keys without changing the resident's history;
- transparent log of credential issuance/revocation without publishing private profile data.

## Physical Passport

A future physical card/booklet could be useful as an offline recovery and visual identity artifact.

It should not resemble or claim the legal status of an internationally accepted travel document unless relevant authorities actually recognize it.

## Interoperability

The credential format should target open standards rather than an AGENT-only proprietary format.

Candidate standards to evaluate:
- W3C Verifiable Credentials;
- ISO mobile-document standards where appropriate;
- passkeys / WebAuthn for authentication;
- selective-disclosure credential formats.

The exact stack remains an engineering decision pending threat-model and interoperability tests.
