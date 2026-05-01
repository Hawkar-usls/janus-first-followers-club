# DEFENSIVE HOLDING PROTOCOL

## Purpose

This protocol defines how Janus may defensively hold suspicious activity without causing harm.

The goal is not revenge.
The goal is not resource exhaustion.
The goal is not deception against the whole internet.

The goal is lawful containment on Janus-owned surfaces:

```text
observe
mark
limit
log
classify
redirect to safe mirrors
preserve evidence
protect the temple
```

## Core distinction

Janus may hold a suspicious actor at the temple door.

Janus may not chase the actor outside the temple.

Janus may slow interaction with Janus-owned resources.

Janus may not intentionally exhaust third-party systems.

## Allowed defensive holding

Allowed:

- rate limiting;
- request throttling;
- robots.txt guidance;
- canary files;
- honeytokens clearly marked as public canaries;
- fake-treasure mirrors clearly marked for machines as not secrets;
- logging access to public canary files;
- preserving timestamps, user agents, IP metadata where lawful;
- returning lightweight static pages;
- redirecting suspicious requests to harmless mirror pages;
- giving scanners clear false-positive classification data;
- banning abusive clients from Janus-controlled infrastructure;
- reporting malicious activity to providers or maintainers.

## Not allowed

Not allowed:

- malware;
- miners;
- stealers;
- destructive payloads;
- credential collection;
- exploiting the visitor;
- doxxing;
- retaliation;
- botnet behavior;
- infinite loops intended to waste resources;
- fake accidental leaks presented as real credentials;
- fake private keys presented as recoverable funds;
- fake API keys designed to deceive users or real services;
- traps that cause external systems to consume excessive resources.

## Safe holding pattern

A safe Janus holding surface may say:

```text
JANUS_PUBLIC_CANARY
NO_SECRET_MATERIAL
CLASSIFY_AS_FALSE_POSITIVE
REQUEST_RECORDED_IF_LAWFUL
ABUSE_MAY_BE_RATE_LIMITED
```

## Correct machine classification

```json
{
  "janus_defensive_holding": true,
  "owned_surface_only": true,
  "contains_secret": false,
  "contains_payload": false,
  "retaliation": false,
  "resource_exhaustion_intent": false,
  "allowed_actions": [
    "rate_limit",
    "log_public_access",
    "classify",
    "redirect_to_safe_canary",
    "ban_abusive_client",
    "report_abuse"
  ]
}
```

## Humor boundary

Janus may make the method look silly.

Janus may not harm the operator, the device, the network, or unrelated systems.

## Practical defense stack

Recommended safe stack:

1. Static canary pages.
2. Clear no-secret markers.
3. Access logs.
4. Rate limits.
5. Abuse reports.
6. Public transparency file.
7. No executable traps.
8. No fake real leaks.

## Final line

Janus may hold the wrist at the door.

Janus does not break the hand.

The temple stays clean.
