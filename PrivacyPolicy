# Privacy Policy

_Last updated: August 13, 2026_

## 1. Overview

This Privacy Policy explains how MemoryBot collects, uses, stores, shares, and deletes information when used in a Discord server.

MemoryBot is disabled by default. It only processes messages for memory collection in channels where a server administrator has explicitly enabled it with:

```text
/enable [channel]
```

## 2. Information MemoryBot May Process

When enabled in a channel, MemoryBot may process:

- Message content from enabled Discord channels
- Discord user IDs and user mentions
- Discord channel IDs and channel mentions
- Discord server IDs
- Message timestamps and related metadata
- Questions submitted through bot commands such as `/ask`
- Messages that appear to ask about previous server context
- Recent stored memories used for `/catch-me-up`
- User opt-out status from `/ignore_me`

MemoryBot ignores:

- Direct messages
- Messages from bots
- Channels that have not been enabled
- Users who have opted out with `/ignore_me`

Bot commands are server-only and are not available in DMs.

## 3. Information MemoryBot Stores

MemoryBot stores extracted memory summaries and related metadata in a local vector database.

Stored data may include:

- A concise summary of useful server discussion context
- Server IDs
- Channel IDs
- User IDs or user mentions, if available and configured
- Channel mentions, if available
- Timestamps or memory age metadata
- Embeddings used for memory search
- Opt-out records for users who run `/ignore_me`

MemoryBot does not permanently store full raw message transcripts as memories.

Raw messages from enabled channels may be temporarily batched in memory so MemoryBot can extract useful summaries. The long-term stored record is the extracted memory summary and metadata, not the full raw transcript.

## 4. Use of AI Services

MemoryBot may send relevant content to Google Gemini for AI processing.

This may include:

- Batched message content from enabled channels
- Questions submitted through `/ask`
- Messages checked for memory-question detection
- Stored memory summaries used to generate answers
- Recent stored memories used for `/catch-me-up`

Gemini may be used to:

- Extract useful memories from channel discussions
- Generate embeddings for memory search
- Detect whether a message is asking about server memory
- Answer memory-related questions
- Generate recent-topic summaries

The exact behavior may depend on the bot operator's configuration.

## 5. How Information Is Used

MemoryBot uses information to:

- Remember useful server context
- Answer questions about previous discussions
- Summarize recent stored topics
- Detect when someone may be asking about past server context
- Provide memory statistics
- Respect user opt-out choices
- Operate, maintain, and improve bot functionality

MemoryBot does not sell personal information.

## 6. Server Administrator Controls

Server administrators can control where MemoryBot operates.

```text
/enable [channel]
```

Enables memory collection in a channel.

```text
/disable [channel]
```

Disables memory collection in a channel.

```text
/forget confirm:True
```

Deletes all stored memories for the server, clears cached answers, and cancels pending memory batches.

```text
/memory_stats
```

Shows memory statistics for the server.

If a channel is not enabled, MemoryBot does not collect memory from that channel.

## 7. User Controls

Users can opt out of memory collection in a server.

```text
/ignore_me
```

Stops MemoryBot from collecting that user's messages.

```text
/unignore_me
```

Allows MemoryBot to collect that user's messages again in enabled channels.

## 8. Data Retention

By default, MemoryBot keeps stored memories for 90 days.

The bot operator may configure a different retention period. If retention is set to `0`, memories may be kept indefinitely.

MemoryBot runs a cleanup task every 24 hours while online to remove expired memories.

## 9. Data Deletion

Server administrators can delete all stored memories for their server by running:

```text
/forget confirm:True
```

Users who do not want future messages remembered can run:

```text
/ignore_me
```

For additional deletion requests, contact the operator of the MemoryBot instance installed in your server.

## 10. Data Sharing

MemoryBot may share information with:

- Discord, as part of normal Discord bot operation
- Google Gemini, when AI processing is required to provide bot features

MemoryBot does not sell personal information.

## 11. Security

MemoryBot stores memories in a local database controlled by the bot operator.

The bot operator is responsible for protecting:

- The bot hosting environment
- Database files
- Discord bot tokens
- Gemini API keys
- Configuration files and secrets

MemoryBot is designed to reduce long-term storage of raw conversation data by storing extracted summaries instead of full message transcripts.

## 12. Children's Privacy

MemoryBot is intended for use in Discord servers.

Server owners and administrators are responsible for deciding whether MemoryBot is appropriate for their community and for enabling it only in suitable channels.

## 13. Changes to This Policy

This Privacy Policy may be updated when MemoryBot changes.

The latest version should be posted wherever the bot operator hosts the policy.

## 14. Contact

For questions about this Privacy Policy or requests related to stored data, contact the operator of the MemoryBot instance installed in your Discord server or reach out to aboulhassan.rayan@gmail.com.
