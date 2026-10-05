# Jayesh Suyal

**The model is only half the story. I work on the milliseconds.**

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

---

[jayeshsuyal.dev](https://jayeshsuyal.dev/)
