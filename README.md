# Waiga Arya

I build tools for real-world operators.

I set product direction, operating boundaries, and release standards. Public code and
documentation are AI-assisted and reviewed, and every proposed release is checked
against those standards before publication.

## Current work

**[Repo Scout](https://github.com/Waiga/repo-scout)** — evidence-led evaluation of
public developer and AI tooling. Reports what the evidence supports, and reports the
rest as unknown.

**[Follow Through](https://github.com/Waiga/follow-through)** — finds the commitments
people make out loud in a meeting transcript, and tracks each one until somebody closes
it with a reason. Reads English and Hinglish, because most meetings in India are not
held in one language. Runs entirely on your machine: no account, no API key, and no
way to upload anything.

**[Show Your Work](https://github.com/Waiga/show-your-work)** — finds the numbers in a
spreadsheet that nobody can explain: a formula someone typed over, a total that stops
one row short, a cell quietly doing something different from the column around it.
It says which numbers the sheet cannot account for, never that a number is wrong.
Local only, and cell contents stay out of the report unless you ask for them.

**[Before You Send](https://github.com/Waiga/before-you-send)** — reads a PDF and
reports what is still inside it that you may not mean to send: text under a box that
was never removed, an earlier version of the document kept in the same file, an
attached spreadsheet, a name left in the properties. It never says a file is safe to
send, and it reports the places it could not see into separately from what it found.
Local only, and what it finds stays out of the report unless you ask for it.

Four tools, one rule. Each one reads something people already produce — a repository, a
meeting, a spreadsheet, a document about to leave the building — and reports only what
it can actually check. Absence of evidence is reported as unknown, never as a confirmed
no, and none of them claims a certainty it cannot support.

## Contributing

Useful tests, clearer evidence, reproducible examples, honest limitations, and bounded
technical ownership are first-class contributions.
