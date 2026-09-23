# Sapiocracy — governance research specification

Status: design hypothesis

## 1. Definition

In this repository, **sapiocracy** means routing a decision toward people with demonstrated expertise relevant to the specific question.

It does not mean a permanent class of experts governs every domain. Expertise is contextual, and expert input is only one component of legitimacy.

## 2. Decision record

A public decision should be represented as a versioned record containing:

```text
Decision {
  question
  scope
  affected_parties
  rights_constraints
  evidence
  uncertainty
  expert_requirements
  selected_experts
  conflicts_of_interest
  public_comments
  options
  impact_model
  decision
  minority_views
  implementation
  metrics
  review_date
  appeal_paths
}
```

## 3. Expertise signals

Possible signals include:
- demonstrated work relevant to the exact question;
- reproducible or peer-reviewed contributions where applicable;
- professional experience;
- forecasting/calibration record;
- open-source or public artifacts;
- references from independent experts;
- affected-community knowledge;
- recency of expertise.

These signals should be inspectable and contestable rather than converted into one opaque score.

## 4. Independence and conflicts

For consequential decisions, the design should test safeguards such as:
- employer and sponsor diversity;
- conflict disclosure;
- preservation of minority expert views;
- affected-party ability to identify missing expertise;
- separate funding for adversarial review.

## 5. Rights and due process

A technical recommendation does not by itself settle a legal or values dispute.

A proposed decision should therefore have separate checks for:
1. legal authority / jurisdiction;
2. fundamental rights;
3. due process;
4. security and privacy;
5. domain-specific optimization.

## 6. Citizen participation

Open questions include how residents can:
- propose questions;
- submit evidence;
- challenge panel composition;
- comment on alternatives;
- appeal procedure;
- trigger review when measured outcomes diverge from expectations;
- participate in constitutional-level changes.

Voting, sortition, delegation, consent, and other mechanisms should be evaluated rather than assumed interchangeable.

## 7. Rules as software

A rule can have:
- human-readable normative text;
- machine-readable representation;
- executable implementation where appropriate;
- tests and invariants;
- version history;
- rationale and evidence;
- dependency graph;
- review/sunset date.

Software is an audit and implementation mechanism. It has legal force only where the competent legal framework gives it such force.

## 8. Appeals

At minimum, the model should distinguish:
- **fact appeal** — evidence or factual premise is challenged;
- **process appeal** — panel, conflict, or procedure is challenged;
- **rights appeal** — protected rights are implicated.

Appeals should have institutional separation from the original decision maker.

## 9. Emergency powers

Any emergency mechanism should be evaluated for:
- narrow trigger conditions;
- automatic expiration;
- bounded scope;
- auditability;
- independent review;
- multi-party authorization for extraordinary actions.

## 10. Capture metrics

Research metrics may include:
- expert-selection concentration;
- funder/employer concentration;
- repeat-panel concentration;
- conflict-disclosure completeness;
- appeal success rate and latency;
- participation by affected groups;
- calibration error;
- policy rollback rate.

## 11. Questions to test

- Does question-specific expert routing improve decisions on measurable problems?
- How easily can reputation signals be gamed?
- Does the process exclude local or experiential knowledge?
- What happens when expert disagreement reflects values rather than facts?
- How should legitimacy work when evidence is weak?
- How can expertise metrics avoid becoming targets that distort behavior?
