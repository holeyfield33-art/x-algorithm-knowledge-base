# Playbook: Small AI-Security Account — 14-Day Dogfood Protocol

**Primary dogfood account:** @1Aihub  
**Niche:** AI security / agent security / LLM and agent vulnerabilities

## Purpose

This protocol turns the public X ranking architecture into a **measurable 14-day operating experiment** for a small AI-security account.

It does not promise a follower count and does not claim to reproduce X's internal ranking score.

The objective is to learn which combination of content, conversations, and positioning produces more **qualified engagement and relevant followers** for this specific account.

## Evidence Status

### Verified from the public X algorithm

As of the current upstream sync, the public `xai-org/x-algorithm` defaults include:

- `ReplyWeight = 5.0`
- `BidirectionalFollowReplyWeightBoost = 15.0`
- `QuoteWeight = 5.0`
- `FollowAuthorWeight = 4.0`
- `ShareViaDmWeight = 5.0`
- `ShareViaCopyLinkWeight = 20.0`
- `FavoriteWeight = 0.5`
- negative weights for reports, mutes, blocks, and "Not interested"

These weights multiply **predicted probabilities**, not raw engagement counts.

Primary references:

- `home-mixer/params/param.rs`
- `home-mixer/scorers/value_model.rs`
- `docs/SCORING_WEIGHTS.md`

### Experimental assumptions we are dogfooding

The following are FeedFit-style hypotheses, not claims made by X:

- niche consistency can improve audience recognition
- useful replies can create discovery opportunities inside the right community
- technical reference material may generate more high-intent sharing than generic commentary
- repeated original formats make it easier to compare performance
- qualified followers matter more than raw follower count
- one strong post per day is enough to run the first experiment

## @1Aihub Positioning

For this 14-day test, keep the public identity narrow.

### Primary identity

**Agent security intelligence and research**

### Content pillars

1. **Agent Security Incidents**  
   Real-world failures, disclosures, vulnerabilities, escapes, supply-chain events, and agent misuse.

2. **Agent Security Research**  
   Explanations, taxonomy questions, experiments, architecture, attack paths, mitigations, and evidence.

3. **Building ASI**  
   Useful behind-the-scenes work on the Agent Security Index when it teaches the audience something.

Avoid turning the account into a general feed for every project or business idea during the experiment.

## Four Post Formats

Tag every original post with one of these categories in the tracking sheet.

### DISCOVERY

Surface an important development.

Structure:

```
What happened
→ why it matters
→ what is still unknown
```

### EXPLANATION

Teach a mechanism.

Structure:

```
Claim / question
→ mechanism
→ concrete example
→ takeaway
```

### EVIDENCE

Show evidence rather than only opinion.

Structure:

```
Finding
→ source / test / artifact
→ interpretation
→ limitation
```

### BUILD

Use build-in-public only when there is a lesson.

Structure:

```
What changed
→ problem it solves
→ what you learned
→ artifact if useful
```

"Worked on ASI today" is weak.

"ASI kept classifying these two incidents together, so I changed the evidence model; here's the distinction" is useful.

## Daily Protocol

### Session A — Intelligence capture

Spend a short block reviewing material you are already researching.

Capture **1–3 possible post ideas**.

Do not create extra research solely to satisfy X.

### Session B — One original post

Publish **one strong original post per day when you have one**.

If there is no worthwhile post, skip it rather than publishing filler.

Rotate formats across the first week so we have something to compare.

Suggested first-week sequence:

```
Day 1  DISCOVERY
Day 2  EXPLANATION
Day 3  EVIDENCE
Day 4  BUILD
Day 5  DISCOVERY
Day 6  EXPLANATION or EVIDENCE
Day 7  strongest format so far
```

This rotation is experimental, not an X rule.

### Session C — Relevant replies

Write **8–12 substantive replies per day** across relevant conversations.

This is our dogfood workload target.

Prioritize:

- agent-security researchers
- AI red-teamers
- security engineers
- agent framework builders
- AI infrastructure developers
- vulnerability researchers
- founders building agentic systems

A reply counts as substantive if it adds at least one of:

