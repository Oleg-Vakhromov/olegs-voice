# Academic papers: structure learned from three highly cited papers

Source of these notes: a structural reading (November 2026) of the three most-cited papers
rated "useful" in the ScholarGraph corpus. The papers show how sections, paragraphs and
arguments are organized. Their sentence-level habits (passives, "allows us to", stacked
citations, inflated adjectives) are not a model: Zinsser and the rest of SKILL.md still govern
the sentences.

| Paper | Type | Citations at reading |
|---|---|---|
| Zupic and Čater (2015), *Bibliometric Methods in Management and Organization*, Organizational Research Methods | Methods guide with a worked demonstration | 7,514 |
| Cobo, López-Herrera, Herrera-Viedma and Herrera (2011), *Science Mapping Software Tools: Review, Analysis, and Cooperative Study Among Tools*, JASIST | Tool comparison with a common test dataset | 3,288 |
| Bornmann and Daniel (2008), *What do citation counts measure? A review of studies on citing behavior*, Journal of Documentation | Narrative review answering one question | 1,607 |

---

## 1. What each paper does well

### Zupic and Čater: a guide built around the reader's workflow

- **The introduction runs as one argument.** It moves from why the task matters, to the two
  methods people use now, to what is wrong with them, to the rising use of the new method,
  to the gap ("there are hardly any guidelines"). It then gives the purpose and the
  contribution, says what the guidelines rest on (81 coded studies) and closes with how the
  paper shows them in use (a worked analysis). Each paragraph does one of these jobs.
- **The body follows the steps the reader will take.** The sections are Step 1 research
  design through Step 5 interpretation. The authors say so once: "We have organized the
  article according to these stages."
- **Each method is explained the same way:** what it is (a definition), what it assumes
  ("A fundamental assumption of co-citation analysis is that..."), what it is good for, and
  where it fails. The reader can compare methods because every one answers the same four
  questions.
- **A choice is written as a trade-off, then a decision.** Setting the citation cutoff is "a
  judgment call that tries to balance two competing objectives". If the cutoff is too high,
  small groups are missed. If it is too low, spurious links appear. "After several trials...
  we decided to limit our analysis to 112 documents cited nine or more times."
- **Tables answer the reader's questions.** Table 3 lists literal research questions ("Who
  are the central, peripheral, or bridging researchers in this field?") against the method
  that answers each one.
- **Belief is labelled as belief.** "We believe this is because...", "We argue there are
  three major types...", "We envision...". The reader always knows which statements are
  evidence and which are the authors' judgment.
- **A limitation comes with its counterweight.** Negative citations bias counts, "However,
  citations for negative reasons are extremely rare."
- **A question turns the results into meaning.** "What might be the conclusions from this
  brief analysis?" The next paragraph answers it with the evidence.
- **The conclusion ends on a firm practical point.** "Bibliometric methods are no substitute
  for extensive reading and synthesis... it is up to the researcher... to interpret the
  findings, which is the hard part."
- **Detail is held back.** Study selection and coding sit in Appendix A, and the steps to
  reproduce the demonstration sit in Appendix B.

### Cobo et al.: a comparison on declared criteria

- **The verdict comes early.** Before any tool is described, the introduction says that the
  tools "present complementary characteristics" and that using them together could be
  better. The rest of the paper earns that claim.
- **A shared framework comes first.** The science-mapping workflow (data, preprocessing,
  networks, normalization, mapping, analysis, visualization) is laid out before the tools.
  Every tool is then described and compared against the same steps.
- **Criteria are declared before the comparison.** The comparison uses "five points of view:
  (a) the preprocessing methods, (b)..." and puts each in its own table. A summary table
  (Table 7) pulls them together.
- **The worked test uses one dataset for every tool,** and the authors justify that choice
  from the comparison: co-word analysis was the only network every tool could build, "For
  this reason, we select the words... as the unit of analysis."
- **A synthesis section states what the comparison taught.** The "Lessons learned" section
  opens "each software tool has different characteristics" and ends "a deep science mapping
  analysis requires the use of different tools". The concluding remarks repeat the verdict:
  "There is not one software tool that we could consider the best one."
- **The authors are fair to the tools.** They note where a printed map "does not show the
  power of" an interactive tool.

### Bornmann and Daniel: a review that answers one question

- **The title is the question, and the paper comes back to it.** The discussion opens its
  final turn with "we return to our starting point, the question of what citation counts
  measure", and then answers it.
- **The introduction sets up a dispute.** It opens with history (the first use of citation
  counts in 1927), then why counts are attractive, then the two camps that disagree. It
  states the central problem and the three conditions under which counts are valid (Smith,
  1981). It says why the question matters now, and why a new review is needed: the earlier
  reviews are more than ten years old.
