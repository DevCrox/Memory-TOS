# Terms of Service

_Last updated: August 13, 2026_

## 1. Acceptance

By inviting, enabling, or using MemoryBot in a Discord server, you agree to these Terms of Service.

If you do not agree, do not use MemoryBot and remove it from your server.

## 2. Description of Service

MemoryBot is a Discord bot that helps servers remember useful context from opted-in channels.

MemoryBot may:

- Read messages in enabled Discord channels
- Temporarily batch messages for memory extraction
- Store extracted memory summaries and metadata
- Answer questions about stored server memory
- Summarize recent remembered topics
- Detect when a user appears to be asking about previous server context

MemoryBot is disabled by default and only begins memory collection after a server administrator enables it in a channel.

## 3. Server Administrator Responsibilities

Server administrators are responsible for:

- Deciding whether MemoryBot is appropriate for their server
- Enabling MemoryBot only in suitable channels
- Informing server members that MemoryBot may process messages in enabled channels
- Managing user concerns, deletion requests, and configuration choices
- Protecting any bot credentials, API keys, database files, or hosting environment under their control

Administrators can use:

```text
/enable [channel]
/disable [channel]
/forget confirm:True
/memory_stats
```

## 4. User Controls

Users may opt out of memory collection in a server by running:

```text
/ignore_me
```

Users may opt back in by running:

```text
/unignore_me
```

## 5. Acceptable Use

You agree not to use MemoryBot to:

- Violate Discord's Terms of Service or Community Guidelines
- Collect, process, or expose information unlawfully
- Harass, abuse, threaten, or target other people
- Store highly sensitive information without appropriate consent
- Attempt to bypass bot permissions, rate limits, or security controls
- Reverse engineer, attack, overload, or disrupt the bot or its hosting environment

## 6. AI-Generated Output

MemoryBot uses AI services to summarize discussions and answer questions from stored memories.

AI-generated responses may be incomplete, incorrect, or outdated. You should not rely on MemoryBot for legal, medical, financial, safety-critical, or emergency decisions.

## 7. Data and Privacy

MemoryBot's data practices are described in the Privacy Policy.

By using MemoryBot, you understand that enabled-channel messages may be temporarily processed and may be sent to AI services such as Google Gemini to provide bot features.

## 8. Availability

MemoryBot may be unavailable, delayed, rate-limited, changed, or discontinued at any time.

No guarantee is made that MemoryBot will always respond, remember every useful detail, or preserve stored memories indefinitely.

## 9. No Warranty

MemoryBot is provided "as is" and "as available," without warranties of any kind.

To the maximum extent permitted by law, the bot operator disclaims all warranties, express or implied, including warranties of reliability, fitness for a particular purpose, accuracy, and non-infringement.

## 10. Limitation of Liability

To the maximum extent permitted by law, the bot operator is not liable for any indirect, incidental, special, consequential, or punitive damages, or for loss of data, profits, reputation, server activity, or access arising from use of MemoryBot.

## 11. Removal

A server administrator may stop using MemoryBot by disabling it in channels or removing it from the server.

Stored server memories may be deleted with:

```text
/forget confirm:True
```

## 12. Changes to These Terms

These Terms may be updated from time to time. Continued use of MemoryBot after changes means you accept the updated Terms.

## 13. Contact

For questions about these Terms, contact the operator of the MemoryBot instance installed in your Discord server or reach out to aboulhassan.rayan@gmail.com.
