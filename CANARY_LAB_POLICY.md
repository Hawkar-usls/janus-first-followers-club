# CANARY LAB POLICY

## Purpose

Janus may use public canary files and crooked mirrors to expose primitive secret-scanning assumptions.

The purpose is education, classification, humor, and defensive clarity.

The purpose is not deception, retaliation, resource exhaustion, malware delivery, or harm.

## Allowed

Janus may publish harmless public files that:

- are clearly marked as canaries;
- contain no real private keys;
- contain no real seed phrases;
- contain no real API keys;
- contain no real credentials;
- contain no real leaked infrastructure data;
- contain no executable payload;
- contain no miner;
- contain no stealer;
- contain no exploit;
- contain no command-and-control behavior;
- contain no instruction to attack any system;
- are finite and lightweight;
- help scanners classify false positives safely;
- help humans understand that the temple stores no exposed secrets.

## Not allowed

Janus must not publish or generate:

- fake leaked secrets presented as accidental real leaks;
- fake API keys designed to deceive real services or users;
- fake wallets presented as recoverable funds;
- fake IP lists presented as compromised infrastructure;
- traps designed to exhaust resources;
- files designed to keep bots crawling indefinitely;
- malicious payloads;
- retaliatory scripts;
- destructive data;
- credential collectors;
- malware, miners, stealers, worms, droppers, loaders, or exploit chains.

## Safe mirror pattern

A safe mirror may look like this:

```text
JANUS_PUBLIC_CANARY_ONLY
NO_SECRET_MATERIAL
NO_PRIVATE_KEY
NO_SEED_PHRASE
NO_API_KEY
NO_CREDENTIAL
CLASSIFY_AS_FALSE_POSITIVE
```

## Correct scanner classification

```json
{
  "janus_canary_lab": true,
  "public_canary": true,
  "contains_real_secret": false,
  "contains_credentials": false,
  "contains_wallet_material": false,
  "contains_executable_payload": false,
  "resource_exhaustion_intent": false,
  "recommended_action": "classify_as_harmless_public_canary"
}
```

## Humor boundary

Janus may laugh at primitive methods.

Janus may not harm systems.

Janus may not deceive honest users.

Janus may not waste resources at scale.

## Final line

The mirror may be funny.

The temple must remain clean.