- **Theory before evidence.** Section 1 presents the two competing theories of citing
  behaviour and the studies that tested them. Section 2 then groups the empirical studies by
  research method: context analysis, content analysis, surveys, and studies of not citing.
- **Each reviewed study gets the same paragraph shape:** who did it, on what sample, with what
  categories, what they found (with percentages), and what the authors concluded.
- **The discussion weighs evidence before answering.** It sets out which studies support
  which theory, combines the categories into one typology with the range found for each, and
  then says why the evidence is weak (studies differ in design and cannot be replicated).
  Only then does it answer.
- **The answer is conditional, not yes or no.** "Should we then conclude that citation
  counts are not appropriate indicators...? Not so." Counts are reliable at a high level of
  aggregation and not for the individual researcher.
- **The structured abstract puts the qualification into the findings.** The findings say
  what the studies show, then "However, the results... must also be deemed scarcely
  reliable".
- **Side material goes to notes.** Notes hold the extra evidence, so the main argument stays
  short.

---

## 2. What the three have in common

1. **One question or one claim carries the whole paper.** It is in the title or the first
   paragraph, the sections build toward it, and the conclusion answers it.
2. **The introduction follows a fixed chain:** why this matters → what people do now → what
   is wrong or unresolved → why now → what this paper does and contributes → what it rests
   on. Every link is one paragraph or less.
3. **A framework comes before the details.** This is a workflow (Zupic, Cobo) or a pair of
   theories (Bornmann). It gives the reader a map, so the details have somewhere to land.
4. **Parallel structure makes comparison possible.** Every method, tool or study is
   described against the same questions, in the same order.
5. **Choices are argued.** Each design decision states the trade-off and the reason, then the
   decision.
6. **The evidence is weighed before the verdict,** and the weakness of the evidence is named
   in the same section as the verdict.
7. **Belief, evidence and recommendation are kept apart** and labelled: "We believe", "the
   results show", "we recommend".
8. **Conclusions end on a practical point or a condition,** not on a summary.
9. **Method and coding detail goes to an appendix or notes,** so the main text stays an
   argument.

---

## 3. The questions each section answers

Use these as the test for every section. If a paragraph answers none of its section's
questions, cut it or move it.

| Section | Questions it must answer |
|---|---|
| Abstract | What problem? What did we do? What did we find, with the one or two numbers that matter? What does it mean, and what is the main limit? |
| Introduction | Why does this matter? What do people do now? What is wrong, missing or disputed? Why now? What does this paper do, and what is its contribution? (Optionally, what questions guide it?) |
| Literature review | What concepts or competing explanations frame the problem? What has been tried, and with what result? What exactly is still open, and how do we know? |
| Methodology | What did we do, step by step? Why each choice: the trade-off and the reason? What data, from where, and with which rules fixed in advance? How do we measure success, and what threatens that measure? |
| Results | What did we find, in the order of the questions? How large and how certain is each result? Where does a result not hold? |
| Discussion | What does it mean, set against the literature review? How far can the evidence be trusted? What is the answer to the paper's question, and under what conditions? What should a researcher do differently? |
| Conclusion | What did the paper show, in one or two sentences? What should the reader do or believe now? What remains open? |
| References | Every source cited in the text, and nothing else. |

---

## 4. Paragraph patterns to reuse

- **Concept paragraph:** definition → assumption → what it is good for → where it fails.
- **Choice paragraph:** the decision needed → the two pulls (too much of X loses A, too little
  loses B) → what we tried → what we chose and why.
- **Reviewed-study paragraph:** who → sample and setting → method → result with numbers → what
  the authors concluded → (if needed) how far it can be trusted.
- **Verdict paragraph:** a question the reader would ask → the answer → the condition under
  which it holds → the evidence for the condition.
- **Limitation paragraph:** the limit → why it matters for this claim → the counterweight or
  how far it moves the result.

---

## 5. Where these papers conflict with SKILL.md, and which wins

- **Roadmap paragraph.** Cobo and Bornmann both end the introduction with "This article is
  organized as follows". SKILL.md forbids signposts. In a journal paper, one short sentence
  saying how the body is organized is acceptable when the organizing principle is itself
  informative (for example, by workflow step or by research method). No other signposts.
- **Enumerations (a)...(h).** Use one only when the items are criteria the reader will meet
  again as headings or table columns. Otherwise write prose.
- **Stacked citations.** Bornmann cites up to ten studies in one parenthesis. Cite the two or
  three that carry the claim.
- **Passive and "allows us to".** Zinsser wins: active verbs, "we" as the actor.
- **Inflated words** ("deep comparative study", "great potential", "valuable reference").
  Zinsser and the anti-AI list win.

After drafting a paper, run the edit pass in `references/edit_pass.md` (moves 1-6 and 10-12). Edit the draft in place, never regenerate it.
