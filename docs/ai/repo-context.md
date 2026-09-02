# Repository AI Context — PCR Readiness reference

Status: repository-local AI context. Engineer-standard remains the cross-repository engineering authority.

## Repository identity

- Repository: `TrueCrew1/PCR-Readiness`
- Product/role: Reference/readiness artifact retained for evaluation, not an active True Crew product.
- Lifecycle: reference
- Canonical True Crew agent runtime: Node `24.19.0`

## Ownership

**Owns:** Only the retained PCR readiness artifact and explicitly authorized reference maintenance.

**Does not own:** Customer-product workflow state, company compliance authority, or production application runtime.

## Data/runtime boundary

No database authority.

## Deployment boundary

Reference-only by default; no production deployment or product expansion without reclassification.

## AI execution contract

1. Material mutation requires a current claimed Engineering Task Packet from True Crew HQ. If direct Notion access is unavailable, a trusted orchestrator must provide a current Notion-derived packet snapshot before work starts.
2. Set `TRUECREW_TASK_PACKET` to the current packet identity and run `node scripts/ai-preflight.mjs` from the intended isolated worktree before material mutation.
3. Treat a missing task packet or `BLOCKED` result as a stop condition. Never reset/stash/clean/rebase/discard unexpected state or substitute raw chat/model memory to make preflight pass.
4. When the packet supplies branch/base expectations, set `TRUECREW_EXPECTED_BRANCH` and `TRUECREW_EXPECTED_HEAD` before preflight and reconcile the generated runtime context with the packet.
5. `--allow-dirty` and `--allow-production-branch` are read-only/recovery snapshot controls only; they never authorize mutation.
6. Reference/experimental lifecycle is a real constraint: do not expand a reference or experiment into a product/runtime without explicit portfolio reclassification.
7. Baseline validation: Minimal artifact integrity review unless explicitly reclassified.

## Durable documents to load when applicable

- No additional repository-local governance document is currently canonical beyond `AGENTS.md` and this context.

## Cross-system rule

Provider and customer-product records remain owned by their source systems. Reference code never gains True Crew production authority merely because it is stored in a True Crew repository.
