# Waiga Arya

Director of Business Strategy and Innovation at Sadaway Pvt. Ltd., formerly Indus
Cosmeceuticals. The company began in 1976 as a research and analytical laboratory in
Faridabad, India, and today manufactures organic beauty and personal care products under
Indus Valley Organic Beauty, MINA IBROW and Bio Organic, sold across India, the United
States, Europe and Asia.

I trained as a cosmetic scientist before moving to the commercial side of the
industry, which is why I tend to argue about formulation and margin in the same
meeting. I hold an MBA from the Yale School of Management, and before this role I
worked in marketing and strategy at L'Oreal in Paris.

I build tools for real-world operators.

I set product direction, operating boundaries, and release standards. Public code and
documentation are AI-assisted and reviewed, and every proposed release is checked
against those standards before publication.

## Current work

**[Repo Scout](https://github.com/Waiga/repo-scout)** — reads a public GitHub
repository and reports the static evidence about it: what it can check, what it
could not establish, and how much of the repository it actually opened. Version 0.2
was run against 385 real public repositories it did not author. Version 0.1 had been
reading 8% of the bytes of a typical one, nothing at all in 15 of them, and reporting
no findings either way; two of its four verdicts could never be produced by any input.
The README carries the before and after, including the parts that did not improve and
the directories it does not look in at all.

**[Follow Through](https://github.com/Waiga/follow-through)** — finds the commitments
people make out loud in a meeting transcript, and tracks each one until somebody closes
it with a reason. Reads English and Hinglish, because most meetings in India are not
held in one language. Runs entirely on your machine: no account, no API key, and no
way to upload anything. Version 0.2 was measured against 6,320 real meeting records —
IETF working-group minutes and US congressional hearings — and the README carries the
score, including the parts of it that are poor and the question the corpus could not
answer.

**[Show Your Work](https://github.com/Waiga/show-your-work)** — finds the numbers in a
spreadsheet that nobody can explain: a formula someone typed over, a total that stops
one row short, a cell quietly doing something different from the column around it.
It says which numbers the sheet cannot account for, never that a number is wrong.
Local only, and cell contents stay out of the report unless you ask for them.
`pip install unexplained-cells` — the command is still `show-your-work`; the plain
name on the package index belongs to somebody else's project, so it was left alone.

**[Before You Send](https://github.com/Waiga/before-you-send)** — reads a PDF and
reports what is still inside it that you may not mean to send: text under a box that
was never removed, an earlier version of the document kept in the same file, an
attached spreadsheet, a name left in the properties. It never says a file is safe to
send, and it reports the places it could not see into separately from what it found.
Local only, and what it finds stays out of the report unless you ask for it.
`pip install before-you-send`

**[Says On The Tin](https://github.com/Waiga/says-on-the-tin)** — finds where a
cosmetic label contradicts itself: a free-from claim on the front, and an ingredient
on the back that breaks it. Paraben-free over a list containing methylparaben, vegan
over carmine, sulphate-free over sodium laureth sulphate. It never says a product is
compliant or clean — both halves it compares are printed on the same pack, so the
finding is arithmetic rather than an opinion. It also reports what it deliberately did
*not* count, because flagging cetearyl alcohol under an alcohol-free claim is how a
tool like this loses a formulator in the first five minutes. Measured against 2,554
real published labels, which showed that reading only English claims found none of the
contradictions in the sample: they were on Portuguese, French, German, Italian and
Dutch packs.

Five tools, one rule. Each one reads something people already produce — a repository, a
meeting, a spreadsheet, a document about to leave the building, a label about to be
printed — and reports only what it can actually check. Absence of evidence is reported as unknown, never as a confirmed
no, and none of them claims a certainty it cannot support.

Each has now been run against real files it did not write, and each time that found
things the tests did not. Those results are in the READMEs, including where the numbers
are poor and what the measurement could not settle. The newest one was also handed to
a reviewer told to attack it before release, which found five more; that is in its
README too.

## Elsewhere

- [waiga.github.io](https://waiga.github.io) — who I am, in one page
- [LinkedIn](https://www.linkedin.com/in/waigaarya/)
- On the Python Package Index: [unexplained-cells](https://pypi.org/project/unexplained-cells/)
  and [before-you-send](https://pypi.org/project/before-you-send/)

## Contributing

Useful tests, clearer evidence, reproducible examples, honest limitations, and bounded
technical ownership are first-class contributions.
