# meeting-notes-skill

A [Claude Code](https://claude.com/claude-code) skill that turns messy meeting notes or transcripts into a structured summary: decisions, action items with owners and due dates, open questions, and formal minutes with motions and votes.

The main rule is **never invent anything**. A missing owner becomes `TBD`. An unclear date, an uncertain name or a point nobody agreed on goes under **Open questions** instead of being guessed.

## What you get

Every summary uses the same sections, in the same order:

- **Header:** title, date, time and place, attendees, purpose
- **Summary:** 3 sentences at most
- **Decisions:** only what was actually agreed, with exact figures and dates
- **Action items:** a table with task, owner and due date (`TBD` if not stated)
- **Key discussion points:** grouped by topic, with opinions attributed ("Marco thinks…", not stated as fact)
- **Open questions / to confirm:** anything unresolved, unclear or contradictory
- **Next steps:** the next meeting and anything else coming up that isn't a task

For formal meetings, such as a board or committee, these optional sections are added when the notes contain them:

- **Motions and votes:** mover, seconder, voting method, count and result
- **Quorum and approval of the previous minutes**
- **Carried-over items:** status, plus old and new dates if a deadline moved
- **Closed sessions:** only that one took place, its times, who attended and any vote result

## Highlights

- **No guessing.** Missing owners and dates become `TBD`, an owner who is only implied becomes "Name (to confirm)", and an uncertain spelling becomes "Geoff (spelling to confirm)".
- **Careful with dates.** "Friday" stays "Friday". A calendar date is added only when the meeting's full date (day, month and year) is known: "Friday (13 Nov 2026)".
- **Keeps the original language.** Greek notes give a Greek summary, with the headings translated too.
- **Neutral and factual.** The past tense for what happened, active voice for who does what, and no feelings or opinions presented as facts.
- **Final self-check** before every answer.
- **Email draft on request.** Subject "Draft Minutes – [Meeting], [Date]", with a deadline for corrections.

## Install

Clone the repo into your personal Claude Code skills folder:

```bash
git clone https://github.com/mkarask/meeting-notes-skill.git ~/.claude/skills/meeting-notes
```

On Windows, `~` is `C:\Users\<you>`.

To use it in a single project only, clone it into `.claude/skills/meeting-notes` inside that project instead.

Claude Code picks it up automatically. There's nothing else to configure.

## Use

Paste your notes into Claude Code and ask for a summary:

```
summarize this meeting: "Q3 sync — attendees: Dana, Marco, Priya … Marco → updated timeline by Fri …"
```

You can also start it directly with `/meeting-notes`.

## Example

**Input (excerpt):**

```
Motion (Carmen) to raise plot fee from $40 to $50/yr starting 2027. 2nd by Raj.
Bill against bc "older members are on fixed incomes". Show of hands 4-1, Bill no,
Tom abstained — conflict of interest. Carried.
Raj moved to buy a 2nd compost bin, ~$300. no second.
```

**Output (excerpt; the full names come from the attendee list earlier in the notes):**

> **Raise the plot fee from $40 to $50 per year, starting 2027.** Moved by Carmen Diaz, seconded by Raj Patel. Show of hands: 4 for, 1 against, 1 abstention. Bill Novak voted against, stating that older members are on fixed incomes. Tom Reyes abstained, declaring a conflict of interest. **The motion carried.**
>
> **Buy a second compost bin (about $300).** Moved by Raj Patel. **The motion failed for lack of a seconder.**

## Files

| File | Purpose |
|------|---------|
| `SKILL.md` | The instructions and rules Claude follows |
| `template.md` | The structure every summary is filled into |

## Customize

Edit `template.md` to change the sections, and `SKILL.md` to change the rules. Keep `SKILL.md` short: under 200 lines works well. Put extra detail in separate files in the skill folder.

## License

[MIT](LICENSE). You're free to use, change and share it.
