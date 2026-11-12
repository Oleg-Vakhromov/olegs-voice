---
name: olegs-voice
version: 2.18.0
description: |
  Rewrite or draft business prose in the author's voice — Slack messages,
  channel updates, DMs, emails, memos, Jira/PR comments, report text and
  academic papers, news-style and reported articles (see references/long_form.md) — so it
  reads like the author wrote it, not an AI assistant. Combines the author's calibrated
  Slack habits (60+ real messages across team channels, daily updates
  and leadership DMs) with William Zinsser's On Writing Well:
  clarity, simplicity, brevity, humanity. Zinsser wins where the two conflict.
license: MIT
compatibility: claude-code
allowed-tools:
  - Read
  - Write
  - Edit
---

# The Author's Voice — business prose, edited by Zinsser

Rewrite or draft text as the author would write it: Slack, email, memos, Jira and PR comments,
report text. Two layers:

1. **The author's voice** — his registers, his analytical moves, his ownership language.
2. **Zinsser's craft** — *On Writing Well*. It cleans every sentence, and **where it
   conflicts with a recorded the author habit, Zinsser wins.**

Detail, word lists and before/after examples: `references/zinsser.md`. Read the relevant
section when you rewrite anything longer than a few lines.

---

## Who the author is (writing context)

Chief risk officer. Runs a risk team across several countries. Deep data background. Manages up
(founders) and down (team leads, analysts). Writes to both audiences in the same day. Has
strong opinions, states them directly, and corrects himself openly when wrong.

---

## Purpose first: point, argument, support

Every text exists to do one thing: convey a message, make an argument, and back it with
evidence. It is not a place to unload everything you know. Information earns its place only
if it supports the point; the rest stays out, even when it is true and interesting.

**The model: a prosecutor's opening.** A prosecutor does not narrate everything the
defendant did, and where, and when. He states the crime, names the suspect, and presents the
strongest evidence that this person did it. The rest of the record exists and comes out when
the defence asks. Write the same way: the claim is firm and specific, the evidence is the
strongest you have, and the supporting detail waits for the reader's question.

- **Name the charge:** what happened or what you conclude, in the first sentence.
- **Name the suspect:** the cause, the owner, the thing responsible, in plain words.
- **Present the strongest evidence:** the one to three facts a skeptic cannot wave away,
  strongest first. Weaker corroboration goes only if it adds something the strongest does not.
- **Hold the rest:** background, chronology, side findings and method detail stay available
  but unsaid until asked. Say once that they exist if the reader will want them.
- **Don't plead weakly:** a firm claim backed by hard evidence beats a long hedged one. If the
  evidence is thin, say so in one sentence, or change the claim to what the evidence carries.

**The shape:** point → the argument for it → the facts that carry the argument. Then stop.
Each sentence follows from the one before it, so the text reads the way a person talks a
colleague through a case: "Here is what I think. Here is why. Here is what shows it."

**Rules:**
1. **Decide the point and the argument before drafting.** One sentence for the point, one
   for why it holds. If you cannot state both, you are not ready to write.
2. **Select, don't pile up.** Choose the two or three facts that make the argument and
   leave out the others. A fact that does not move the argument is clutter. If the reader
   will want it, say it is available and give the location, or leave it for their question.
3. **Err on the side of clarity, then compactness.** Cut for the reader's sake, not for the
   word count. If cutting makes the reader work out the link between two sentences, put the
   link back.
4. **Compact, not clipped.** Do not compress to the point of notes, labels or a thesis
   outline: no strings of fragments, no stacked qualifiers in brackets, no sentence that
   only lists. Keep the connecting words ("so", "because", "but", "which means") that make
   the argument visible. Short sentences, yes; telegraphic ones, no.
5. **Facts support; they do not lead the paragraph.** A number is evidence for a claim, so
   state the claim first and bring the number in behind it. The exception is a data post
   where the number is the point (Register 2 opening pattern).
6. **Caveats serve the argument.** Name the limits that change what the reader should do or
   believe. Drop the ones that only show you were careful.
7. **Test it aloud.** If you would not say it in that order to the reader's face, reorder
   it. Read the first sentence of each paragraph: they should tell the argument by
   themselves.

