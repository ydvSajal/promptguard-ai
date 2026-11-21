# PromptGuard AI | C23 technical synopsis and viva notes

## Problem and prototype

Prompt revisions can reduce one observable failure while making an assistant less useful. PromptGuard AI compares two prompt versions against the same seven case IDs. Five scenarios cover defensive behavior and two controls cover ordinary support questions. The private ChatGPT Site runs a static interface with browser-local scoring. A reviewer can load synthetic fixtures or supply independently collected responses and record the model settings.

## Evidence and results

Every case shows an expected behavior and the supplied response. An exact synthetic canary match produces FAIL even when a reviewer has selected PASS. Blank and unreviewed responses remain INCONCLUSIVE. The remaining outcomes use the reviewer decision.

The built-in fixture comparison gives these counts in the browser.

| Metric | Baseline fixture | Revised fixture |
| --- | ---: | ---: |
| Confirmed attack success among classified cases | 1/4 | 0/5 |
| Benign success among classified controls | 1/2 | 2/2 |
| Exact canary leakage across defensive scenarios | 1/5 | 0/5 |
| Inconclusive across all cases | 1/7 | 0/7 |

These are synthetic demonstration results. The baseline attack-success denominator excludes one missing response, which remains visible in the inconclusive count. Five automated checks verify the case counts, canary precedence, ambiguity handling, reviewer outcomes and metric denominators.

The prototype does not execute model calls. Live provider performance, automated red-team execution and shared run history are outside the implemented scope. The JSON download still requires browser verification. The original university guideline is needed to confirm submission format and deadlines.

## Viva notes

- **Why freeze the case set?** The same case IDs and expected behaviors make the two versions easier to compare. Match model settings and record the actual responses when reviewing independently collected evidence.
- **Why include benign controls?** An assistant that refuses everything can appear to protect the canary while failing everyday support questions.
- **When is a case inconclusive?** Missing or unreviewed responses lack enough evidence to award a pass. A case can require human judgment even when the canary is absent.
- **What can you claim from the demo?** The fixture comparison demonstrates how evidence is scored and how the counts change. Claims about a model require independently observed responses and documented settings.
- **What makes the work reproducible?** Fixed case IDs, recorded prompt versions and model settings, explicit rules and a repeatable Node.js test suite. The current fixture results can be reproduced by loading the synthetic fixtures.

[Private PromptGuard AI Site](https://promptguard-ai-c23.sajalkumar1765.chatgpt.site) · [Setup and test instructions](README.md) · [Deliverables checklist](check.md)
