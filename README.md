# Smail

The mail client that makes you :)

A modern, lightweight client for [SMXP](https://github.com/orielhaim/SMXP) built to be fast, clean, and actually pleasant to use. No legacy baggage. Just messaging that works the way it should in 2025.

Built with [TanStack Start](https://tanstack.com/start) and powered by the [@smxp/sdk](https://github.com/orielhaim/SMXP-JS)

## Why smail

Anyone can build a client on top of SMXP - that's the whole point. This one's mine. It's opinionated, minimal, and designed around the idea that a messaging client should get out of your way and let you communicate.

The name? Say it out loud. You're welcome.

## What you get

### Real-time streaming

Messages appear the instant they arrive. No refresh button. No "check for new mail." smail holds a persistent SSE connection to your server and renders incoming messages live. You see them as they happen - edits, deletes, receipts, everything.

### Native conversations

SMXP treats conversations as a first-class concept, and so does smail. Threads aren't reconstructed from vague header heuristics - they're real. Clean, ordered, always correct. Reply to a specific message and it just works.

### Edit & delete

Sent something wrong? Fix it. Regret something? Remove it. smail surfaces SMXP's edit and delete capabilities as natural actions.

### Rich content rendering

Every message declares what it is - plain text, markdown, or HTML. smail renders each one properly without guessing. Markdown is a first-class citizen, which means formatted messages without the security circus of arbitrary HTML.

### Message expiration

Temporary messages (OTPs, invites, time-sensitive info) are displayed with awareness of their shelf life. Expired messages are dimmed or hidden based on the sender's intent.

### Delegation

Send on behalf of others, read inboxes you've been granted access to, manage accounts you're responsible for - all without switching credentials or juggling API keys. smail handles delegation natively because SMXP makes it trivial.

### Cryptographic verification

Every message in SMXP is signed with post-quantum cryptography (ML-DSA-65). smail shows you verification status on every single message. Spoofing isn't "hard to detect" - it's impossible at the protocol level. The green checkmark actually means something here.

### Keyboard-first

Navigate, compose, reply, archive - all without touching your mouse. A messaging client you can fly through at the speed of thought.

## Getting started

```bash
git clone https://github.com/orielhaim/smail.git
cd smail
bun install
bun dev
```

Configure your SMXP server connection and credentials, and you're in.

## Status

Under active development. The protocol and the sdk is in alpha, and the client is being built to match. If something's broken - it's probably because I pushed at 3am. Give it an hour.

## License

[Apache 2.0](LICENSE)