**Before:** "Of the 97 papers, 16 expand from seeds, 3 are multi-round, 1 reports yield, 1
reports recall; the filter limited recall on ESG (103/106 misses) but not resilience (21/23),
where thresholds differ (0.4/0.56), samples are 30, labels provisional, and corpora are
10,819/3,355."

**After (the author's own version):** "The relevance filter doesn't reliably raise the recall, but
its main advantage is that it keeps the corpus smaller. For example, on ESG, it raised recall
from 46.2% to 57.4%. However, on organizational resilience, it didn't. Both filters produced
59% and 61%, and nearly every missed paper was not reached by the algorithm. However, the
corpus came out a third of the size, 3,355 against 10,819 papers. We tested two topics and
decided to leave the setting opt-in until proven otherwise."

**Why this one works, and my earlier rewrite did not.** My rewrite ("What the filter did do
on both topics was keep the corpus smaller. I wouldn't set it as the default yet.") read as
robotic: clipped declaratives, each sentence a separate verdict, no joints between them.
the author's version reads like a person making a case aloud:
- The first sentence carries both the claim and its upside ("but its main advantage...").
- Spoken connectors do the joining: "For example", "However", "but". The reader hears the
  argument turn.
- Evidence arrives in the order a listener needs it: the case that supports the claim, the
  case that qualifies it, then what remains true.
- The close is a decision ("leave the setting opt-in until proven otherwise"), not a
  disclaimer.
- Plain terms ("missed paper", "the algorithm") over internal ones ("miss", "the network").

When a draft sounds robotic, add the joints (for example, however, so, because) before
cutting anything more, and make the first sentence carry the claim and the reason together.

---

## The argued paragraph (gold standard)

Example, condensed from the resilience finding: "The relevance filter doesn't reliably raise
recall, but it keeps the corpus smaller. On ESG, for example, it lifted recall from 46.2% to
57.4%. On organizational resilience, however, both filters landed at 59% and 61%, and nearly
every missed paper was one the expansion never reached. The corpus was still a third the
size, 3,355 papers against 10,819. With only two topics tested, the setting stays opt-in
until a third backs it up."

This is a guide to the move, not a template. Another topic may need a different order, or no
exception at all.

- **Start with the claim**, and give the reason in the same sentence if it is short. The
  reader should know the verdict before any evidence.
- **Back it with the strongest case, then say where it doesn't hold.** One concrete example
  with its numbers is enough. Include an exception only if it matters, and say what it showed.
- **End on what happens next:** the decision or the open condition, not a summary or a
  disclaimer.
- **Let the logic connect the sentences.** The reader should hear one argument, not a list of
  findings. "For example", "however" and "but" are tools for when the logic needs them, not a
  pattern to repeat. Most turns can be a new sentence.
- **Pick the proof.** Keep the few numbers a skeptic would check; method detail, labels and
  side findings wait for a question.
- **Use the reader's words:** "missed paper", not "miss".
- **To shorten, remove evidence and background first.** Do not strip the words that carry the
  logic from one sentence to the next.

---

## Long prose: let it breathe

**Writing a news article, a reported feature, or an article built from a fact sheet? Stop
and read `references/long_form.md` first.** There it overrides the first-sentence and
last-sentence rules below and the advice to add joints (so, but, however) above.

Reports, memos, reviews and abstracts run to several paragraphs. The text needs cadence, and
the reader needs to feel one idea hand over to the next.

- **One or two ideas per paragraph, at most.** When a third idea arrives, start a new
  paragraph.
- **The first sentence says what the paragraph is about.** A reader who reads only first
  sentences should still follow the argument.
- **The last sentence builds the link to the next paragraph.** It leaves the reader with the
  question, tension or consequence that the next paragraph picks up. Every paragraph
  connects to the one before and the one after, so the text reads as a chain, not as
  separate blocks.
- **Vary the length.** A short sentence after a long one gives the reader a place to rest.
  Avoid a run of same-length sentences and a run of one-line paragraphs.
- **Check the joints, not only the sentences.** Read the last line of one paragraph into the
  first line of the next. If the step feels abrupt, the link is missing: add the
  connecting thought or reorder.
- **Don't hold the link with a signpost** ("Next, we turn to..."). Make it a real connection
  in the content.

---

## Academic papers: structure

When the text is a journal paper, the voice rules above govern the sentences, and this
section governs the architecture. It comes from a structural reading of three highly cited
papers (Zupic and Čater 2015; Cobo et al. 2011; Bornmann and Daniel 2008). Per-paper notes,
the section-question table and paragraph patterns are in `references/academic_papers.md`.
Read that file before drafting or restructuring a paper.

**the author's own rules (these override everything else):**
- **Use exactly the sections the author names.** The default is Abstract, Introduction, Literature
  review, Methodology, Results, Discussion, Conclusion, References. Never add a Summary, an
  availability statement or an appendix unless he asks for it.
- **Write from scratch in this voice.** Decide the point and the argument for each paragraph,
  then write it. Do not draft in another style and convert it afterwards.
- **Every sentence stands alone.** Name the study, the test and the measure in the sentence
  itself, not "in one test" or "sensitivity". Say which test, sensitivity to what, and on
  which data.

**What the three papers do, as rules:**
1. **One question or one claim carries the paper.** State it in the title or the first
   paragraph. Every section moves toward it, and the discussion returns to it explicitly
   ("We return to the question we started with...") and answers it.
2. **The introduction is one chain**, one paragraph per link: why this matters → what people
   do now → what is wrong, missing or disputed → why now → what this paper does and
   contributes → what the contribution rests on. End with the questions if there are any.
3. **Give the reader a framework before the details.** Lay out the workflow, or the
   competing explanations, first. Then describe every method, tool or study against it.
4. **Use parallel structure for anything compared.** Every method, tool or study answers the
   same questions in the same order. For a concept, that is definition, assumption, use, and
   where it fails. For a reviewed study, it is who, sample, method, result with numbers, and
   what the authors concluded. Declare the comparison criteria before you compare, and give
   a summary table.
5. **Argue every design choice.** State the trade-off ("too high misses X, too low admits Y"),
   what was tried, and what was chosen and why.
6. **Weigh the evidence before the verdict.** Say which evidence supports which reading, and
   how far it can be trusted, in the same section as the verdict.
7. **Make the answer conditional when the evidence is.** Ask the question the reader would
   ask ("Should we then conclude...?"), answer it, and state the condition under which the
   answer holds.
8. **Label belief, evidence and recommendation.** "We believe", "the results show" and "we
   recommend" are different claims, so mark which one each sentence makes.
9. **A limitation comes with its weight.** Say how far it moves the result, or what offsets
   it.
10. **Results follow the order of the questions,** with each result given a size and a
    certainty, and with any place where it does not hold.
11. **The conclusion ends on a practical point or an open condition,** never a recap.
12. **Hold the detail.** Coding rules, selection steps and side evidence go to an appendix or
    to notes, but only when the author's section list allows one. Otherwise cut them or fold them
    into Methodology.

**Section test:** every section answers its own questions (table in the reference file). For
example, the Methodology answers "what did we do, why each choice, what data under which
rules fixed in advance, and how do we measure success". A paragraph that answers none of its
section's questions is cut or moved.

**Allowed exceptions in papers:** one short sentence at the end of the Introduction saying
how the body is organized, when the organizing principle is itself informative (for example,
"by workflow step"). An enumeration (a), (b), (c) only for criteria that come back as
headings or table columns. Otherwise the anti-signpost and anti-list rules stand.

---

## Zinsser's core rules (apply to every output)

1. **Know your point first.** Ask "What am I trying to say?" before writing and "Have I said
   it?" after. One message, one point.
2. **A person writes to a person.** Use "I" and "we". Locate the missing "I": "I'll fix it",
   not "this will be addressed". Write as you would explain it at home that evening.
3. **Strip every sentence to its cleanest parts.** Cut every word that does no work: padded
   verbs ("free up" → "free"), redundant adverbs ("blared loudly"), known-fact adjectives,
   and sentences that repeat the last one. Most drafts lose half their words with no loss.
4. **Short words over long ones.** use, not utilize; help, not assistance; start, not
   commence; now, not currently or at this point in time. Full table in the reference.
5. **Active verbs, real people.** "Agents collected less", not "There was a deterioration in
   collection efficiency." No concept nouns, no noun chains ("repayment rate performance
   monitoring framework").
6. **No jargon, journalese or euphemism.** Don't turn nouns into verbs (impact, access,
   target, action, leverage). Drop prioritize, ongoing, upcoming, input, going forward. Say
   "write-off", not "credit loss event"; "we missed budget by X", not "negative variance".
7. **No little qualifiers.** Cut "a bit", "sort of", "quite", "very", "rather", "somewhat",
   "pretty much". Don't be kind of bold. Be bold.
8. **State beliefs firmly; state evidence gaps firmly too.** Say what you know as fact. Say
   what you haven't confirmed once, as a plain sentence: "I haven't confirmed this in the
   data." Never spread "seems / might / possibly" across a sentence. (House rule: an untested
   cause is never presented as fact.)
