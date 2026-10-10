# CodeSignal General Coding Assessment: How the 70-Minute Format Actually Scores You, and How to Prepare Without Grinding 300 Problems

You got the email from a recruiter, clicked the link, and now there's a 70-minute window with four problems standing between you and a human conversation. The General Coding Assessment is not a LeetCode contest and it isn't a knowledge quiz. It's a timed execution test with a scoring model that rewards different behavior than most candidates bring to it.

This guide covers what the GCA actually is, how the 200–600 score is put together, where most people leak points, and how to prepare when you have four to eight weeks rather than four months.

---

## What the GCA actually is

CodeSignal's own documentation describes the General Coding Assessment as four questions of varying difficulty, completed in a single sitting, with 70 minutes on a shared clock. You can move between the four problems in any order and split the time however you like. You write your solution inside CodeSignal's browser IDE.

Two mechanics from the official rules matter more than most prep articles admit:

- **You must submit before leaving a task.** Not save. Submit. If you jump to question 4 to read it and come back, the rules page says the code does not persist unless you submitted it. People lose working solutions this way.
- **CodeSignal grades your highest-scoring submission per question**, not your last one. The rules explicitly note that even if your final submit has a syntax error, a higher earlier score is kept. Practically: bank a passing run early, then experiment.

Setup happens before the clock starts. You'll take a face photo, photograph an ID, and click through a list of assessment rules. If you've never used the in-browser editor, there's a Practice button on that same screen. Use it. Ten minutes of interface familiarity is cheaper than ten minutes of your assessment.

### The rule about searching that trips people up

The certified GCA allows web searches for **syntax reference only**. CodeSignal's own example: looking up which methods a C++ `queue` supports is fine. Looking up how to implement a deque is not, because that page is helping you with the solution. The same FAQ states that AI is not allowed, including as a syntax search.

Proctoring captures your camera, microphone, and screen for the duration. One thing worth knowing before you panic about it: CodeSignal states that proctoring has no impact on the score you receive, because scores are calculated automatically. It's a verification layer, not a scoring one.

---

## How the 200–600 score is built

CodeSignal retired the old 300–850 scale back in 2023. If you're reading a guide that tells you to aim for 750, close the tab. The current certified assessment score runs 200–600, and it comes with skill labels (Developing, Intermediate, Advanced, Expert) across areas like arrays, graphs, and dynamic programming.

The score is not simply "problems solved out of four." One widely circulated breakdown of the mechanics describes two layers: base points for completing questions within a module, plus bonus points that only unlock if you solve **100% of that module**. Partial credit still earns base points, but it forfeits the bonus. And the bonus allocation skews toward the harder, more discriminating questions.

That explains a pattern candidates keep running into: reaching a plateau across retakes. If you reliably clear Q1 through Q3 and stall on Q4, your ceiling is roughly the same every attempt, because the upside lives in the question you're not finishing. It also explains why "almost solved" is the worst outcome. A Q4 sitting at 90% correctness can lose you the entire bonus pool for that module.

Two more things worth internalizing:

**Speed is an official scoring factor.** CodeSignal lists correctness, speed, implementation, and problem-solving ability. That's why two candidates who both solve all four questions can end up 15 points apart.

**CodeSignal doesn't publish a pass mark.** It frames the score as a data point for employers, and each company sets its own bar. Public forum posts show candidates advancing with scores in the 500–550 band at real companies, but those are individual accounts from different roles and hiring quarters. Treat company-specific thresholds as something to check against current candidate reports, not against any static chart, including this one.

---

## What the four questions look like in practice

CodeSignal publishes average module times that add up to 75 minutes: 10 for Q1, 15 for Q2, 20 for Q3, 30 for Q4. You have 70. That mismatch is the test.

| Tier | Typical topics | Suggested budget |
| --- | --- | --- |
| Q1 (easy) | Array manipulation, string processing, basic math | 5–10 min |
| Q2 (easy/medium) | Hash maps, frequency counts, two pointers, sliding window | 10–15 min |
| Q3 (medium/hard) | Trees, BFS/DFS, 1D dynamic programming, stacks and queues | 15–20 min |
| Q4 (hard) | Graph algorithms, harder DP, simulation with dense edge cases | 20–30 min, partial credit acceptable |

