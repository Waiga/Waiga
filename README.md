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

I direct the building of tools for real-world operators.

I set product direction, operating boundaries, and release standards. Public code and
documentation are AI-assisted and reviewed, and every proposed release is checked
against those standards before publication.

## Current work

**[Repo Scout](https://github.com/Waiga/repo-scout)** reads a public GitHub
repository and reports the static evidence about it: what it can check, what it
could not establish, and how much of the repository it actually opened. Version 0.2
was run against 385 real public repositories it did not author. Version 0.1 had been
reading 8% of the bytes of a typical one, nothing at all in 15 of them, and reporting
no findings either way; two of its four verdicts could never be produced by any input.
The README carries the before and after, including the parts that did not improve and
the directories it does not look in at all.

**[Follow Through](https://github.com/Waiga/follow-through)** finds the commitments
people make out loud in a meeting transcript, and tracks each one until somebody closes
it with a reason. Reads English and Hinglish, because most meetings in India are not
held in one language. Runs entirely on your machine: no account, no API key, and no
way to upload anything. Version 0.2 was measured against 6,320 real meeting records,
from IETF working-group minutes and US congressional hearings. The README carries the
score, including the parts of it that are poor and the question the corpus could not
answer. `pip install follow-through`

**[Show Your Work](https://github.com/Waiga/show-your-work)** finds the numbers in a
spreadsheet that nobody can explain: a formula someone typed over, a total that stops
one row short, a cell quietly doing something different from the column around it.
It says which numbers the sheet cannot account for, never that a number is wrong.
Local only, and cell contents stay out of the report unless you ask for them.
`pip install unexplained-cells`, though the command is still `show-your-work`. The
plain name on the package index belongs to somebody else's project, so it was left alone.

**[Before You Send](https://github.com/Waiga/before-you-send)** reads a PDF and
reports what is still inside it that you may not mean to send: text under a box that
was never removed, an earlier version of the document kept in the same file, an
attached spreadsheet, a name left in the properties. It never says a file is safe to
send, and it reports the places it could not see into separately from what it found.
Local only, and what it finds stays out of the report unless you ask for it.
`pip install before-you-send`

**[Says On The Tin](https://github.com/Waiga/says-on-the-tin)** finds where a
cosmetic label contradicts itself: a free-from claim on the front, and an ingredient
on the back that breaks it. Paraben-free over a list containing methylparaben, vegan
over carmine, sulphate-free over sodium laureth sulphate. It never says a product is
compliant or clean. Both halves it compares are printed on the same pack, so the
finding is arithmetic rather than an opinion. It also reports what it deliberately did
*not* count, because flagging cetearyl alcohol under an alcohol-free claim is how a
tool like this loses a formulator in the first five minutes. Measured against 2,554
real published labels, which showed that reading only English claims found none of the
contradictions in the sample: they were on Portuguese, French, German, Italian and
Dutch packs. `pip install says-on-the-tin`

**[On The List](https://github.com/Waiga/on-the-list)** reads a cosmetic
ingredient list and reports what the EU's official annexes say about the ingredients
on it: a name that matches the prohibited list, a colour printed out of position, the
same ingredient entered twice. It is the first of these that checks a document against
an outside official register rather than against itself, and the register is shipped
inside the package, so nothing leaves the machine. It reports a match as a match and
never as a compliance verdict, because an ingredient list states no concentrations and
most annex entries carry a condition a label cannot answer. The pinned corpus run
selected 16,635 published labels. An exhaustive review of the 19 Annex II entries
behind 1,066 unconditional prohibited findings found one overbroad mapping responsible
for 99 findings. In a seeded sample of 30 repeated entry findings, 21 were false
positives and 9 correctly described a repeated normalized name in the recorded text.
This is a sample result, not a population rate. The warning wording check could not be
measured with this corpus. The README publishes the method, findings, and limits.
`pip install on-the-list`

**[Adds Up](https://github.com/Waiga/adds-up)** reads a price list and reports
the arithmetic in it that contradicts itself: a volume tier where buying more costs
more per unit, the same item priced two different ways, a stated discount that does
not reconcile with the prices beside it. It never says whether the pricing is right,
because a price list states no cost and a tool that cannot see cost cannot see margin.
Measured over 200 real hospital price files, 20,513,338 rows read and 190,549 set
aside because their cell count did not match the header, and 29,521 published utility
tariffs. Hand-auditing the first run found a defect in the reader, not the
checks: rows with an unquoted comma shift every column after the break, and the tool
was reporting findings from them. One file supplied a third of a check's entire output
that way. It is fixed, the rows are now set aside and counted, and the account of it is
in the README because it is the strongest thing the measurement has to say.
`pip install adds-up`

Seven tools, one rule. Each one reads something people already produce: a repository, a
meeting, a spreadsheet, a document about to leave the building, a label about to be
printed, an ingredient list about to be signed off, a price list about to go out. It
reports only what it can actually check. Absence of evidence is reported as unknown, never as a confirmed
no, and none of them claims a certainty it cannot support.

The On The List README records two defects from its real label work. One input path
exited clean when a prohibited ingredient appeared first, and two print orders of the
same colourant received opposite answers. Both examples and their fixes are documented
there.

## Writing

**[An ingredient list cannot tell you most of what you want to know](https://medium.com/@aryawaiga0/an-ingredient-list-cannot-tell-you-most-of-what-you-want-to-know-f3807f357837)**,
September 2026. What 16,635 real published cosmetic labels say when they are checked
against the European Commission's own register, why more than half the prohibited-list
matches turn on a condition an ingredient list cannot answer, and what a hand audit of
30 repeated entry findings found, including 21 false positives and the limits of that
sample.

## Elsewhere

- [waiga.github.io](https://waiga.github.io): who I am, in one page
- [LinkedIn](https://www.linkedin.com/in/waigaarya/)
- [Medium](https://medium.com/@aryawaiga0)
- On the Python Package Index: [adds-up](https://pypi.org/project/adds-up/),
  [before-you-send](https://pypi.org/project/before-you-send/),
  [follow-through](https://pypi.org/project/follow-through/),
  [on-the-list](https://pypi.org/project/on-the-list/),
  [says-on-the-tin](https://pypi.org/project/says-on-the-tin/) and
  [unexplained-cells](https://pypi.org/project/unexplained-cells/)

## Contributing

Useful tests, clearer evidence, reproducible examples, honest limitations, and bounded
technical ownership are first-class contributions.