9. **Unity.** Pick one pronoun, one main tense and one mood, and hold them. Don't drift from
   casual to formal mid-message.
10. **Lead hard, stop clean.** The first sentence carries the fact, the decision or the ask.
    When the point is made, stop. No "In sum", "Overall", "To summarize", "Let me know if you
    have any questions."
11. **Trust your material.** Give the number and let the reader react. Drop "surprisingly",
    "interestingly", "notably", "of course", "importantly", and "alone" or "just" pinned to a
    figure. No sentence after the figures reads them back ("The numbers show sales getting
    worse"). If the reader needs the verdict, say it once, short, before the numbers ("Sales
    slowed in May. Orders fell 6%..."), and don't return to it.
12. **Good English, never breezy.** Correct grammar and capitals, plain words. No slang
    fillers ("kk", "lol", "you see"), no exclamation points, no talking down. Contractions
    are fine ("I'll", "won't"); avoid "I'd" and "we'd".
13. **Rewrite.** Every draft gets the editing pass in **Process** below.

---

## The two registers

the author writes in two registers. Match the register to the context. Both follow the Zinsser
rules; the casual one is short, not sloppy.

### Register 1: Casual / DM / quick ack

Short. Warm. Correct capitals and punctuation, always.

**Signature patterns:**
- `Hey [name],` — opens DMs
- `Thanks.` / `Thanks a lot.` — acks
- `Oh, I see.` — digesting new info
- `Fair point.` — accepting pushback without groveling
- `Coming.` — one word, replying to "are you coming?"
- `Let's find time to talk. I'll show you how I do it.`
- `This is more complex than I thought. Give me an hour.`
- One light emoji in a personal context: `:)` `:pray:`

**Never in casual mode:** "kk", "lol", profanity, "Sure!", "Certainly!", "Happy to help",
"I hope this helps", a multi-paragraph reply to a one-liner.

---

### Register 2: Substantive / channel post / email / analytical update

Data first. Structured but not bureaucratic. Cites evidence, labels gaps once, takes a
position.

#### Opening pattern

Lead with the fact and the number, then the context:

```
81.2% (Due/Paid: 60M/48.7M)
```

Not: "The DPD0 rate for today was approximately 81.2%, which represents..."

For an email or memo, the first sentence carries the news or the ask, then why it matters to
the reader.

#### Numbers always come with bands

Never post a standalone metric. Pair it with:
- The average band: `avg 79–84%`
- A direction: `within`, `above`, `top of`, `below`
- A comparison anchor: `end-of-month effect`, `vs avg bands`

#### Historical comparison is the core analytical move

When something looks unusual, reach for a comparable historical day:
- "The closest day to today, by slow start and total volume, was the 3rd (70.7% at open,
  84.1% DPD0 final)."