Community write-ups consistently report that a clean Q1–Q3 with a partial Q4 is a strong outcome, and that a complete Q1–Q3 alone has produced scores in the 570+ range. Chasing Q4 by sacrificing Q3 is the single most common way a good attempt becomes a mediocre one.

---

## The 70-minute run

A workable sequence, adapted from the timing breakdowns circulating among candidates:

1. **Minutes 0–3: read all four questions.** Not to solve them. To decide whether Q3 or Q4 plays to your strengths, since you can attack them in either order.
2. **Minutes 3–13: lock down Q1.** Direct implementation, examples, boundary cases, submit. Don't turn the easiest question into a twenty-minute project.
3. **Minutes 13–28: finish Q2.** Convert the prompt into explicit rules, write a helper if it makes the transformation easier to verify, submit once the core behaves.
4. **Minutes 28–50: take your stronger advanced question.** Detail-heavy simulation and matrices point to Q3. Recognized DP or graph pattern points to Q4.
5. **Minutes 50–65: collect partial credit on the remaining one.** A brute force that passes the smaller valid cases beats an optimal solution you never submit.
6. **Minutes 65–70: audit.** Every intended solution submitted, debug prints gone, signatures unchanged, no unsaved work sitting in another tab.

The brute-force point deserves a caveat rather than a blanket endorsement. There's a well-known candidate account of landing 600/600 with a lightly optimized brute force on Q4. That's one data point against a documented scoring criterion that includes speed. The safe ordering is: get a correct passing solution in, then optimize if the clock allows.

---

## Retakes and reusing your score

Candidate reports and prep guides consistently describe the retake limit as two attempts per rolling 30 days and three per rolling six months. That makes an unprepared first attempt expensive.

The reuse mechanic is the other half. Several accounts describe sharing a single GCA result with a second employer instead of retaking, and six months is the validity window most often quoted. CodeSignal's public documentation doesn't spell out reuse terms clearly, so read your own invitation rather than assuming.

---

## Preparing for the pattern, not the problem set

Here's the uncomfortable part about GCA prep: volume grinding has a worse return than it does for a live interview loop. The GCA rewards fast pattern identification and clean implementation under a 70-minute ceiling. Someone who has solved 400 problems ad hoc can still burn 15 minutes on Q3 deciding which approach fits.

That's the specific gap AlgoMonster was built to close. It's a pattern-based course from ex-Google engineers, organized around roughly 48 patterns rather than a problem feed, and the structure is deliberately compact because it's designed to be finished in four to eight weeks at one to two hours a day. For someone with a CodeSignal invite already sitting in their inbox, that timeline is usually the constraint that decides the tool.

Three features map directly onto how the GCA scores you:

- **The decision flowcharts.** A decision tree of questions ("is the input sorted?", "am I tracking a contiguous window?", "is this a tree or graph?") that lands you on a pattern before you start typing. That's the skill Q1 and Q2 punish you for lacking, because spending eight minutes deciding costs you a whole tier.
- **Speedrun.** Instead of writing full code, it cycles you through problems as multiple-choice pattern and template identification. This is the closest thing to training the speed factor CodeSignal actually scores, and it covers ground far faster than full submissions.
- **The inline IDE with templates and an AI assistant.** Bug-free implementation is the other half of the score, and the platform pushes you through identify-pattern → implement → analyze time and space complexity, which is the loop a GCA question rewards.

Paid plans include the full pattern library, unlimited Speedrun, an AI assistant for explanations and debugging, and company question sets refreshed monthly. The free tier gives limited sample content, and a couple of practice lists, including Blind 75 and Monster 50, are open enough to judge whether the text-and-diagram teaching style clicks for you.

