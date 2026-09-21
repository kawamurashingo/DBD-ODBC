# DBD::ODBC Sustainability Proposal

## Purpose

DBD::ODBC is long-lived infrastructure connecting Perl DBI applications to ODBC-compatible databases. This document proposes exploring a sustainable maintenance model so that the project's continued health does not depend excessively on unpaid work by individual maintainers.

This is a discussion proposal, not a commitment to a particular funding model or budget. Any implementation should be agreed with the existing maintainers and DBI community.

## Goals

- Understand the current maintenance workload, governance, and project risks.
- Identify organizations that depend on DBD::ODBC in production.
- Improve continuity by reducing the project's bus factor.
- Maintain useful CI and compatibility testing across supported Perl, OS, driver-manager, and database combinations.
- Explore transparent recurring funding for maintenance work.
- Keep technical decisions independent from the size of individual sponsorships.

## Proposed first-year pilot

As a starting point for discussion, a pilot could target approximately **JPY 8,000,000 per year** (or an appropriate equivalent in another currency).

An illustrative allocation:

| Area | Annual budget |
| --- | ---: |
| Maintainer work | JPY 5,000,000 |
| Secondary maintainer / review | JPY 1,000,000 |
| CI and compatibility infrastructure | JPY 1,000,000 |
| Emergency work / contingency | JPY 1,000,000 |
| **Total** | **JPY 8,000,000** |

These figures are deliberately provisional. The real budget should be derived from maintainer input and measured maintenance needs.

## Suggested workstreams

1. Confirm maintainer interest and governance principles.
2. Document current maintenance workload and project risks.
3. Define a supported compatibility / CI matrix.
4. Estimate a sustainable annual maintenance budget.
5. Evaluate fiscal-hosting and funding options.
6. Define sponsorship policy and contribution tiers.
7. Find organizations willing to identify themselves as production users.
8. Prepare concise sustainability and sponsorship documentation.
9. Recruit a small number of initial anchor sponsors.
10. Publish transparent periodic maintenance and financial reports.
11. Review the experiment after 12 months.

Each workstream can be tracked as a separate GitHub issue if the maintainers want to proceed.

## Principles

### Funding supports project health, not control

Financial contributions should not purchase authority over technical decisions. Technical governance should remain with the project and its maintainers.

### Keep commercial obligations separate

General maintenance funding should support work such as:

- bug fixes and regression prevention;
- compatibility with supported Perl versions;
- ODBC driver and driver-manager compatibility;
- CI and test infrastructure;
- release work;
- documentation;
- review capacity; and
- continuity of maintenance.

Guaranteed response times, private support, or sponsor-specific feature development should be handled separately if they are offered at all.

### Transparency

If project funding is accepted, income, material expenses, and the broad allocation of maintenance funding should be visible to the community. A fiscal host may be preferable to asking an individual maintainer to receive and administer project funds personally.

### Avoid a single point of failure

A successful sustainability effort should make it easier for at least two people to understand and maintain critical areas of DBD::ODBC.

## Possible sponsor structure

For discussion only, a tiered model could make participation possible for organizations of different sizes:

| Tier | Illustrative annual contribution |
| --- | ---: |
| Supporter | JPY 100,000 |
| Business | JPY 500,000 |
| Critical | JPY 1,500,000 |
| Anchor | JPY 3,000,000 |

The tiers should primarily recognize support for shared maintenance capacity. They should not grant proportionally greater technical control.

## Pilot success criteria

After an initial 12-month period, useful indicators could include:

- at least two people able to maintain critical parts of the project;
- documented maintenance and release responsibilities;
- a reproducible compatibility / CI matrix;
- transparent finances if funding is accepted;
- recurring support from multiple independent organizations;
- measurable maintenance output such as releases, regression tests, compatibility fixes, and documentation; and
- reduced reliance on unpaid emergency work.

## Open questions

Before any fundraising begins, the project should discuss:

- Do the current maintainers want a funding initiative?
- What work would actually benefit most from funding?
- Who should approve expenditures?
- What fiscal or organizational host, if any, is appropriate?
- How should paid maintenance work be selected and reviewed?
- How should conflicts of interest be handled?
- Which compatibility targets matter most to current users?
- How can production users identify themselves without disclosing sensitive infrastructure details?

## Next step

If there is maintainer interest, the smallest useful next step is to open a tracking issue and split the workstreams above into individual issues. The first issue should focus on maintainer interest and governance rather than fundraising.