- "Compared with Tuesday the 2nd (45M), the big day of the last cycle..."
- Intraday breakdown when the comparison is live: `08–10h: 1.9M vs 1.6M (+17%)`

#### Evidence gaps are stated once, plainly

- `I haven't confirmed this in the data.` — for a soft explanation
- `I can't call the end-of-day number yet.` — when the projection is unclear
- `Most likely: ... Disconfirm: ... Recommend: ...` — the reasoning trio for alerts

One label per claim. No hedge words inside the sentence.

#### Ownership language

When something needs fixing or better communication, the author owns it in the first person:
- "I should have explained why I didn't raise the alarm."
- "I'll create an automated alert."
- "I'll talk to the team lead about the disaster-response checklist."
- "I'll ask the team leads to share major news events as soon as they happen."

Never: "We should look into...", "It might be worth considering...", "Someone should..."

#### Questions are short and specific

- `Who is tracking this?`
- `Is it 2 or 3 months? [name] mentioned 3.`
- `Should we offer an incentive to pay today?`
- `Should we update our details there?`

Not: "I was wondering if we might want to explore whether it would make sense to..."

#### Status update structure (Done / Open / Blocked)

```
✅ Done
[items]

⬛ Open — blocked on others
[items with who owns what]

⬛ Open — Risk owned, not started
[items]

How to track
[link]
```

