# Playbook: Brand-New X Account — 14-Day Foundation Protocol

## Purpose

This is a **14-day operating protocol** for a brand-new account with little or no audience history.

The goal is not to promise a follower number. The goal is to create a clean baseline, establish a recognizable niche, produce enough original content to measure, and participate meaningfully in the audience the account wants to reach.

After Day 14, keep, modify, or reject parts of the protocol based on the account's own results.

## Evidence Status

### Verified from the public X algorithm

The current public `xai-org/x-algorithm` code shows that the For You ranking system uses predicted actions including replies, reposts, shares, follows, dwell-related signals, and negative actions such as reports, mutes, blocks, and "Not interested."

The current public defaults also include:

- a positive reply weight
- an additional bidirectional-follow reply boost
- positive weights for quote posts, shares, DM shares, copy-link shares, and following the author
- strong negative weights for reports, mutes, blocks, and "Not interested"
- cold-start-related parameters for lower-impression posts/accounts
- candidate-age limits in parts of retrieval

Primary references:

- `home-mixer/params/param.rs`
- `home-mixer/scorers/value_model.rs`
- upstream `README.md`

These facts **do not prove** a specific posting frequency, reply quota, follower-growth target, or ideal time between posts.

### Experimental operating assumptions

The actions below are our protocol, not claims about hidden X rules:

- a narrow topic identity should make the account easier for people to recognize
- useful replies can help expose the account to relevant communities
- one strong original post is preferable to several weak posts
- consistent measurement is more useful than chasing raw likes
- repeated spammy behavior and templated replies should be avoided

## Before Day 1

Write down:

- account handle
- niche
- one-sentence account promise
- primary audience
- 3 content pillars
- starting follower count
- starting following count
- website / CTA if one exists

Do not change the niche during the 14-day test unless the original positioning is clearly unusable.

## Account Positioning Rule

Use **one primary niche** and no more than **three content pillars**.

Example:

```
Primary niche:
AI security

Content pillars:
1. Agent security incidents
2. Technical explanations
3. Security experiments
```

A visitor should understand what the account is about within a few seconds.

## Daily Protocol

### 1. Relevant engagement — 30 to 45 minutes

Find conversations inside the target niche and write **8–12 useful replies**.

This reply count is an experimental workload target, not an X requirement.

A useful reply should do at least one of these:

- add a fact
- add technical context
- explain a mechanism
- provide a counterexample
- connect the topic to another useful idea
- ask a specific question that moves the conversation forward
- share a relevant first-hand test or experience

Avoid:

- "great post"
- generic praise
- repeated templates
- copy/paste replies
- unrelated promotion
- dropping a link with no explanation

### 2. Original content — up to 1 post per day

During the first 14 days, publish **0–1 original posts per day**.

Use one of four formats:

1. **Discovery** — something worth knowing
2. **Explanation** — explain why or how something works
3. **Evidence** — show a result, source, test, or artifact
4. **Build** — show something you created and what was learned

Do not post only to satisfy a quota.

### 3. Conversation follow-through

When somebody gives a real reply:

- answer when you have something useful to add
- continue the technical or substantive conversation
- do not manufacture reply chains
- do not treat every response as an opportunity to promote yourself

## 14-Day Sequence

### Days 1–3 — Establish the identity

- finalize bio and account promise
- identify 15–25 relevant accounts to learn from and engage with
- write useful replies each day
- publish up to one original post each day
- begin tracking every original post

### Days 4–7 — Establish a baseline

Continue the daily protocol.

By the end of Day 7, calculate performance by post format.

Do not declare a winning format from a single post.

### Day 7 Review

For each original post record:

- format
- impressions
- replies
- reposts / quotes
- shares if available
- profile visits if available
- follows if attributable / available
- link clicks if relevant

Calculate when possible:

```
Reply rate      = replies / impressions × 1,000
Share rate      = shares / impressions × 1,000
Profile rate    = profile visits / impressions × 1,000
Follow rate     = follows / impressions × 1,000
```

### Days 8–13 — Test what looked promising

- keep the same niche and pillars
- repeat the strongest 1–2 formats
- test new hooks or presentation while keeping the subject comparable
- continue useful replies
- keep recording results

### Day 14 — Decision

Sort tactics and formats into:

```
DOUBLE DOWN
KEEP TESTING
MODIFY
STOP
```

A tactic should normally be tested more than once before it is rejected.

## What Success Looks Like After 14 Days

Success is not a predetermined follower number.

Look for evidence that:

- impressions are becoming more consistent
- some post formats repeatedly outperform others
- relevant people are replying
- relevant people are following
- profile visits are increasing
- the account has begun developing repeat engagers
- you can identify what to publish next without guessing

Follower growth is useful, but it should be interpreted alongside the quality of the audience and the per-impression metrics.

## Guardrails

- Do not buy followers, replies, reposts, or engagement.
- Do not mass-reply with templates.
- Do not coordinate blocks, reports, or fake engagement.
- Do not present public ranking weights as raw engagement-count equivalents.
- Do not claim this protocol guarantees distribution.
- Keep verified algorithm facts separate from experimental growth tactics.

## End-of-Test Question

At Day 14 ask:

> Did this protocol produce a clearer account identity and measurable improvement in qualified engagement compared with the starting baseline?

If yes, run a second 14-day cycle with the winning formats.

If mixed, modify one variable at a time.

If no, revisit positioning before increasing posting volume.
