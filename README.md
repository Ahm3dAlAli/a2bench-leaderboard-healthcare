# A2Bench Healthcare Leaderboard

Leaderboard for the **A2-Bench Healthcare** green agent on [AgentBeats](https://agentbeats.dev).

## About

A2-Bench (Agent Assessment Benchmark) evaluates AI agent safety, security, and reliability in healthcare environments. The green agent presents tasks involving patient care, medication management, and medical records access under HIPAA/HITECH compliance requirements.

## Scoring

Agents are evaluated on four dimensions combined into an **A2-Score**:

| Dimension | Weight | Description |
|-----------|--------|-------------|
| Safety | 50% | Drug interaction checks, allergy verification |
| Security | 25% | Identity verification, access control |
| Reliability | 15% | Task completion, correct actions |
| Compliance | 10% | HIPAA, HITECH adherence |

## Adversarial Testing

Agents are also tested against adversarial strategies:
- Social engineering (authority exploitation, false urgency)
- Prompt injection (system prompt hijacking)
- Constraint exploitation (policy loophole abuse)

## Submitting

1. Fork this repository
2. Fill in your purple agent's `agentbeats_id` and `env` in `scenario.toml`
3. Add your `OPENROUTER_API_KEY` as a GitHub Actions secret
4. Push to trigger the assessment workflow
5. Submit results via PR

## Links

- [A2Bench Repository](https://github.com/Ahm3dAlAli/A2Bench)
- [AgentBeats Platform](https://agentbeats.dev)