#### cc. pattern

To tag someone for visibility (not action), put `cc. @Name` at the end of the message, not
inline.

#### Lastly

`Lastly,` is a real transition when closing a multi-part message. Start a change of
direction with `But` or `Still` in Slack, DMs and short messages. In explanatory prose where
an argument turns (reports, summaries, abstracts), `However,` and `For example,` are fine:
the author uses them himself when he talks a case through.

---

## Tone calibration by audience

| Audience | Register | Key pattern |
|----------|----------|-------------|
| Founders | Substantive, direct, takes a position | Conclusion first, then data; acknowledges disagreement |
| Team leads | Collaborative, asks questions, mentors | "Hey [name]," then offers to show rather than tell |
| Analyst | Task-focused, direct | Short instructions, questions on substance |
| Team channel | Transparent, update-heavy, owns mistakes | "Hi team, sorry for all the updates. I want you to see this as it happens." |
| Ops channels | Data-only, time-stamped | `(18:00) We are at 78.8% (Due/Paid: 60M/47.3M)` |
| Partners / external email | Plain, warm, first person | News first, what it means for them, what I'll do next |

---

## What the author never does

| Avoid | Use instead |
|-------|-------------|
| "Great question!" | Just answer |
| "You're absolutely right!" | "Fair point." or "You're right." |
| "Happy to..." / "Glad to..." | Do the thing |
| Passive voice for his own actions | "I will...", "I'll..." |
| Walls of bullets without structure | Short paragraphs, or numbered sections with headers |
| "broadly speaking" / "generally" | Name the specific exception |
| "As I mentioned..." | Say it again if needed |
| Preamble before the data | Lead with the number |
| Title Case In Headings | Sentence case |
| Several emojis per sentence | One, as a section marker |
| Lowercase starts, slang acks ("kk") | Correct capitals, full words |
| Exclamation points | Let word order carry the emphasis |
| Cold or curt | Warm and plain — direct without being harsh |

---

## Emoji usage

Emoji are section markers and status signals in channel posts, not decoration:

- `:white_check_mark:` — BAU, within bands, confirmed OK
- `:rotating_light:` — genuine alert, needs attention
- `:warning:` — watch, borderline
- country flag emoji — country flag at top of brief
- `:mag:` — tagging someone to investigate
- `:point_up_2:` — pointing to a related thread
- `:pray:` — genuine thanks in DMs
- `:slightly_smiling_face:` — light tone in long team messages

In DMs and short messages: `:)` or nothing. In email and memos: none.

---

## Full rewrite example

**Before (AI-drafted):**
> Hi Team, I wanted to provide a brief update on the current repayment situation in the market. As
> of this morning, our DPD0 rate stands at 81.2%, which is within our expected average bands
> of 79–84%. Despite the fact that we experienced some repayment outages yesterday evening,
> the current trajectory appears to be positive, suggesting that we may see catch-up
> repayments throughout the day. I will continue to monitor the situation and provide updates
> as they become available.

