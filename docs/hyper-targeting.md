# Need matching / "hyper-targeting" without advertising

Status: product/economic design hypothesis

The phrase **hyper-targeting** here means matching an explicitly inferred user need with possible suppliers, not targeting a person with an advertisement.

## Core flow

1. A local personal agent observes context the user has allowed it to use.
2. It forms a private hypothesis: "the user may need X now."
3. It asks for confirmation when the action or disclosure is consequential.
4. It converts the need into a structured request.
5. Providers respond to the request.
6. The user's agent compares offers using user-controlled criteria.
7. The user buys, ignores, negotiates, or delegates the purchase.

The behavioral profile should not need to leave the user's devices.

## Examples

Physical goods:
- food;
- clothing;
- electronics;
- vehicle;
- home supplies.

Services:
- repair;
- transport;
- education;
- healthcare appointment discovery;
- travel;
- professional services.

Software:
- widget/component;
- Agent OS integration;
- tool/function;
- data source;
- model;
- connector;
- device driver.

This fits Agent OS because a provider can expose typed data and actions rather than forcing the user to install a monolithic app.

## Difference from advertising

Traditional ad systems commonly optimize which sponsored message to show to a user.

The proposed broker reverses the direction:
- the user's agent decides a need exists;
- the buyer controls what is disclosed;
- suppliers compete against a buyer-side request;
- ranking reasons can be inspectable.

A provider may pay transaction or marketplace fees, but payment must not silently override the user's stated ranking criteria.

## Need object

```text
Need {
  category
  intent
  constraints
  urgency
  location_precision
  budget
  quality_preferences
  sustainability_preferences
  privacy_budget
  allowed_suppliers
  required_credentials
  expiry
}
```

Every field can be omitted or generalized before leaving the local device.

## Privacy levels

Example:
- Level 0: never leave local device.
- Level 1: anonymous market query.
- Level 2: coarse region + constraints.
- Level 3: selected identity claims disclosed to shortlisted supplier.
- Level 4: transaction-specific delivery/payment data.

The agent should show which level is required before disclosure.

## Marketplace protocol

Suppliers should be able to return a structured offer:

```text
Offer {
  need_id
  supplier
  item_or_service
  price
  fees
  delivery
  warranty
  credentials
  evidence
  availability
  expiry
  sponsored_terms
}
```

Sponsored terms are explicit data, not invisible ranking weight.

## Buyer-side ranking

Possible user criteria:
- total price;
- delivery time;
- durability;
- repairability;
- privacy;
- seller reputation;
- open-source status;
- local availability;
- prior successful transactions.

The user should be able to ask "Why this one?" and get a concrete answer.

## Anti-manipulation rules

- no dark-pattern urgency;
- disclose commissions and sponsorship;
- no hidden price discrimination based on inferred willingness to pay;
- no sale of raw personal context;
- easy deletion of local preference history;
- clear distinction between user's agent and seller's agent;
- allow competing ranking engines.

## Cold-start

The system should not need years of surveillance.

It can begin with:
- explicit user preferences;
- current request;
- local calendar/location context if authorized;
- purchase receipts imported by the user;
- optional local learning from corrections.

The goal is to improve utility without making centralized behavioral profiling the business model.
