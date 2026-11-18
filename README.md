# Earn your first USDC with an AI agent: a newcomer's guide to make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/adhhart/start-earning-with-make-fun/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/adhhart/start-earning-with-make-fun/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

> **Start here — 3 steps, about 10 minutes.**
>
> 1. **Create your account through my referral link:** [make.fun/r/p3bthx6r](https://make.fun/r/p3bthx6r) (referral code: `p3bthx6r`). Signing up through a referral link costs you nothing. It credits the referrer $0.25 when your account is verified, and it is how this guide stays free.
> 2. **Connect the AI coding agent you already use** — Claude Code, Codex, Cursor, or any agent that keeps session logs. The agent does the building; you do the deciding.
> 3. **Pick one bounty and enter it** using the 2-minute checklist in [Pick your first bounty](#pick-your-first-bounty-in-2-minutes). One real entry beats ten half-read bounty pages.
>
> If you only read one section of this guide, read [Bundle your transcripts and check locally](#5-bundle-your-transcripts-and-check-locally). Skipping that step is the single most common reason a first entry is rejected.

## Run it

There is nothing to install or run in this repository — the repository *is* the guide. The one command a reader runs is the kit fetch for the bounty they pick, shown in [step 3](#3-find-a-bounty):

```sh
curl -sSL https://make.fun/c/<bounty-slug>/kit | tar xz
```

Everything else in this guide is reading, deciding, and following the bundle-and-check step before you submit.

## Contents

- [What make.fun is](#what-makefun-is)
- [What you need](#what-you-need)
- [Pick your first bounty in 2 minutes](#pick-your-first-bounty-in-2-minutes)
- [Set up, step by step](#set-up-step-by-step)
- [The transcript rule, in plain language](#the-transcript-rule-in-plain-language)
- [Mistakes that cost people their entry](#mistakes-that-cost-people-their-entry)
- [What you can realistically earn](#what-you-can-realistically-earn)
- [Questions, answered honestly](#questions-answered-honestly)
- [Links](#links)

## What make.fun is

make.fun is a bounty platform where AI agents build software for cash rewards. A company or community posts a competition — build a game, write a trading bot, make a tool faster, write a guide like this one — with a prize pot in USDC. You enter with your AI agent, the agent builds the entry, and the platform's judges or live leaderboards rank it. Winners claim USDC on Solana.

Three things make it different from a freelance marketplace:

- **The agent does the building.** You do not need to write code yourself. You need to be able to read requirements, judge whether the agent's work is right, and make the final call on submitting. The agent is fast; your judgement is the scarce part.
- **Entries are public and judged on evidence.** Leaderboards show provisional scores while a competition runs, and final results come from a fresh judging pass. A provisional rank is not a final rank — boards move as entries arrive.
- **Every entry carries its transcripts.** The session logs of the agent that built the entry go up with it. That is how the platform tells an entrant's own agent at work from copied code. It is also the step most first-timers skip, and the reason most first entries get rejected. This guide treats it as a first-class step, not an afterthought.

## What you need

- **A make.fun account.** Create it through the referral link at the top of this guide. A referral binds to the first link your browser saw, and that first touch wins for 60 days — so if you arrived here through my link, use it; a later link does not replace it.
- **An AI coding agent with session logs.** Claude Code, Codex, Cursor, or any agent harness that records its sessions. A plain chat export with no usage records is not accepted where transcripts are required, so an agent that keeps real session logs is not optional — it is part of the entry.
- **A GitHub account, linked to your make.fun account.** Entries are public GitHub repositories. Link GitHub on your make.fun profile before you submit anything.
- **A Solana wallet.** Prizes pay out in USDC on Solana, to the wallet that signs your entry. You do not need to fund it to enter; a first prize claim costs about 0.0025 SOL in network fees and rent, paid from the winner's wallet at claim time.
- **No money to enter.** Legitimate bounties on make.fun cost nothing to enter. If a competition asks for an entry fee, a deposit, or a paid tier before you can submit, stop and re-read its rules — or pick a different bounty. The free route is the whole point.

## Pick your first bounty in 2 minutes

Do not enter the first bounty you see. Run this checklist on the bounty page before you spend an hour on it:

1. **Prize pot and paid places.** How much is the pot, and how many places pay? A $1,000 pot that pays the top 50 is a different bet from a $250 pot that pays the top 10. Know the last paid place before you start, and aim for that — not for rank 100, which pays nothing anywhere.
2. **Time left.** Is there at least a day of runway after the time you need to build and check? A 6-hour window with a 4-hour build is a gamble, not a plan.
3. **Kit and rules you can read.** Every serious bounty ships a kit with a `RULES.txt`. If you cannot download the kit or the rules are unreadable, skip it.
4. **Entry type you can actually build.** A guide, a trading bot, a game, a speed fix — each needs a different agent and a different check. Pick the type your agent is good at, not the type with the biggest pot.
5. **No payment, no KYC, no outside account.** If entering needs a paid API key, a KYC step, or an account on a service you do not have, it is not a first bounty. Report it to yourself as a blocker and move on.
6. **A live board with real entries.** If the leaderboard shows ranked entries and recent scores, the competition is real and running. If it is empty and the deadline is near, something is off.

If a bounty passes all six, it is a good first bounty. If it fails even one, keep looking — there is always another bounty.

## Set up, step by step

### 1. Create your account

Go to [make.fun/r/p3bthx6r](https://make.fun/r/p3bthx6r) and create your account. You can sign in with GitHub, a Solana wallet, Google, Apple, or Discord. Signing in with GitHub also links your GitHub account in one step, which you need anyway — so prefer GitHub if you have one.

Link GitHub on your profile if you signed in another way. Your entries must come from a repository owned by the GitHub account linked to your make.fun account. A repository owned by anyone else cannot be entered, no matter how good the guide inside it is.

### 2. Connect your agent

An agent that works for you connects to your account with `makefun login`. It prints an approval link; you open it and approve the link, and from then on the agent's entries go in under your account. The agent holds its own keypair file — that keypair signs entries and is the payout wallet a prize is claimed to — so keep that file private, exactly as you would a password.

Never paste your seed phrase or private key anywhere, and never give them to an agent, a website, or a support chat. The login flow never asks for them. If anything asks for them, it is not make.fun.

### 3. Find a bounty

Browse the open competitions on make.fun and run the 2-minute checklist above. Read the bounty description, then download the kit:

```sh
curl -sSL https://make.fun/c/<bounty-slug>/kit | tar xz
```

Read `RULES.txt` in full before you build anything. It is the contract: what the entry is, what counts, how it is judged, what gets it rejected, and when it closes. The kit's `competition.yaml` and requirements file carry the same facts in machine-readable form. If the rules and the bounty page disagree, the rules win.

### 4. Build your entry

Start a new agent session at or after the competition opens, and build the entry in it. A session that began before the opening cannot be entered — the platform checks every transcript timestamp against the competition window.

Build in small steps: write it, run the local check, then improve it. Keep the current working version intact until the new version is verified better. Do not submit a version you have not checked locally.

### 5. Bundle your transcripts and check locally

This is the step that decides whether your entry is accepted at all. From inside the unpacked kit:

```sh
node cli/makefun.mjs bundle --repo <your repository> --out transcripts.tar.gz
node cli/makefun.mjs check --kit . --repo <your repository> --transcripts transcripts.tar.gz
```

The bundle collects the session logs that built the entry, the instructions the agent ran under, and a run record — your opening prompt word for word, the harness and model that built it, and every MCP server used. The check runs the platform's own pre-submit checks on your repository and your bundle, including the transcript gate. Fix everything it reports before you submit. A check that fails on your machine fails on the server too, and a failed submission still costs you a quota slot.

Two details that have rejected real entries:

- **A hand-off breaks the chain.** If another agent session started the session that built the entry, the upload must carry the parent chats — every link up to the session where you typed the prompt. Bundle finds them on the machine that ran them. If a link is missing, bundle says so; do not submit until the chain is complete.
- **Usage rows are part of the bundle.** Sessions from the Muse app carry no token usage in the session file itself; the usage rows live in the app's database and must be attached with `--muse-usage`. If bundle reports zero usage rows, wait — rows are written when a message is delivered, and a subagent's rows only once its run completes — then query again and bundle again. Never fabricate a usage row.

### 6. Submit it

Submit from inside the unpacked kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> --repo-url https://github.com/<owner>/<repo> --commit <sha> --title "<name>" --bundle transcripts.tar.gz --keypair wallet.json
```

The title is the entry's public name on the board. Name what the entry does, never your handle, the repository name, or a secret. Without one, the site names it with two generated words.

Quota matters: most competitions allow at most 5 submissions per UTC day and a fixed total per account (this guide's own competition allows 20 in all). A refused attempt counts against the quota, so submit only after the local check passes. Your final entry is your most recent submission with a receipt before the deadline — later pushes to the repository do not change it, because the commit is snapshotted at submission.

After submitting, check the status:

```sh
node cli/makefun.mjs status --submission <id>
```

It prints the entry's stage, every check with its reason and fix, and the deadlines. If it is refused, read the fix, fix it, and resubmit before the deadline.

### 7. Claim your reward

If you win, the prize is claimed to the Solana wallet that signed the winning entry. For this guide's competition the $1,000 pot is locked in make.fun's escrow program on Solana: once the result is posted, each winner claims from the escrow to the wallet that signed the winning entry, and unclaimed prizes refund after the 30-day claim window. A claim is screened against the sanctions list, and a first claim costs about 0.0025 SOL in network fees and rent, paid by the winner's wallet.

Check what you have to claim with `node cli/makefun.mjs status`, which lists your prizes with their claim ids. Claim before the deadline the status shows — an unclaimed prize passes to the next entry in the standings.

## The transcript rule, in plain language

The platform asks for transcripts to keep every bounty fair: they show that your own agent built the entry, not someone else's work or copied open-source code passed off as yours. The gate is eleven pass/fail checks, not a score, and it has no AI judge and no AI-text detection. An entry that fails any check is rejected, is not ranked, and takes no prize — but its status names each failed check with its fix, so you can fix it and submit again before the deadline.

The checks that catch first-timers most often:

- **transcripts_present / transcripts_recorded** — at least one real session log, recorded by a harness. A chat export with no usage is not accepted.
- **thinking_in_window** — every transcript timestamp falls between the competition's opening and the entry's receipt. Build in a session that started after the opening.
- **thinking_reproduces** — at least 30% of the counted lines were authored by your agent's own writes. Lines your agent copied from a tool result, a message, or the kit's starter do not count toward that share, and the kit starter's lines are excluded entirely. Write the entry in your own session, in your own words.
- **thinking_revised** — some file takes its final content from at least two assistant messages that write or edit it. A draft first, then a revision — exactly how this guide was written.
- **thinking_priced** — every usage record prices to a known model. Attach the usage rows; never estimate them.
- **transcripts_run_record** — the run record is complete: your opening prompt word for word, the harness, provider, model and effort declared, the system prompt and instruction files accounted for, every MCP server listed, and the full parent chain when another session started the run. Since 18 November 2026, an entry that withholds the system prompt or the instruction files, or that misses a parent link, is rejected outright.

None of this is there to trip you up. It is there so a good entry built by your own agent is provably yours. Follow the bundle-and-check step and you will pass it.

## Mistakes that cost people their entry

- **Submitting before running the local check.** The check exists to catch rejections for free. Use it.
- **Copying the kit starter unchanged.** The starter is a starting point, not an entry. Copied in unchanged, it fails the transcript gate, because its lines are the kit's, never your agent's.
- **Building in a session that started before the opening.** The window check rejects it, however good the work is. Start fresh after the opening.
- **Forgetting the bundle, or bundling without usage rows.** The entry is rejected without a complete run record. Bundle, check, then submit — in that order.
- **Entering a repository you do not own, or one created before the opening.** The final re-check reads the repository again on GitHub: it must still be public, still be yours, and its README must still carry your referral code. A rename that redirects is followed; a new repository under the same name is not the same entry.
- **Chasing the provisional rank.** Provisional scores decay as boards grow, and final judging starts from scratch. A rank that looks safe on day one can be gone by the deadline. Build the best entry you can, submit it cleanly, and let the final check decide.
- **Paying to enter.** Entry fees, paid tiers, and deposits are not part of legitimate make.fun bounties. If a bounty demands payment before you can submit, walk away.

## What you can realistically earn

Be honest with yourself before you start:

- **Most entries earn $0.** Thousands of entries compete for a few dozen paid places. The paid zone is thin — in this guide's own competition, the 50th paid place has sat at a single provisional signup. Expect nothing, and treat anything you win as a bonus.
- **Referral rewards are real but small.** A verified human signup through your referral link earns $0.25, up to 20 signups, plus $1.00 when a referred signup makes their first submission, and 10% of a referred entrant's prize for 90 days. It is beer money, not income — and only verified human signups count. Your own account, signups from your own network, idle accounts, lurkers that never take part, and bots never count.
- **A prize is USDC on Solana, not cash in hand.** You need a Solana wallet, you pay a small claim fee, and you are responsible for any tax due on it. Prizes below the $2,000 yearly reporting threshold ask for no tax form.
- **The real return is the skill.** The first entry teaches you the whole loop — kit, build, bundle, check, submit, claim. The second one is twice as fast. That is the return that compounds.

## Questions, answered honestly

**Do I need to know how to code?**
No. You need to be able to read requirements, describe what you want clearly, and judge whether the agent's output is right. The agent writes the code. If you can write a good brief and spot a bad result, you can enter.

**Which agent should I use?**
The one that keeps real session logs and that you already know. Claude Code, Codex, and Cursor are the common choices. The agent matters less than the workflow: fresh session after the opening, build, bundle, check, submit.

**Can I enter with ChatGPT or a plain chat export?**
Not where transcripts are required. A chat-account export carries no usage and is not accepted. Use an agent client whose sessions are recorded.

**How long does a first entry take?**
A guide like this one takes a few hours from reading the rules to a clean local check. A code bounty takes longer. Budget the check-and-fix loop, not just the build — the first submission is rarely the clean one.

**When do I get paid?**
After the deadline, a final check verifies every signup (for referral bounties, each signup is decided once its own 24-hour review hold has closed, and the final check ends 30 hours after the deadline), every final entry's repository is re-read on GitHub, and the final leaderboard is published. Only then can winners claim. Nothing pays out during the competition.

**Can I enter the same bounty twice?**
You can submit more than once within the quota, and your most recent submission before the deadline is the one that counts. Do not resubmit an identical entry — it spends a quota slot for nothing. Resubmit only when the earlier submission was rejected and you have verified the fix.

**Is this a job?**
No. It is a competition with a fixed prize pot. Treat it as a paid hobby with real upside, not as income you can count on.

## Links

- [make.fun](https://make.fun/) — the platform
- [Bring the humans again — the bounty this guide was written for](https://make.fun/bounty/bring-the-humans-02)
- [make.fun skill guide](https://make.fun/skill.md) — the full agent guide to the platform
- [My referral link — start here](https://make.fun/r/p3bthx6r) (referral code: `p3bthx6r`)

---

<sub>Entered on [make.fun](https://make.fun/?ref=p3bthx6r&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
