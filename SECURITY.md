# Security Policy

## Reporting a vulnerability

**Do not open a public issue for a security vulnerability.**

Use GitHub's private reporting instead:
[**Report a vulnerability**](https://github.com/rsmiller213/epm-workbench-issues/security/advisories/new).
It opens a private thread visible only to you and the maintainers — no mailbox, no
attachment size limits, and the disclosure timeline stays under your control.

Please include the extension version (VS Code → Extensions → EPM Workbench), your VS Code
version and OS, and the smallest reproduction you can manage.

### Scope

In scope: the EPM Workbench VS Code extension, the `epmwb` CLI, the hosted Groovy language
server (`lsp.epmworkbench.com`), and `epmworkbench.com` including the license portal.

Out of scope: Oracle EPM Cloud itself and anything reachable only with credentials you
supplied. Report Oracle-side issues to Oracle.

### Especially interesting to us

- Anything that could expose Oracle credentials held in VS Code SecretStorage, or leak
  them into logs, journals, telemetry, or a webview.
- Anything that lets rule source or dimension data reach the hosted language server when
  the user has not enabled it.
- Seat Key forgery, replay, or cross-tenant entitlement escalation.

## If you already posted something sensitive

If credentials, a Seat Key, or a Pod URL landed in a public issue: **rotate the secret
first**, then report the issue. Deleting a GitHub comment does not remove it from caches,
notification emails, or third-party mirrors — rotation is the only real remedy.
