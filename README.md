# Jayesh Suyal

I work on inference systems—and the failures their benchmarks can hide.

Verification engineer · Founder, InferenceAtlas

## Fixed upstream

Three merged contributions to [NVIDIA AI Dynamo's AIPerf](https://github.com/ai-dynamo/aiperf).

<details open>
<summary><strong>Three requests. Seventy-four reported completions.</strong></summary>

The counter was counting metric summaries instead of requests. I corrected the accounting and added regression tests for failures, cancellation, and warmup exclusion.

`completed_requests: 74 → 3` · [Read the fix · #1448 ↗](https://github.com/ai-dynamo/aiperf/pull/1448)

</details>

<details>
<summary><strong>The benchmark failed. The controller kept waiting.</strong></summary>

A terminal result with missing records was rejected during message parsing. I fixed the serialization boundary and a debug-logging failure, with regression coverage for failure propagation, cancellation, and shutdown.

[Read the fix · #1434 ↗](https://github.com/ai-dynamo/aiperf/pull/1434)

</details>

<details>
<summary><strong>System diagnostics were mixed with inference metrics.</strong></summary>

I grouped MLflow diagnostic and hardware metrics under `system/`, preserving inference metric names and adding regression tests and migration guidance.

[Read the change · #1447 ↗](https://github.com/ai-dynamo/aiperf/pull/1447)

</details>

## Open the work

**[inferdrome](https://github.com/jayeshsuyal/inferdrome)**  
[Run the synthetic local demo](https://github.com/jayeshsuyal/inferdrome/blob/main/docs/LOCAL_DEMO.md) · [Inspect the evidence-bundle design](https://github.com/jayeshsuyal/inferdrome/blob/main/docs/EVIDENCE_BUNDLE_V1.md)

**[ablatrix](https://github.com/jayeshsuyal/ablatrix)**  
[Inspect the 20-product evaluation](https://github.com/jayeshsuyal/ablatrix/blob/main/docs/evidence/paid-qa-batch-2026-09-28/report.md) · [Read the search ablation](https://github.com/jayeshsuyal/ablatrix/blob/main/docs/search-ablation.md)

**[inferenceatlas-agent-demo](https://github.com/jayeshsuyal/inferenceatlas-agent-demo)** · historical hackathon demo  
[Run the public demo](https://github.com/jayeshsuyal/inferenceatlas-agent-demo#try-it-in-60-seconds) · [Read the packet contract](https://github.com/jayeshsuyal/inferenceatlas-agent-demo/blob/main/docs/CONTRACT.md)

---

Earlier: [neural accelerator verification](https://github.com/jayeshsuyal/2-neural-accelerator) · [RISC-V / UVM](https://github.com/jayeshsuyal/RISCV_Verification)  
The story outside the code → [jayeshsuyal.dev](https://jayeshsuyal.dev/)
