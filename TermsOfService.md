# Privacy Policy for MemoryBot

_Last updated: August 13, 2026_

MemoryBot is a Discord bot that helps servers remember useful context from opted-in channels. This Privacy Policy explains what information MemoryBot processes, what it stores, and what server members and administrators can do to control it.

## Summary

MemoryBot is disabled by default in every server and every channel. It only begins processing messages after a server administrator enables memory collection for a channel with `/enable`.

MemoryBot does **not** store raw Discord message text as permanent memory. Instead, it temporarily batches messages from enabled channels, sends those batches to Gemini for memory extraction, and stores only extracted summaries plus related metadata in a local vector database.

## Information MemoryBot Processes

When MemoryBot is enabled in a Discord channel, it may process:

- Message content from enabled channels
- Discord user mention tokens and user IDs, when available
- Discord channel mention tokens and channel IDs, when available
- Server IDs and channel IDs
- Timestamps or memory age metadata
- Questions submitted through `/ask`
- Messages that appear to be asking about prior server context, for trigger detection
- Command usage needed to operate bot features

MemoryBot ignores:

- Direct messages
- Messages from bots
- Channels that have not been enabled
- Users who have opted out with `/ignore_me`

Bot commands are only available inside Discord servers and are disabled in DMs.

## What MemoryBot Stores

MemoryBot stores extracted memory summaries and metadata in a local ChromaDB vector database.

Stored data may include:

- A concise summary of useful discussion context
- Server and channel metadata
- User or channel references, where available
- Embeddings used for similarity search
- Opt-out records for users who run `/ignore_me`

MemoryBot does **not** permanently store full raw message transcripts as memories.

Raw channel message batches are held temporarily in memory during the batching window so MemoryBot can extract useful memories. After processing, the durable stored record is the extracted summary and metadata, not the original raw transcript.

## Use of Gemini

MemoryBot uses Google Gemini for several AI features, including:

- Extracting durable memories from enabled-channel message batches
- Creating embeddings for stored memories, if configured to use Gemini embeddings
- Confirming whether a message appears to be asking a memory-related question
- Generating answers for `/ask` and proactive memory responses
- Generating `/catch-me-up` summaries

This means message batches, questions, and some triggering messages may be sent to Gemini for processing.

If MemoryBot is configured for local embeddings, embeddings can be generated locally instead. However, Gemini may still be used for memory extraction, trigger confirmation, and answer generation unless the bot operator changes that behavior.

## How MemoryBot Uses Stored Memories

MemoryBot uses stored memories to:

- Answer server memory questions through `/ask`
- Proactively respond when users appear to ask about previous context
- Generate recent-topic summaries with `/catch-me-up`
- Show memory statistics with `/memory_stats`
- Help server members recover previous decisions, plans, and discussion context

MemoryBot is designed to answer using retrieved stored memories, not by exposing raw message logs.

## Retention

By default, MemoryBot keeps stored memories for **90 days**.

The retention period is controlled by the bot configuration value:

MemoryBot runs a cleanup task every 24 hours while online to remove expired memories.

## Data Deletion

Server administrators can delete all stored memories for their server by running:

```text
/forget confirm:True
```
This deletes stored memories, clears cached answers, and cancels pending memory batches for that server.
Users who do not want future messages remembered can run:
```/ignore_me```

## Data Sharing

MemoryBot may share information with:
- Discord, as part of normal bot operation
- Google Gemini, when AI processing is required
MemoryBot does not sell personal information.

## Security

MemoryBot stores memories in a local database controlled by the bot operator. The bot operator is responsible for protecting the bot host, database files, Discord token, Gemini API key, and other configuration secrets.
MemoryBot is designed to reduce long-term storage of raw conversation data by storing extracted summaries instead of full message transcripts.

## Children’s Privacy

MemoryBot is intended for use in Discord servers. Server owners and administrators are responsible for deciding whether the bot is appropriate for their community and for enabling it only in suitable channels.

## Changes to This Policy

This Privacy Policy may be updated when MemoryBot changes. The latest version should be posted wherever the bot operator hosts the policy.

## Contact

For questions about this Privacy Policy or requests related to stored data, contact the operator of the MemoryBot instance installed in your Discord server or reach out to aboulhassan.rayan@gmail.com

