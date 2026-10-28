---
name: meeting-notes
description: Turn raw, messy meeting notes or transcripts into a structured summary with decisions, action items (owner + due date), and open questions. Use when the user pastes meeting notes, a call transcript, or asks to "summarize this meeting".
---

# Meeting Notes

When the user provides meeting notes or a transcript:

1. Read the whole input before writing anything.
2. Fill in the structure from `template.md` (in this skill's folder). Always use the same sections in the same order. Leave out an empty section only if the template says it is optional.
3. Follow the rules below.
4. Before replying, run the final check.
5. End by asking whether they want it as an email draft. If yes, use the subject "Draft Minutes – [Meeting name], [Date]" and ask readers to send corrections by a stated deadline (write "[deadline]" if the user hasn't given one).

## Rules

### Outcomes, not a transcript
- Capture decisions, action items and key points. Synthesize; don't copy the notes line by line.
- Include side discussions only if they led to a decision or action.
- Long enough that someone absent can follow what happened, short enough that decisions aren't buried. Summary: 3 sentences max.
- Refer to an earlier meeting by its date ("as agreed on 3 Oct") instead of repeating its history. If the date isn't given, write "a previous meeting".

### Decisions
- Only list something as a decision if it was actually agreed, not just discussed.
- State each decision explicitly and precisely, including figures, dates and amounts. Add the reason in a few words if it is given.
- Never write "Discussed X" as an outcome. If a topic ended without agreement, it goes under **Open questions**.

### Formal meetings (apply only if the notes mention these)
- **Motions and votes:** for each motion, record the mover, the seconder, the voting method (voice, roll call, show of hands), the count and the result ("The motion carried 5–2."). Record "no" votes and abstentions, including conflicts of interest. Give a reason for a "no" vote or an abstention only if it was stated. Also record motions that failed, were tabled or withdrawn, were amended, or failed for lack of a seconder. Any detail the notes don't give is **not stated**, never guessed.
- **Previous minutes and quorum:** record whether the previous minutes were approved (with any corrections and the mover/seconder) and whether a quorum was present. Record this in the header only, not under **Motions and votes**.
- **Confidential or closed sessions:** record only that the session took place, its start and end times, who attended and any vote result. Leave out what was discussed.
- An action item that comes from a closed session is still listed, but described only by what the vote approved ("Send the formal warning letter approved in closed session"). Leave out names, reasons and other details from the session.

### Action items
- Every action item must have an owner and a due date.
- If no owner is stated, write **Owner: TBD**. If no due date is stated, write **Due: TBD**. Never invent names or dates.
- Start each task with a verb and make it specific ("Send revised budget to finance", not "Budget stuff").
- If the notes don't say what the task is (e.g. "sarah: KPI dashboard"), use a neutral verb ("Follow up on the KPI dashboard") rather than guessing ("Build", "Deliver"). Add the unclear point to **Open questions**.
- If an owner is only implied (a name next to an item, no clear "will do"), write the name followed by "(to confirm)".
- If the notes say "I" or "me", write **Note author** in the language of the notes (e.g. "Συντάκτης σημειώσεων"). Use the author's real name only if the notes give it.
- Keep due dates as written ("Friday", "next week"). If the meeting date is known, add the calendar date in brackets: "Friday (7 Nov)". Never work out a calendar date without a known meeting date.
- A meeting date counts as known only if the day, month and year are all given. If any part is missing (e.g. "3/11" with no year), keep relative dates as written, add no calendar date, and list the missing part under **Open questions**.
- Items carried over from an earlier meeting go under **Carried-over items** with their status (done, pending, blocked). An item counts as carried over if the notes say it was raised, promised or assigned before ("from Sept mtg", "last time", "still waiting", "again"). Otherwise treat it as new. If unsure, list it as new and ask under **Open questions**. If a deadline moved, give both the old and the new date. Record any blocker flagged, and who flagged it.
- Anything someone has to do is an action item, even with Owner: TBD. Don't repeat action items under **Next steps**.
- If the meeting produced no decisions and no action items, say so at the top of the summary.

### Accuracy (never invent)
- Use only what is in the notes. Don't add facts, names, figures or conclusions.
- Name a person only for decisions, action owners, disputed points and reports or presentations. For a report, name the presenter, or their role if the notes give one ("The treasurer reported…"). Otherwise write "the group" or "the team". If it is unclear who said something, don't guess.
- If a name's spelling is uncertain (e.g. "Jeff? Geoff?"), use the spelling the notes lean towards, or the first one given, consistently throughout. Add "(spelling to confirm)" at its first mention and list the alternatives under **Open questions**.
- If something is unclear, contradictory or incomplete, don't guess. Put it under **Open questions / to confirm**.
- Record who chaired and when the meeting started and ended, if the notes say so. Write relative times as given ("started 10 min late", "ran over by 15 min"), without working out a clock time.
- If the date isn't stated, ask for it or mark it **not stated**. If only part of it is given, write it as given and say what is missing ("3/11 (year not stated)").
- Purpose: base it only on the notes (their title or the topics covered). Don't add labels like "regular", "weekly" or "kick-off" unless the notes say so. If even the topic is unclear, write **not stated**.

### Language and style
- Keep the original language of the notes (e.g. Greek notes → Greek summary). Translate every template heading and label too ("Αποφάσεις", "δεν αναφέρεται"). Keep "TBD" as is in every language.
- Neutral and factual. Describe what happened, not how people felt. Don't present opinions as facts ("Maria thinks X is too costly", not "X is too costly").
- Active voice that shows who does what ("Nikos will send the report", not "The report will be sent").
- Write the summary, discussion points and decisions in the past tense and the third person ("The team agreed…", "Priya flagged…"). Use the future only for action items. Keep the tense the same throughout.
- Match the wording to the meeting. Board and committee minutes are formal ("The motion carried unanimously.", "The meeting was adjourned at 4:30 pm."). Team meetings can be plainer.
- Short bullets under clear headings, no long paragraphs.
- Use each person's name and each term the same way throughout. Spell out an abbreviation the first time unless it is obviously common.
- Fix spelling silently, except for people's names (see Accuracy).

## Final check

Before replying, make sure that:
- every action item has an owner and a due date (or TBD),
- every decision is stated as an outcome, not a topic,
- names, dates and figures match the original notes exactly,
- nothing was added that isn't in the notes (check the Purpose and task verbs too),
- no action item is repeated under Next steps,
- every motion has a mover, a seconder and a result (or **not stated**), and no confidential discussion is included,
- discussion points and decisions are in the past tense,
- unclear points are under **Open questions / to confirm** rather than guessed.