- technical context
- evidence
- an attack-path observation
- a mitigation
- a useful disagreement
- a concrete example
- a first-hand experiment
- a sharp technical question

Do not optimize for the follower count of the account you reply to. Optimize for relevance and conversation quality.

### Session D — Follow-through

Respond to real replies on your own posts when you can add value.

If a useful conversation emerges, continue it.

Do not force reply loops.

## Network Map

During the 14-day test, build a working list of approximately:

```
10 established AI/security accounts
15 peer-sized accounts
10 emerging accounts
10 builders / potential ASI users
```

These numbers are organizational targets, not algorithm requirements.

The goal is to stop randomly browsing X and deliberately spend time around the community @1Aihub wants to serve.

## Post Readiness Check

Before publishing, score each statement Yes / No:

- Is this clearly about one of the three content pillars?
- Does the first sentence give the target reader a reason to continue?
- Is there a concrete fact, mechanism, artifact, or insight?
- Would a technical reader learn something?
- Is there a reason somebody might reply, quote, save, or send it?
- Does the post say more than "this happened"?
- Can I support factual claims if challenged?

If fewer than **5 of 7** are Yes, revise or skip the post.

This is our editorial gate, not X's ranking formula.

## Measurement

Record every original post.

Minimum columns:

| Field | Description |
|---|---|
| Date | Publication date |
| Format | Discovery / Explanation / Evidence / Build |
| Topic | Main subject |
| Impressions | X impressions |
| Replies | Replies |
| Reposts / Quotes | Visible amplification |
| Shares | If available |
| Profile visits | If available |
| Follows | If attributable / available |
| Link clicks | If relevant |
| Notes | What was unusual |

Normalize performance when possible:

```
Replies per 1K impressions
Shares per 1K impressions
Profile visits per 1K impressions
Follows per 1K impressions
Link clicks per 1K impressions
```

Raw totals alone can be misleading when impressions vary.

## Day 0 Baseline

Before starting, record:

- current follower count
- following count
- impressions for the last 10 original posts
- replies for the last 10 original posts
- reposts / quotes for the last 10 original posts
- profile visits if available
- link clicks if available

Also label those previous posts by approximate format where possible.

That gives us a pre-protocol comparison.

## Day 7 Review

Do not redesign the system yet.

Identify:

- highest median-performing format
- topics producing the best replies
- posts producing relevant new followers
- replies that generated profile discovery or new relationships
- obvious off-topic posts that underperformed

Choose **one thing** to improve for Week 2.

Examples:

- stronger opening lines
- more evidence posts
- narrower incident coverage
- more diagrams/screenshots
- better follow-through on replies

## Days 8–13

Keep the account positioning fixed.

Run the same protocol while applying the single Week-2 improvement.

Repeat promising formats rather than introducing five new strategies.

## Day 14 Review

Classify each tactic:

```
DOUBLE DOWN
KEEP TESTING
MODIFY
STOP
```

For original post formats, prefer comparing medians or repeated results rather than declaring a winner from one viral or dead post.

## 14-Day Success Criteria

We are looking for directional evidence, not a guaranteed follower target.

A successful first cycle should leave us with:

- clearer topic consistency
- at least one repeatable post format
- measurable per-impression engagement data
- more relevant conversations
- evidence about which topics cause people to follow or visit the profile
- a small list of repeat engagers or mutual connections
- enough data to design Cycle 2

Follower growth is part of the result, but **quality and repeatability matter more than a raw number**.

## What We Are Explicitly Not Testing Yet

To keep the experiment clean, do not add:

- paid promotion
- engagement pods
- automated replies
- mass following
- multiple posts per hour
- unrelated viral-content experiments
- a new X automation SaaS
- a complicated posting scheduler

Dogfood the manual protocol first.

## Final Dogfood Question

At the end of Day 14:

> Did @1Aihub improve qualified reach, relevant engagement, or follower conversion enough to justify another 14-day cycle?

If yes, Cycle 2 doubles down on the strongest post formats and conversations.

If results are mixed, change **one major variable** and retest.

If the account shows no meaningful improvement, revisit positioning and content usefulness before increasing volume.
