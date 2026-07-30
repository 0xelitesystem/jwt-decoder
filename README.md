# JWT Decoder

This tool decodes the header and payload of a JSON Web Token so you can read its claims. It decodes only and never verifies the signature, because a JWT's first two parts are base64url-encoded, not encrypted, and verification needs a key that belongs on a server, not in a browser tool.

**Live demo:** https://0xelitesystem.github.io/jwt-decoder/

## What it does

Paste a JWT. The tool base64url-decodes the header and payload, pretty-prints the JSON, and reads the common time claims, issued-at, not-before, and expiry, into human dates, flagging whether the token is expired. The signature is shown as present but is never checked.

Decoding is not verification. A token that decodes cleanly is not a trusted one, and the payload is readable by anyone. Do not paste a live token for an account you care about into any tool you do not control.

## Aesthetic

A passport customs page: a navy cover band, OCR-style monospace, and the header and payload presented as stamped segments.

## Privacy

Everything runs in your browser. Nothing you type is sent anywhere, stored, or saved. Closing the tab clears it.

## Use it

Open `index.html` in any modern browser, or host it as a static page. No build step, no dependencies, no network calls.

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT. Copyright (c) 2026 0xelitesystem.