👉 [**Try AlgoMonster free before you commit to anything**](https://algo.monster?fpr=li69)

### What AlgoMonster does not do

Worth knowing before you buy, because these gaps are predictable rather than hidden:

- **No video.** Everything is text plus interactive diagrams. Readers do well here; people who learn from watching someone code should look at video-first platforms instead.
- **Around 230 problems and lessons.** The point is pattern coverage, not volume. If your gap is raw fluency, you'll want to supplement with a larger problem bank.
- **System design coverage is introductory.** Not a problem for the GCA, which doesn't test it. A real problem if you're targeting senior loops after the screen.
- **No live interviewer.** Nothing on the platform simulates a senior engineer watching you reason out loud.

---

## AlgoMonster plans and current pricing

There's no monthly option. AlgoMonster sells annual or lifetime access, and the listed prices move with promotions. Current list pricing reflects a 50% promotional discount: $99/year against a $198 standard rate, and $189 lifetime against a $378 standard rate.

| Plan | What you get | Price | Billing | Get it |
| --- | --- | --- | --- | --- |
| Free | Limited access to sample patterns and problems, plus open practice lists | $0 | No card | [Start with the free tier](https://algo.monster?fpr=li69) |
| Pro – Yearly | All patterns, lessons and problems; unlimited AI assistant; unlimited Speedrun; company question sets updated monthly; 500+ lessons across 6 courses, 1,000+ illustrations, 3,000+ editorials; member discount on live bootcamps; 12 months of access | $99/year (~$8.25/mo billed annually), standard rate $198 | Billed annually, cancel or upgrade anytime | [Get Pro Yearly at the current discount](https://algo.monster/subscribe?fpr=li69) |
| Pro – Lifetime | Everything in the annual plan, plus lifetime content updates, paid once | $189 one-time, standard rate $378 | One-time payment | [Buy Pro Lifetime and keep access](https://algo.monster/subscribe?fpr=li69) |

Bonus courses are bundled at no extra cost, including a CS fundamentals course and a build-an-LLM course. New content is added to the membership rather than sold separately.

On discount timing: a partner code (SCHELLEY) has been reported as stacking an additional 10% off the existing 50% sale, bringing yearly to roughly $89 and lifetime to roughly $170. Codes like this get retired without notice, so test it at checkout and confirm the final total before paying. If it doesn't apply, the standard promotional price is still the price.

Which plan makes sense depends on how many job searches you expect in front of you. If this is a single push with a CodeSignal deadline inside two months, annual covers it and costs less upfront. If you interview every two to three years, the lifetime plan pays for itself on the second cycle, and the lifetime option is what keeps you from paying a renewal fee the next time a recruiter emails you out of nowhere.

---

## A realistic four-week prep plan around a GCA deadline

This assumes you can already write working code in one language and your gap is pattern recognition speed, not programming fundamentals. If you're still learning what a hash map is, fix that first — pattern courses assume fluency and teach selection.

**Week 1: baseline and damage report.** Take one full 70-minute timed run before studying anything. CodeSignal's own practice assessment mirrors the interface, and AlgoMonster's Speedrun plus practice problems let you run timed sets. Record where the minutes went, specifically. "I lost time on DP" is useless; "I spent six minutes deciding whether the problem was DP or greedy" gives you something to fix.

**Week 2: cover Q1 through Q3.** Arrays and strings, hash maps and frequency counts, two pointers and sliding window, tree traversal, BFS/DFS on grids, and 1D DP. This band is where most of your achievable points live. Do not start here by memorizing Q4-grade graph algorithms.

**Week 3: timed simulation, twice.** Full sessions, same language, same browser, no pausing. Between sessions, drill only the weakness the last session exposed. Then rebuild the edge-case habit: empty input, single element, duplicates, all-zeros, maximum size. Missing one of these is how a solution drops from 100% visible tests to a partial score.

**Week 4: Speedrun and interface friction.** Rapid pattern identification under a clock, then a final full run in the actual test environment. Confirm your language's standard-library syntax so you're not burning permitted-search time on basics. Check your browser, camera, and network ahead of the day.

Add one habit that costs nothing: write down the reason for every delay during practice. Broad labels hide the fix.

---

## Test-day checklist

- Confirm deadline, time zone, and ID requirements, and re-read the rules shown for your specific invitation. Companies can configure different durations — if your invite says 90 minutes, believe the invite.
- Close every other application. Proctoring flags tab and fullscreen exits.
- Pick one language and stay in it.
- Submit before you switch tasks, every time.
- If a question stalls, leave something submitted and move on.

---

## The short version

The General Coding Assessment is a 70-minute, four-question execution test scored on a 200–600 scale where partial credit is real, speed counts, and your highest submission is the one that survives. Nobody publishes the pass mark because companies set their own. What you can control is how fast you identify the right approach and how reliably you close out Q1 through Q3.

Pattern drilling beats random problem volume for that specific goal, and a structured course with flowcharts and timed pattern recognition work fits a four-to-eight-week job search better than a raw problem bank does. If you want to see whether the approach suits how you learn before spending anything, the free tier is the cheapest way to find out:

👉 [**Start practicing on AlgoMonster for free**](https://algo.monster?fpr=li69)
