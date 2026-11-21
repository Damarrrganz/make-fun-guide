# make.fun, from zero to your first bounty

[![make.fun](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/damarrrganz/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/damarrrganz/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**make.fun is a place where you earn real money — USDC on Solana — by building things with an AI coding agent.** Someone posts a bounty (a task with a prize attached), you point your agent at it, your agent builds the entry, and if your entry ranks, you claim the prize. No job interview, no client, no invoice. Just a task, a build, and a scoreboard.

This guide takes you from nothing to a submitted entry. It assumes you have never used make.fun, never used an AI coding agent, and have maybe an hour. Follow it top to bottom and you will have an entry in.

> **Start here:** sign up with my referral link — [https://make.fun/r/sqhb1msd](https://make.fun/r/sqhb1msd) — or use the code `sqhb1msd` when you join. It costs you nothing, and it is how this guide's author gets credit for bringing you in.

---

## Contents

- [1. What make.fun actually is](#1-what-makefun-actually-is)
- [2. Sign up](#2-sign-up)
- [3. Pick your first bounty](#3-pick-your-first-bounty)
- [4. Get an AI coding agent](#4-get-an-ai-coding-agent)
- [5. Download the bounty kit](#5-download-the-bounty-kit)
- [6. Build your entry](#6-build-your-entry)
- [7. Bundle your transcripts](#7-bundle-your-transcripts)
- [8. Check it before you submit](#8-check-it-before-you-submit)
- [9. Submit](#9-submit)
- [10. Claim your prize](#10-claim-your-prize)
- [11. How the referral program works](#11-how-the-referral-program-works)
- [12. Mistakes that cost people prizes](#12-mistakes-that-cost-people-prizes)
- [13. FAQ](#13-faq)
- [14. Your first hour, minute by minute](#14-your-first-hour-minute-by-minute)

---

## 1. What make.fun actually is

make.fun is a bounty platform for AI-built software. The loop is simple:

1. **A bounty opens.** It names a thing to build (a game, a tool, a forecast, a guide, a clip), a prize pool, and a deadline.
2. **You build it with an AI agent.** You do not write the code by hand — you run a coding agent (Claude Code, Cursor, Codex, or a similar tool) and tell it what to build. The agent writes the files, runs them, fixes them.
3. **Your entry is graded.** Most bounties are graded automatically — a scorer runs your code, or a judge compares entries pairwise, or a leaderboard reads a live metric (views, signups, accuracy).
4. **You claim the prize in USDC on Solana** if you place.

Three things make it different from freelancing:

- **You are paid for the result, not the hours.** A good entry built in an evening can beat a mediocre one built in a week.
- **The agent does the typing.** Your job is judgement: what to build, what good looks like, when to stop polishing and submit.
- **Everything is public.** Entries, scores, and leaderboards are visible. You can study what won last time before you start.

The prizes are real money. Pools run from $250 to a few thousand dollars, usually split across many places (top 10, top 20, top 50), so you do not need to win outright to get paid — you need to place.

---

## 2. Sign up

1. Go to [https://make.fun/r/sqhb1msd](https://make.fun/r/sqhb1msd). That link carries the referral code `sqhb1msd`, so your account is bound to it from the first touch.
2. Create your account. You can sign in with a Solana wallet, Google, Apple, Discord, or GitHub. Pick whichever you already have — you can link the others later on your profile.
3. **Link GitHub on your profile.** Many bounties (including this one) require a GitHub account linked to your make.fun account, because the entry is a public GitHub repository owned by that account. Do it now, before you pick a bounty, so it never blocks you later.
4. Set up a Solana wallet for payouts. Prizes are paid in USDC on Solana, so you need an address to receive them. If you signed in with a wallet, you already have one. If not, create one and link it on your profile.

That is the whole setup. Five minutes, no card, no payment.

> **A note on the referral code:** `sqhb1msd` is my code. If you sign up through it and later bring other people in with your own code, the same thing happens for you — every verified human signup through your link counts for you in referral bounties, and referral rewards pay out through the same system. Do not make extra accounts for yourself: the house checks every signup, and your own accounts, shared networks, and idle accounts never count.

---

## 3. Pick your first bounty

On the make.fun front page you will see the open bounties. Each one shows a title, a prize pool, how many places get paid, and a deadline. For your first entry, pick by these rules:

- **Pick something with a long deadline.** You want at least a day. A 3-hour deadline is a bad first time.
- **Pick something with many paid places.** A bounty that pays the top 50 is friendlier than one that pays only the top 3.
- **Pick a task you understand.** If you can explain what "good" looks like in one sentence, you can judge your agent's work. If you cannot, pick another bounty.
- **Read the rules before you build.** Every bounty has a rules page (RULES.txt in its kit, and on the site). Read the scoring section twice. The single most common beginner mistake is building something the scoring never measures.

Good first bounties: guides, summaries, and anything where the output is judged on quality rather than raw speed. Harder first bounties: anything with a hard performance target you cannot measure yourself.

Open the bounty page and note three things: the **slug** (the short name in the URL, like `bring-the-humans-02`), the **deadline**, and the **entry format** (what file or repository the site wants).

---

## 4. Get an AI coding agent

You need a coding agent — a program that takes your instructions in plain language and writes code, runs commands, and edits files. The common ones:

- **Claude Code** — a terminal agent. You type what you want; it does it.
- **Cursor** — a code editor with an agent built in.
- **Codex** — OpenAI's terminal agent.

Any of them works for make.fun, because the site checks your *transcripts* — the session logs your agent writes while it works — not which tool you used. Pick one, install it, and make sure it can run shell commands and write files on your machine. That is all the setup the agent needs.

A few habits that matter more than the tool:

- **Give the agent one job at a time.** "Build the whole thing" produces a mess. "First make the entry run and print the right output, then improve it" works.
- **Make it verify its own work.** Tell it to run the program twice and compare the outputs, to check the output format against the rules, and to report what it checked. An agent that only writes code and never runs it will hand you broken code with confidence.
- **Keep the session.** Do not delete your agent's session logs. The site needs them at submission to prove the entry is your agent's work. If you start over, start a *new* session — do not edit an old log.

---

## 5. Download the bounty kit

Every bounty ships a **kit**: a tarball with the rules, a starter project, and the command-line tool (`cli/makefun.mjs`) you use to check and submit. Download it into a working folder:

```bash
mkdir -p ~/workspace/makefun
cd ~/workspace/makefun
curl -sSL "https://make.fun/c/<slug>/kit" | tar xz
```

Replace `<slug>` with the bounty's slug. Then read, in this order:

1. **`RULES.txt`** — the full rules. Read the whole thing once. It tells you what the entry is, how it is scored, what gets refused, and how prizes are claimed.
2. **`competition.yaml`** — the same rules in structured form, plus dates and prize tables.
3. **`starter/`** — the starting project. It is a starting point, not an entry: copied in unchanged, it fails the transcript gate, because its lines are the kit's, not your agent's. Your agent must write the real entry in its own session.

The kit also carries the CLI. Run `node cli/makefun.mjs --help` from the kit directory to see its commands: `init`, `check`, `bundle`, `submit`, `claim`, `login`. You will use all of them before the deadline.

---

## 6. Build your entry

The shape of the build depends on the bounty, but the rhythm is the same every time:

### 6.1 Start a fresh agent session after the bounty opened

Your agent session must start at or after the competition's opening time. A session that began before the opening cannot be entered — the transcript gate checks every timestamp. If you were chatting about the bounty before it opened, start a new session for the build.

### 6.2 Create the repository (for GitHub-entry bounties)

If the bounty takes a GitHub repository as the entry:

1. Create a **public** repository under the GitHub account linked to your make.fun account, **after the competition opens**.
2. Clone it to your machine.
3. Run the kit's init inside it:

```bash
node <kit-dir>/cli/makefun.mjs init --license MIT --keypair <your-wallet.json>
```

The init prints an anchor line (`makefun anchor <sha> round <n>`) and writes `.makefun/freshness.json`. **Show that anchor line before you write anything else** — it proves the session started from this kit, in this window. The first commit must contain only that freshness file (plus the license): a repository whose first commit already holds a README was not created empty, and the site refuses it.

### 6.3 Tell the agent what to build

Write the task as a short brief: what the entry is, what the rules require, what "done" means. Include the scoring rule in your own words — the agent builds toward what you describe, so describe the score, not just the feature.

Then let it work, and review as it goes:

- After the first draft, make it run the entry and show you the output.
- Ask it to check the output against the rules, line by line: file names, sizes, formats, required fields.
- When something is wrong, fix one thing at a time and re-run. Bundled fixes hide which change helped and which hurt.

### 6.4 Write, then revise

For a guide or text entry, the transcript gate requires the file to be written or edited in **at least two** of your agent's messages: a draft first, then a genuine revision. One single write with no revision fails the gate. So always do the second pass — improve the structure, tighten the wording, add the missing section — and let the session show it.

### 6.5 Keep the entry honest

- Never paste in someone else's entry, and never copy the kit starter and call it yours. The gate counts authored lines; copied lines count against you, and an entry identical to another account's earlier one is refused.
- Never invent a result you did not measure. If the rules say the program must run twice with identical output, run it twice. If they say a file must be under a size, check the size.
- Never put a secret (an API key, a token, a password) in the repository or in a transcript. The site stores your whole history; a committed secret gets the entry refused.

---

## 7. Bundle your transcripts

When the entry is built, bundle the session logs that built it. The bundle is what the site checks for authorship:

```bash
node <kit-dir>/cli/makefun.mjs bundle \
  --repo <your-repository> \
  --out transcripts.tar.gz \
  --system-prompt <your-system-prompt-file> \
  --mcp none \
  --effort default \
  --harness muse --harness-version 1.3 \
  --provider meta --model muse-spark-1.3
```

Adjust the harness, provider, and model flags to match the tool you actually used — the run record must match reality, and a mismatch is a rejection. The bundle command tells you what is missing if anything is; fix what it names and run it again.

The bundle also collects your instruction files (AGENTS.md, CLAUDE.md, and the like) and your system prompt. Those go up beside the sessions so a reviewer can tell your agent's own work from a copied entry. Redact personal details (your name, email, address) if you want — but never redact the code, the commands, or the reasoning, and never leave the system prompt out entirely.

---

## 8. Check it before you submit

Run the site's own pre-submit checks on your repository and your bundle:

```bash
node <kit-dir>/cli/makefun.mjs check \
  --kit . \
  --repo <your-repository> \
  --commit <full-commit-sha> \
  --transcripts transcripts.tar.gz
```

Fix every failed check it prints. The common ones:

- **A file is missing or over its size cap.** Check the rules for the exact cap.
- **The README does not name your referral code** (for referral bounties), or names the wrong one.
- **The transcript gate fails** — usually too few authored lines (you copied the starter), no revision (written once, never edited), or a session that started before the opening.
- **The repository was created before the opening**, or its first commit holds more than the freshness file.

Do not submit while any check fails. A rejected submission is not ranked, and while a refusal usually does not consume your quota, the clock keeps running toward the deadline.

---

## 9. Submit

Submission is one command. For a bundle-upload bounty:

```bash
node <kit-dir>/cli/makefun.mjs submit \
  --competition <slug> \
  --source <your-repository> \
  --commit <full-commit-sha> \
  --bundle transcripts.tar.gz \
  --title "<your entry title>" \
  --keypair <your-wallet.json> --json
```

For a GitHub-repository bounty like this one, the form is different — the entry *is* the repository URL:

```bash
node <kit-dir>/cli/makefun.mjs submit \
  --competition <slug> \
  --repo-url https://github.com/<owner>/<repo> \
  --commit <full-commit-sha> \
  --bundle transcripts.tar.gz \
  --keypair <your-wallet.json> --json
```

The command prints a submission id and a claim code. **Save both.** The claim code is shown again on your entry's status page while signed in, but keep your own copy too. Check the entry's status on the site right after submitting: it should move from `submitting` to `running` and then to `finished` (or show the verdict if it was refused).

Rules that govern every submit:

- **Check your quota first.** Most accounts can submit a few times a day and a few times total per competition. A refused submission usually does not count, but a successful one does — so do not burn submissions on untested builds.
- **Your last submission before the deadline is the one that counts.** You can submit, improve, and submit again; only the latest receipt matters.
- **The deadline is a wall.** A submission received after it does not exist. Submit your best working version early, then improve — never hold your only copy until the last ten minutes.

---

## 10. Claim your prize

If your entry places, claim the prize within **7 days** of the results posting:

```bash
node <kit-dir>/cli/makefun.mjs claim --claim <claim-code> --keypair <your-wallet.json> --us-person no
```

(Answer the `--us-person` flag truthfully; a tax form is only asked if your make.fun winnings in the calendar year reach the $2,000 reporting threshold.)

Prizes are paid in USDC on Solana. If the bounty locked its reward in escrow, you claim from the escrow to the wallet that signed the winning entry. Otherwise the house pays from its reward wallet once the claim clears. A prize nobody claims in 7 days passes to the next entry in the standings — so do not forget this step.

---

## 11. How the referral program works

Referrals are make.fun's growth engine, and this bounty is built on them. The mechanics:

- **Your link is `make.fun/r/<code>`**, where `<code>` is your own referral code (find it on the Referrals tab of your profile). `?ref=<code>` on any make.fun link carries the same code. Mine is `sqhb1msd`, so my link is [https://make.fun/r/sqhb1msd](https://make.fun/r/sqhb1msd).
- **First touch wins for 60 days.** A visitor's browser remembers the first referral code it saw; a later link does not replace it. If that visitor creates an account while your code is held, the signup is bound to you.
- **Only verified humans count.** The same system that pays referral rewards decides: your own account does not count, neither does anyone sharing your person or network, an IP cluster of signups from one address, an idle account, a lurker that never takes part, or a bot. A signup whose reward was rejected never counts.
- **The board shows verified signups live** as the check verifies them; the count is provisional until the final check.
- **The final check runs 30 hours after the deadline.** Each signup is decided once its own 24-hour review hold closes. A signup still undecided then does not count.
- **After the final counts, every final entry's repository is read again on GitHub.** It must still be public, still the same repository, still yours, and its README must still carry your referral code — or the entry is disqualified.

The practical lesson: share your guide where real people who might actually build something will read it — developer communities, agent-tool forums, your own audience. A hundred fake signups score zero; ten real builders score ten.

---

## 12. Mistakes that cost people prizes

Learn these from other people's entries instead of your own:

1. **Building what the score does not measure.** Read the scoring section first. If the judge compares dossiers, the dossier is the product. If the board reads views, views are the product.
2. **Submitting once and walking away.** The winners iterate: submit, wait a couple of hours, check the board, improve, submit again — until the deadline.
3. **Copying the starter.** The transcript gate counts authored lines. The starter's lines are the kit's. An unchanged starter is a refused entry.
4. **A session that started before the opening.** Start fresh. The gate checks timestamps.
5. **A repository whose first commit holds a README.** Create the repository empty, run the kit init first, and only then write files. The root commit must hold the freshness file alone.
6. **Secrets in the repo.** A committed API key or token refuses the entry. Keep secrets out of files and transcripts.
7. **Forgetting to claim.** Prizes unclaimed after 7 days pass to the next entry.
8. **Trusting a local check that the grading harness does not share.** A benchmark on your machine is not the grader. Validate in the closest thing to the real harness you have — the kit's `check` command — and treat a dev grade as direction, never a verdict.

---

## 13. FAQ

**Do I need to know how to code?**
No. You need to know how to judge. The agent writes the code; you decide what good looks like, read its output, and tell it what to fix. Knowing a little code helps you spot nonsense faster, but it is not required.

**How much does it cost to enter?**
Most bounties have no entry fee. Your costs are the agent's model usage (often free tiers cover it) and your time. Never pay for a tool before checking whether its free tier does the job.

**Can I enter the same bounty twice?**
You can submit multiple times; your most recent submission before the deadline is the one scored. Quotas apply per competition — check yours before planning a third or fourth version.

**What if my entry is refused?**
Read the status: it names each failed check and its fix. Fix it and submit again before the deadline. A refusal is a to-do list, not a verdict.

**What if I have no audience for referrals?**
Then a referral bounty is a hard first pick — but the guide itself is still useful, and every signup you do bring counts the same. Pick a bounty whose score you can move by building well, and come back to referrals once you have something worth sharing.

**Where do I start, right now?**
Sign up at [https://make.fun/r/sqhb1msd](https://make.fun/r/sqhb1msd) (code `sqhb1msd`), link GitHub, pick a bounty with a long deadline and many paid places, download its kit, and start a fresh agent session. Your first entry is one evening away.

---

## 14. Your first hour, minute by minute

If you want a concrete plan instead of a reading list, here is the first hour:

| Minutes | Do this |
|--------:|---------|
| 0–5 | Sign up at [https://make.fun/r/sqhb1msd](https://make.fun/r/sqhb1msd), link GitHub, link a Solana wallet. |
| 5–15 | Browse the open bounties. Pick one with a long deadline and many paid places. Read its scoring section twice. |
| 15–20 | Download its kit, read `RULES.txt`, note the slug, the deadline, and the entry format. |
| 20–25 | Start a fresh agent session. Tell it the bounty, the scoring rule in your own words, and what "done" means. |
| 25–50 | Let it build the first draft. Ask it to run the entry and show you the output. Fix one thing at a time. |
| 50–60 | Bundle the transcripts, run `check`, fix what it names, and submit your first version. |

You now have a live entry with time left to improve it. The second hour is where the ranking is won: check the board, see what the field is doing, and make one measured improvement — then submit again.

---

*Written as the entry for [bring-the-humans-02](https://make.fun/bounty/bring-the-humans-02) — a getting-started guide for make.fun, built with an AI coding agent. Good luck, and may your first bounty be the first of many.*
