# Jayesh Suyal

**Python/backend engineering · inference tooling · evaluation reliability**

I build tools that make model-serving runs and product answers inspectable: what was requested, what happened, what evidence supports the result, and where the claim stops. [Portfolio](https://jayeshsuyal.dev/) · [LinkedIn](https://www.linkedin.com/in/jayeshs07)

## Merged upstream: NVIDIA AI Dynamo AIPerf

- [#1434 — Preserve terminal benchmark failures](https://github.com/ai-dynamo/aiperf/pull/1434): fixed missing-record parsing and debug logging so failures reach the controller.
- [#1448 — Count completed requests from phase records](https://github.com/ai-dynamo/aiperf/pull/1448): corrected a case that reported 74 completions for 3 requests; added regression coverage.
- [#1447 — Group MLflow diagnostics under `system/`](https://github.com/ai-dynamo/aiperf/pull/1447): separated system diagnostics from inference metrics with tests and migration guidance.

[Review the merged PRs upstream](https://github.com/ai-dynamo/aiperf/pulls?q=is%3Apr+is%3Amerged+author%3Ajayeshsuyal). As of 9 October 2026, [#1463](https://github.com/ai-dynamo/aiperf/pull/1463) and [#1464](https://github.com/ai-dynamo/aiperf/pull/1464) are **open PRs under review**.

## Selected projects

- [Inferdrome](https://github.com/jayeshsuyal/inferdrome) — Python pipeline for repeatable vLLM/SGLang serving experiments and offline-checkable evidence. Its [A100 baseline](https://github.com/jayeshsuyal/inferdrome/blob/main/evidence/gpu/2026-08-23-qwen3-8b-a100-sxm4/README.md) is a bounded single-GPU result, not a capacity claim.
- [Ablatrix](https://github.com/jayeshsuyal/ablatrix) — evidence-grounded product answers and a reviewer-driven revision loop. The [pinned paid batch](https://github.com/jayeshsuyal/ablatrix/blob/main/docs/evidence/paid-qa-batch-2026-09-28/report.md) records 20/20 completed calls and 52/52 exact citation-quote matches; no answer-quality gain has been established.
- [ExitSpec](https://github.com/jayeshsuyal/ExitSpec) — Python acceptance workbench that freezes a criterion, checks evidence, and returns a scoped verdict. Its [guided example](https://github.com/jayeshsuyal/ExitSpec/blob/main/docs/DEMO_RUNBOOK.md) uses synthetic cases, not a customer benchmark.
