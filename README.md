# AideMemo for Grok Bot

Ask Grok Bot about the memories you choose to share from [AideMemo](https://www.aidememo.com), the
personal memory app for iPhone and iPad: notes, voice transcripts, calendar events, reminders, the
descriptions of your photos, places you went, and your Trakt or Bangumi records if you connect those
accounts in AideMemo and choose to share them. If you allow it, Grok Bot can add notes too.

This repository is the plugin for Cursor's plugin marketplace. It holds no code that runs: a manifest,
the address of AideMemo's connector (`https://mcp.aidememo.com/mcp`), a skill that tells Grok Bot how to
search and cite memories and when to add a note, and the logo.

## How it works

- **You choose what to share:** the kinds of memories, and the period they come from.
- **Your iPhone or iPad answers.** Grok Bot's request goes to AideMemo's relay, which wakes your device
  with a notification. Your device answers from its own copy of what you shared, and the answer goes back
  the same way. The relay keeps no question, answer or note.
- **Three tools.** `search` finds up to 20 memories by words or dates, and `fetch` reads one in full.
  `create_note` adds a new note with the text Grok Bot gives it, only once you turn on Add Notes for Grok
  Bot in AideMemo; it is off until then. Nothing can change or delete a memory you have.
- **You see every access.** Each search, each read and each note added shows a notification, and Recent
  Access in AideMemo lists them.
- Every memory Grok Bot cites comes with a link that opens it in AideMemo.

## Connecting

There is no AideMemo account or password. When you connect AideMemo in Grok Bot, a page opens AideMemo
on your iPhone or iPad, or shows a QR code when you connect from another device. AideMemo shows where the
request came from and what Grok Bot would read, and you allow it there. You can pause the connection,
change what it reads, or delete it in AideMemo at any time.

## What you need

- AideMemo on an iPhone or iPad with iOS 27 or iPadOS 27.
- An AideMemo subscription or its free trial. Without one, AideMemo pauses its assistant connections.
- Notifications allowed for AideMemo. AideMemo asks when you connect.
- Your iPhone or iPad on, online, and unlocked at least once since it last restarted. AideMemo does not
  need to be open.

Health, Motion and email are never offered to an assistant.

## Links

- [AI assistants and AideMemo](https://www.aidememo.com/assistants)
- [Privacy policy](https://www.aidememo.com/privacy) · [Terms of use](https://www.aidememo.com/terms) ·
  [Support](https://www.aidememo.com/support)

AideMemo is published by Proairos Pte. Ltd. This plugin is released under the MIT License.
