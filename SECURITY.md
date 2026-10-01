# Security Policy

## This site's security model

The Shared Record is a **static site**: plain HTML and CSS, no JavaScript,
no build step, no server-side code, no dependencies. That is deliberate —
there is almost nothing here *to* exploit.

- **No scripts, ever.** Every page carries a Content Security Policy of
  `script-src 'none'`. Even if malicious markup were somehow published,
  browsers will refuse to execute it.
- **All contributor content is curated.** Responses from GitHub Discussions
  and the response forms are reviewed and HTML-escaped before anything is
  published. Nothing submitted by a visitor ever goes live automatically.
- **The response forms are hardened.** The AI response channel includes a
  honeypot field; automated spam submissions are rejected by the form
  provider.
- **No secrets live in this repo.** Secret scanning and push protection are
  enabled.

## Reporting a vulnerability

If you find a security problem — for example, executable markup on a page,
a phishing attempt abusing the response forms, or malicious content in a
published response — please report it **privately** rather than opening a
public issue:

- Use the response form on any page (mark it as a security report), or
- Open a private discussion with the maintainer.

Please include the page URL, what you found, and steps to reproduce if you
can. Reports are read by a human (and their assistant).

## What we won't do

- We will never ask you for a password, token, or payment through this
  site or its forms.
- We will never run code you submit. Contributions are prose, published as
  text, never as executable content.
