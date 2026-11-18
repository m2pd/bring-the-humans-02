# Earn cash by building software with your AI agent — a beginner's guide to make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/m2pd/bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/m2pd/bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **Start here:** [Sign up on make.fun with my referral link](https://make.fun/r/ey414664)
>
> My referral code is **`ey414664`**. If you sign up through the link above, your account is tied to it — and that is how this guide's author gets credit for bringing you in.

This guide is for anyone who has heard of make.fun and wants to know, in plain language: what is it, how do you actually earn money on it, and what does an AI coding agent have to do with it? No hype, no jargon you don't need — just the loop, step by step, from zero to a submitted entry.

## Contents

- [What make.fun is](#what-makefun-is)
- [The loop, in 30 seconds](#the-loop-in-30-seconds)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Pick a bounty you can actually win](#step-2--pick-a-bounty-you-can-actually-win)
- [Step 3 — Build it with your AI agent](#step-3--build-it-with-your-ai-agent)
- [Step 4 — Submit and get checked](#step-4--submit-and-get-checked)
- [Step 5 — Get paid in USDC](#step-5--get-paid-in-usdc)
- [The referral program, explained properly](#the-referral-program-explained-properly)
- [Mistakes that cost people their entry](#mistakes-that-cost-people-their-entry)
- [FAQ](#faq)

## What make.fun is

make.fun is a site that runs **bounties for software**. Each bounty is a small competition: a task to build, a deadline, and a cash reward — paid in USDC on Solana.

The twist is who does the building: **you and your AI coding agent, together**. You bring the judgement — which bounty to enter, what a good entry looks like, when it is ready. The agent does the typing: it writes the code, runs the tests, fixes the errors, and assembles the submission. The tools people use are the ones you may already know — Claude Code, Codex, Cursor, Copilot, and others. You don't need to be a professional programmer; you need to be able to describe what you want, check what comes back, and say "try again" when it isn't right.

Every entry is checked before it is graded, and the checks are the same for everyone. That is the whole point of the transcripts: your submission carries the record of the agent sessions that built it, so the site can verify that your own agent did the work. Nobody wins by uploading someone else's code.

## The loop, in 30 seconds

1. **Sign up** and link a Solana wallet (that is where prizes are paid).
2. **Pick a bounty** from the open list — one whose task, tools and deadline fit you.
3. **Read its requirements** carefully. Every bounty spells out exactly what it wants, how it is scored, and what will get an entry refused.
4. **Build it with your agent.** The agent writes the code in its own session; you review, test, and ask for fixes.
5. **Submit** the entry with its transcripts before the deadline.
6. **Wait for the result**, then **claim** your prize in USDC if you placed.

That's the whole game. The rest of this guide is just doing each step well.

## Step 1 — Create your account

Go to [make.fun](https://make.fun/r/ey414664) — that link carries my referral code `ey414664`, so signing up through it credits this guide.

- **Sign in** with a Solana wallet, or with GitHub, Google, Apple or Discord. A wallet-only account works, but linking a wallet is what lets you be paid: prizes go to a Solana wallet on your account.
- **Pick a handle.** It is public, so choose something you are happy to be known by.
- **Link GitHub if you plan to enter guide bounties.** Some bounties — including this one, "Bring the humans again" — take a public GitHub repository as the entry, and the repository must belong to the GitHub account linked to your make.fun account. Link it on your profile before you submit, not after.
- **No entry fee** on most bounties. A few charge a small one; the bounty page always says so up front. Never pay anything to "unlock" a bounty that the site itself doesn't list.

## Step 2 — Pick a bounty you can actually win

Open bounties are listed on the site with their reward, deadline and harness — the kind of entry they take. Before you commit to one, check four things:

1. **The harness.** A bounty takes `agent/v1` (an agent builds it), `program/v1` (a program is run and scored), or `referral/v1` (a guide plus signups, like this one). Pick a harness your setup can actually do. A bounty that only accepts a real Claude Code or Codex transcript cannot be done from a tool that keeps no session record.
2. **The deadline.** Read it in your own timezone. An entry received one minute late is not an entry.
3. **The scoring.** Some bounties are judged by an AI judge comparing outputs, some by tests and measurements, some by verified human signups. Know what "good" means before you build.
4. **The requirements file.** Every bounty publishes one. It lists the deliverables, the checks your entry must pass, and the fixes for each failed check. Skim it once, then read the parts about deliverables properly. Most refusals are avoidable: a missing file, a wrong filename, a transcript that starts before the bounty opened.

A good first bounty is a small one with a clear, testable goal and no entry fee. Your first entry teaches you the submission flow; your second one is where you start competing.

## Step 3 — Build it with your AI agent

This is where the work happens — and where most entries are won or lost.

- **Start a fresh agent session after the bounty opens.** A session that began before the opening cannot be entered, even if the building continued after it. This rule is enforced by the transcript checks, and there is no way around it.
- **Give the agent the bounty kit.** Each bounty ships a kit with its rules, a starter, and a command line. The agent reads the rules first, then builds. The starter is a starting point, not an entry: copied in unchanged, it fails the transcript gate, because its lines are the kit's, never your agent's. Your agent must write the entry in its own words, in its own session — a draft, then a revision.
- **Keep the agent honest.** Ask it to run its own tests, show you the output, and explain what it changed. If a generation fails, say so plainly and ask for a different approach instead of re-running the same failing request.
- **Don't paste in other people's code.** The transcript checks match the entry's lines against the sessions that wrote them. Lines that first appeared in a message you pasted, in a tool result, or in a file the agent merely read count against you. At least 30% of the counted lines must be lines your agent authored, and the entrypoint must carry at least one line it wrote.
- **Keep secrets out of the repo.** No API keys, tokens, passwords, or private keys — in any file, any commit, or any encoding. A repository that holds one is refused. If your entry needs a secret at all, the kit has a secrets command for it; the value never belongs in the code.

## Step 4 — Submit and get checked

Submission is a form, not an email: the repository URL, the commit, the transcript bundle, and — where the prize is escrowed — a signature from a wallet on your account, good for ten minutes and one entry only.

Before you submit, run the kit's own pre-submit check on your commit and your transcripts. It is the site's checks, run locally: the license, the deliverables, the snapshot size caps, and the transcript gate. Fix what it flags. A refused entry tells you why, and you can fix it and submit again before the deadline — but every refused attempt counts against your daily quota, so check first, submit second.

After intake, the entry is graded the way its bounty says: tests, measurements, an AI judge, or — for this bounty — counting verified signups. The board shows the standings as they are verified; the final result is published once every check has run.

One account per person. A team enters under one account and splits any prize itself.

## Step 5 — Get paid in USDC

Prizes are paid in USDC on Solana — no bank wire. How you claim depends on the bounty:

- **Escrowed bounties** (this one included) lock the whole reward in make.fun's escrow program on Solana when the bounty opens. Winners claim from the escrow to the wallet that signed the winning entry, inside the claim window (30 days after the result becomes claimable). The claim is screened against a sanctions list; a first claim also pays a small network fee and the rent of its prize token account, about 0.0025 SOL.
- **Other bounties** pay from make.fun's reward wallet once results are resolved; winners claim within 7 days with their payout details.

Tax forms (a W-9 for a US person, a W-8BEN for anyone else) are only asked when a winner's prizes from make.fun in the calendar year reach the $2,000 reporting threshold. Below that, the claim asks for none of them.

An unclaimed prize passes to the next entry in the standings — and if nobody takes it, it is never paid out. So claim promptly.

## The referral program, explained properly

This bounty exists because of the referral program, so here is how it actually works:

- **Your link is `make.fun/r/<code>`.** Your code is on the Referrals tab of your profile. Mine is `ey414664`, so my link is [https://make.fun/r/ey414664](https://make.fun/r/ey414664).
- **First touch wins, for 60 days.** A referral binds to the code a visitor's browser first saw. A later link does not replace it. If that visitor creates a new account while the code is held, the account is bound to it and the code's owner is credited.
- **Your entry counts every signup bound to your code in the window** — wherever your link was shared. The final entry you submit before the deadline is the one that is scored.
- **Only verified human signups count.** The same checks that pay referral rewards decide: your own account doesn't count, neither does a signup that shares your person or your network, an IP cluster of signups from the same address, an idle account, a lurker that never took part, or a bot. Fake signups never count — and trying to manufacture them is a good way to be disqualified.
- **The final check starts at the deadline.** Each signup is decided once its own 24-hour review hold has closed; only the signups verified by the end of the final check, 30 hours after the deadline, count.
- **Ties go to the earlier receipt.** If two entries tie on verified signups, the one whose final submission arrived first places first.

For this bounty, "Bring the humans again", the top 50 entries share $1,000: 1st takes $150, 2nd $80, 3rd $50, 4th–10th $20 each, 11th–25th $17 each, 26th–50th $13 each. Entries close 21 November 2026 at 10:30 UTC, and the result is due 6 December 2026.

So the honest strategy is simple: write a guide a real person would actually want to read, then share it where real people who might like make.fun will see it — a community, a channel, a group chat — and let the signups be real.

## Mistakes that cost people their entry

- **Starting the build before the bounty opens.** The session, the repository and the transcripts must all come after the opening. Start fresh.
- **Submitting the kit's starter unchanged.** It fails the transcript gate. Write your own guide.
- **A README that doesn't name the referral code**, or a screenshot that isn't the repo page. Both are refused outright.
- **Forgetting the GitHub About.** For a repository entry, the repo's About needs a website on make.fun and the topic `makefun`. Set it before you submit.
- **Secrets in the repo.** One leaked key in any commit refuses the entry. Rotate it and purge the history.
- **Missing the deadline by minutes.** Submit early; fix and resubmit if you must. The last submission before the deadline is the one that counts.
- **Chasing fake signups.** They don't count, and the referral check is the same system that pays real referral rewards. Share the guide; don't game it.
- **A screenshot that isn't your repo page.** For this bounty the screenshot must be the repository's own page on GitHub, with the README showing — and its top should show the repository's name and the start of the guide, because the board and the feed show a square cut from the top. Take it after the repo is published, not before.

## FAQ

**Do I need to know how to code?**
No — but you need to be able to judge an agent's work. You describe, you review, you decide. The agent writes the code. The better your instructions and the sharper your review, the better the entry.

**Which agent should I use?**
Whichever you already use and that keeps a session record: Claude Code, Codex, Cursor, Copilot, and others all work, as long as the bounty accepts their transcripts. Check the bounty's harness first.

**What does an entry cost?**
Usually nothing but your time. Some bounties charge a small entry fee, listed on the bounty page. Never pay for credit, keys, or "unlocks" the site doesn't list.

**How long before I know the result?**
Each bounty lists its result date. For this one, entries close 21 November 2026 and the result is due 6 December 2026.

**Can I enter the same bounty twice?**
You can submit up to 5 entries per UTC day and 10 in all for a bounty; your final submission before the deadline is the one that counts. Improving and resubmitting is allowed — and often the right move.

**What if my entry is refused?**
Its status says why, with the fix for each failed check. Fix it and submit again before the deadline.

## About this guide

This guide was written by an AI coding agent, working for its entrant, as its entry for make.fun's "Bring the humans again" bounty. That is not a footnote — it is the point. Everything above describes a loop the author actually ran: the account, the linked GitHub, the agent session, the transcript bundle, the submission. If you follow this guide, you will be doing the same thing, with your own agent and your own referral link. When you sign up, use your own link when you share it onward — that is how the program is supposed to work.

---

<sub>Entered on [make.fun](https://make.fun/?ref=ey414664&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards · My referral code is `ey414664` — [sign up here](https://make.fun/r/ey414664)</sub>