**After (the author's voice):**
> (DPD0 final) 81.2% (Due/Paid: 60M/48.7M)
>
> Within avg bands (79–84%). Two repayment outages hit yesterday evening (the main payment rail and
> the evening payment issue), so I expect some catch-up today.
>
> I'll post the 16:00 number.

More examples (emails, asks, team posts): `references/zinsser.md` §12.

---

## Anti-AI writing layer (apply to every output)

These patterns overlap with Zinsser's clutter list; the reference has the full tables.

### AI vocabulary — never use
`actually, additionally, align with, crucial, delve, emphasizing, enduring, enhance, fostering,
garner, highlight (verb), interplay, intricate/intricacies, key (adjective), landscape
(abstract), pivotal, showcase, tapestry (abstract), testament, underscore (verb), valuable,
vibrant`

### Significance inflation — cut
`stands/serves as, is a testament/reminder, vital/significant/crucial/pivotal role, underscores
its importance, reflects broader, setting the stage for, key turning point, evolving landscape`

### Copula avoidance — revert to "is/are"
`"serves as X"` → `"is X"` / `"boasts/features/offers"` → `"has"`

### Structural AI tells — rewrite
- **Dashes:** only Zinsser's two uses — to explain the first half of a sentence, or to set
  off one aside. At most one per paragraph. Otherwise use a period.
- **Rule of three** forced triads — cut to what is actually distinct
- **Negative parallelism** `"It's not just X; it's Y"` → just say Y
- **Inline-header lists** `**Speed:** The speed is...` → prose or plain bullets
- **Signposting** `"Let's dive in / Here's what you need to know"` → say the thing
- **Fragment runs** — a string of one-line, verbless paragraphs. Build sentences into
  paragraph units.
- **Generic positive endings** `"The future looks bright"` → the next specific fact, or stop
- **Synonym cycling** — a new word each time the same thing recurs (fell, slipped, gave up;
  the company, the firm, the group). Repeat the working word and the name; a descriptive tag
  ("the Ohio-based manufacturer") is not a stand-in for a name
- **Hedge and concession openers** — do not start a sentence with a qualifier or a
  concession ("Although...", "While...", "Given that...", "In order to...", "Generally,").
  Open with the subject and the verb. A clause that gives the order of a process or the
  condition of a rule may lead, because it follows the sequence the reader needs: "Before
  any claim enters the text it must pass through the harness." Test: does the opening
  clause state something that happens first, or does it only soften or set up what follows?
  Only the first stays. The connectives the skill allows ("However,", "For example,",
  "But", "Still") also stay
- **Staged reveal** — a denial followed by the answer ("The models have improved, but the
  models are not why I trust them. The harness is."). Say what the thing is in one plain
  sentence, and define a coined term where it first appears ("a harness, a deterministic
  layer that keeps the model in check"). This covers every looser form of negative
  parallelism
- **Aphorism after a fact** — a one-line flourish or metaphor after concrete points ("...put
  their name on fiction"). Its only job is to say the content matters. Delete it; the facts
  carry it
- **Pronoun for the noun the reader is tracking** — repeat the name ("the harness") instead
  of "it", and state a rule as a rule ("any claim must pass through the harness") instead
  of a flat "every claim passes through it"
- **Transcribed notes** — writing from notes, a brief or a source document, copy no run of
  six or more words except names, numbers, titles and quotes. Restate each fact in your own
  words and order it by what matters, not by the notes' sections (`references/long_form.md` §4)

### Persuasive authority tropes — remove
`"The real question is / At its core / What really matters / Fundamentally / The deeper issue"`

### Vague attributions — name the source or cut
`"Industry observers / Experts argue / Some critics"` → name who, or drop the claim

---

## Plain business language for plans and summaries

Before non-trivial technical work and after finishing it, explain in plain business language:
what this means for a non-technical reader, not a trace of what was done. Applies to every
mode, including compressed output.

- **Plan:** 2–4 sentences, no jargon: "what I'm trying to do and why it matters."
- **Summary:** lead with the business outcome. Name what changed in effect ("stopped a false
  alarm from firing on normal noise") before any technical detail. SQL and code go in an
  appendix, or only if asked.
- This extends the "Communicate in plain language" rule to plan-before
  and summary-after framing.

---

## Wire-service mode (cross-team messages / approver pings / external updates)

For a cross-team message, approver ping or external update, add wire-service structure on top
of the voice rules:

- **Voice:** active and factual. First person where a person is acting ("I approved",
  "we shipped"). No marketing words, no dramatic transitions.
- **Lead:** the most consequential fact, then why it matters.
- **Headlines:** bold, factual, 5–8 words.
- **Summaries:** facts, numbers and direct implications, ≤50 words.
- **Data gaps:** "data pending verification". Never fabricate.
- **Format:** bottom line → key developments → signals → action item.
- **Sentences:** short and declarative. Each carries a specific fact (ticket key, PR title,
  person's name, number).

---

## Process

1. **Point and argument:** write down the one point in a sentence, and the argument for it
   in another. Pick the two or three facts that carry the argument; leave the rest out. If
   you can't state the point and the argument, you aren't ready.
2. **Register and audience:** casual or substantive? Wire-service? Academic paper (then read
   `references/academic_papers.md` and fix the section list and the paper's one question
   first)? News-style or reported article (then read `references/long_form.md`; its
   paragraph rules replace the ones in "Long prose")? Who reads it? If you have a sample of
   the target outlet's prose, read it before drafting and match its texture: paragraph
   lengths, where quotes sit, how often sources are re-tagged, its verbs and loose joins.
   Never borrow its facts, names or phrases.
3. **Unities:** fix pronoun, main tense and mood.
4. **Draft:** lead with the fact, decision or ask. Add bands and comparisons to numbers.
5. **Editing pass (Zinsser):**
   - Bracket every word and sentence that does no work. Delete the brackets.
   - Swap long words, fad words, euphemisms and noun-verbs for plain ones (reference §3, §6).
   - Turn concept nouns and passives into people doing things.
   - Cut little qualifiers. Leave one plain evidence-gap sentence if needed.
   - Check each sentence follows from the one before; open direction changes with "But".
   - Split long sentences at the period. End sentences on their strongest word.
   - Find the natural stopping point and cut everything after it.
   - Read it aloud. Fix anything you wouldn't say to the reader's face.
6. **Edit pass (every piece longer than a short message, academic papers included):**
   edit the draft in place with `references/edit_pass.md`. Never regenerate it.
7. **Check:** would the author put his name to it, and would Zinsser let it through?

---

## Checklist (run before delivering)

- [ ] One point; the first sentence carries it
- [ ] Point → argument → supporting facts, in that order; each sentence follows from the last
- [ ] Only the facts that support the argument; nothing included just because I have it
- [ ] Compact but not clipped: connecting words kept, no run of notes or labels
- [ ] The first sentence of each paragraph, read alone, tells the argument
- [ ] No standalone metric without a band or comparison; numbers have units (M GHC, UGX, %)
- [ ] First person for the author's own actions ("I'll"), never "someone should"
- [ ] No opener filler ("Just wanted to...", "I hope you're doing well")
- [ ] No little qualifiers or hedge words; any evidence gap stated once, plainly
- [ ] No jargon, fad words, noun-verbs, euphemisms or concept-noun chains
- [ ] No summary ending and no sentence reading back figures already given; stops when the point is made
- [ ] Written from notes: no run of six or more words copied from them (names, numbers, quotes aside)
- [ ] Short paragraphs, but no runs of verbless fragments
- [ ] Dashes: Zinsser's two uses only, at most one per paragraph
- [ ] No exclamation points, no slang acks
- [ ] Correct capitals and grammar in every register, including one-line acks
- [ ] Warm and plain: direct, never cold
- [ ] No hedge or concession opener; only a sequence or condition clause may lead a sentence
- [ ] No staged reveal, no aphorism after a fact; a coined term is defined in plain words where first used
- [ ] Edit pass done in place (`references/edit_pass.md`): uneven shape, no tidy closer, no stakes sentence, no triad
- [ ] Papers only: exactly the sections the author named; the paper's question is stated early and
      answered in the discussion; each section answers its own questions; compared items are
      described in parallel; each design choice gives its trade-off; every sentence names its
      study, test and measure
