# Fayd

Ventures, the stack they run on, and the engineering practice behind both.

## How this organization is laid out

Every repo falls into one class, recorded as the `kind` custom property and mirrored as a topic.

| Class | What it is | Naming |
|---|---|---|
| **venture map** | A venture's legible definition — identity, product map, integrations, decisions. Documents and pointers only, never runtime. | `venture-<name>` |
| **product** | A thing a venture operates or sells. Own repo, own runtime, own lifecycle. | domain-named |
| **stack wrapper** | A pinned upstream component of the composable operating stack, wrapped not forked. | `venture-stack-<component>` |
| **tooling** | Estate tooling that is not a stack component. | domain-named |
| **practice** | How we build. | `engineering` |

Repos also carry `venture` (which venture owns it), `tier` (`E` = executable, so the pre-merge review
gate is mandatory; `P` = prose), and `terminal` (`pr` = pull-request-terminal, `direct` = direct to
main allowed).

## Ventures

| Venture | Shape |
|---|---|
| **DH** | Digital humanities infrastructure for cultural institutions — preservation, digitization, authority control, packaging. |
| **Investigations** | Own-capability OSINT and investigations vertical. Single tenant, confidential by default. |
| **ACH** | Arab Crafts Hub. Being restarted as a venture setup. |

**venture-stack** is estate-level: one dedicated, modern, API-first open-source system per business
function, composed rather than monolithic, and swappable by design.

## Where to start

- A venture's own repo (`venture-*`) is the map — read it before its products.
- `engineering` holds how we build: the loop, the review gate, artifact conventions, and how to
  contribute.
- Work is tracked as issues in the repo that owns the change, viewed in the venture's project board.
