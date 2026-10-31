### Hi, I'm Manveen

I build LLM systems and the evals that keep them honest. Where I've measured it, each one says how often it's wrong, and how I found out.

**LLM systems, and how often they're wrong**

- **[Tender Radar](https://github.com/Manveen07/tender-radar-showcase)**: an LLM sorts UK public tenders into bid, maybe or skip, with the reason quoted from the notice. It has started on its own every morning since July. Once, 12 of 12 tests passed while the morning run crashed for three weeks, because no test opened the new files. So now I watch the runs, not just the tests: [the bars](https://manveen.me/#proof), red when one fails. In October, nine mornings failed when a tender portal stopped answering; since 29 Oct each source fails on its own.
- **Drawing reader** (code private): Gemini reads engineering drawing PDFs into a quote sheet, and every value carries the exact text it came from. On 23 hand-checked drawings it got 7 values wrong out of 419. All 7 quoted real text from the sheet, so a quote proves the text exists, not that it went in the right box. [Marked like homework](https://manveen.me/writing/marking-the-ais-homework)
- **My eval that cheated** (leadlens, code private): my AI judge caught all 11 fake AI jobs in my test, because my own notes in the test data were giving it the answers. With the notes gone it caught 9 of the 11 fakes, still with no false alarms, on the same 72 postings. A later audit found two more leaks (two of the judge's worked examples were among the 72, and it could see the classifier's verdict), so the 9 needs a re-run too. [The write-up](https://manveen.me/writing/schema-as-eval-spec)
- **AI receptionist** (code private): answers calls and books appointments; in the live voice version the model calls a booking tool and a callback tool itself. Plain-code graders fail any call that invents a price, books outside opening hours or books an emergency instead of passing it on, and a second AI plays the difficult callers.

**Also on here**

- [champion-move-checker](https://github.com/Manveen07/champion-move-checker): rules, no model. It finds people who changed jobs and holds the unsure matches for a person. Its release gate blocks the naive same-name matcher (8/29 right), and three blind test sets, each written by a separate agent that never saw the code, failed the gate on their first run; the raw logs are in the repo. 60 tests, CI, made-up data.
- [transformer_trained-on-text](https://github.com/Manveen07/transformer_trained-on-text): a small character-level GPT I wrote in PyTorch to learn how Transformers work, following Karpathy's Let's build GPT lecture.
- [n8n-workflow-tests](https://github.com/Manveen07/n8n-workflow-tests): 45 tests on a toy n8n workflow, the way I test the real ones.

By day I build GTM systems in Clay, n8n and Python. How I build them: [manveen.me/how-i-build](https://manveen.me/how-i-build)

New Delhi, working remotely. [manveen9650@gmail.com](mailto:manveen9650@gmail.com) · [LinkedIn](https://www.linkedin.com/in/manveen-singh-b9b7672a0) · [manveen.me](https://manveen.me)
