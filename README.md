# veritas-sandbox-runners
Ephemeral sandbox VMs for Véritas agents, via GitHub Actions (`workflow_dispatch` only).
- Public repo = unlimited free standard-runner minutes. Contains **no secrets and no code to protect**: the workflow only decodes caller-supplied input, runs it with caps (48 KB code, 300 s, truncated output) and prints the result between log markers.
- One disposable Ubuntu VM per run. Triggered only through the API with the user's own token (`sandbox_exec` tool, `actions` provider).
