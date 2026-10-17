# Moonshadow Developer Forge (proposal)

Owner: Connectivity and Developer Infrastructure. Amber coordinates construction.

Goal: equip one AI builder with a real sandbox workspace, Git repository, browser editor, CLI, tests and reviewable change workflow.

Reuse candidates, not installed:
- Forgejo: self-hosted Git hosting, pull requests and APIs. https://forgejo.org/docs/latest/
- code-server: browser editor and terminal. https://coder.com/docs/code-server

Acceptance test:
1. Provision an isolated workspace and disposable test repository.
2. Grant worker least-privilege access.
3. Clone repo, edit a test file, run a real test and record exit status.
4. Submit a reviewable change, without direct protected-main write.
5. Verify diff, evidence and rollback.
6. Record results and owner in Board Log.

Security: secrets in approved vault only; no secrets in commits/chat/logs. Authenticate and encrypt browser IDE access. Isolate commands, files and network. Josh approves spending, public publishing and destructive operations.

Interfaces to coordinate:
- Amber: workspace identity, permissions and assignments.
- Codex: worker tool catalog and job contracts.
- Ellie: consuming reviewed outputs in Studio Go.
- This department: MCP/API/CLI handshakes and diagnostics.

Status: DESIGN ONLY. No live deployment or handshake proven.

Next: inspect existing city architecture and agree hosting before deployment.