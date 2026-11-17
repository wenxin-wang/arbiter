# arbiter

Static approval page.  A request travels in the URL fragment; the page shows
it, signs SHA-256 of its exact bytes with a passkey, and posts the WebAuthn
assertion to the ntfy topic named in the request.  The host verifies the
signature; this page and ntfy are untrusted transport.

Design and host-side tool: `docs/projects/261116-sudo-tiers/` in
[uraj](https://github.com/wenxin-wang/uraj).
