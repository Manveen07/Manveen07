### Hi, I'm Manveen

GTM engineer who builds outbound systems like software: tested before they touch a real lead, monitored after, fixed when they break.

At my day job I built an outbound agency's pipeline in Clay, n8n and Python. The visual version, with charts and the three times it broke: **[manveen.me/how-i-build](https://manveen.me/how-i-build)**

**The numbers**

- **12,030** verified emails for 15,514 decision makers, a 78% find rate
- **34,044** companies mapped in Clay for 0 data credits
- **870+** automated tests on the pipeline

**How I test, because I've seen what happens when you don't**

- Label real cases by hand before an AI step goes live. My Claygent fit check rejected all four good companies in a hand-labelled set of 25. I caught it before the 24,506-company run, and after the rewrite it lost none on 30 it had never seen.
- Replay old vs new on real history before switching. My email identity check was rejecting real people; the new rules accepted 77 more on 2,376 past emails and lost none of the old passes.
- Trace every fact in an email to a source. In a 50-agency work sample (76 two-email sequences), the check blocked two leads whose facts didn't trace, until I fixed them.
- Watch the runs after. Tender Radar (below) went red on nine mornings in October when a tender portal stopped answering and took the whole run down. Since 29 Oct each source fails on its own. [The bars](https://manveen.me/#proof)

**Code you can actually open**

- [champion-move-checker](https://github.com/Manveen07/champion-move-checker): finds past champions at their new companies and holds unsure matches for a person. 60 tests, CI green, made-up data.
- [n8n-workflow-tests](https://github.com/Manveen07/n8n-workflow-tests): four of my five test layers on a toy n8n workflow, 45 tests.
- [tender-radar-showcase](https://github.com/Manveen07/tender-radar-showcase): the public engine of Tender Radar, which reads UK public tenders every morning and says bid, maybe or skip, with the reason quoted (the schedule is off in this copy).

**Writing:** [149 tests for a few Slack buttons](https://manveen.me/writing/149-tests-for-a-few-slack-buttons) · [How I caught my own AI test cheating](https://manveen.me/writing/schema-as-eval-spec) · [Marking the AI's homework](https://manveen.me/writing/marking-the-ais-homework) · [Things AI got confidently wrong](https://manveen.me/writing/things-ai-got-confidently-wrong)

Day-job code and client data stay private; I'm happy to walk through it on a call. New Delhi, working remotely. [manveen9650@gmail.com](mailto:manveen9650@gmail.com) · [LinkedIn](https://www.linkedin.com/in/manveen-singh-b9b7672a0)

<img src="n8n-testing-explained.png" alt="How I test an n8n workflow before it goes live: 149 tests across five layers" width="100%">
