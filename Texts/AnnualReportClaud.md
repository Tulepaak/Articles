Filing an Annual Report for an Inactive Company — With a Little Help From Claude
by Ingmar Vali
There is a particular kind of innovation that doesn’t start with a grand architecture diagram or a moonshot roadmap. It starts with the simplest positive scenario — the most used, most boring happy path — and asks whether it actually works end-to-end. If it does, you iterate outward: the next scenario, then the edge cases, then, finally, the corner cases you close off with a risk matrix. This, I believe, is how modern government services should be built. Not by trying to solve every exception up front, but by first nailing the easy case and letting reality push you toward the hard ones.
Last week I did exactly that with one of the oldest pieces of Estonian digital-government infrastructure: the annual report submission to the Business Register.

The Forgotten Innovation
The option to submit an annual report in the machine-readable XBRL format has existed in the Estonian Business Register since annual reporting became mandatory in 2009. At the time, it won awards for its innovation and implementation — a government system that accepted structured, machine-validated financial statements long before “API-first” became a buzzword.
And yet, for me, XBRL has always felt less like a format and more like code: an XML dialect, a taxonomy schema, contexts, dimensions, instant vs. period facts. Not exactly the kind of thing you hand to a small-business owner and say “good luck.” So the format sat there, technically superb, used mostly via accounting software that hid it from view.

The User Story That Changed My Mind
While doing user research with entrepreneurs, I ran into a familiar story. A business owner had an inactive company — no operations, no revenue, no changes from the previous year — and still had to file an annual report. The alternatives were the usual two: skip it and risk a fine, or sit down and do the paperwork one more time. Most people pick option one until the warning letter arrives.
We decided to try a third option. We sat down together for about fifteen minutes.

The Simplest Positive Scenario
The Estonian annual reporting system has a genuinely useful feature: you can download the current year’s report template pre-filled with the previous year’s figures, as an XBRL file. That download was our starting point.
I handed the file to Claude AI with an instruction that was almost absurdly short: copy last year’s numbers into this year’s columns, because the company is inactive and nothing has changed.
Claude parsed the XBRL, identified every tag that existed for the 2024 period but was missing for 2025, and mirrored them. It reconciled the balance sheet — Assets = Liabilities + Equity, both 2 546 €, both years — confirmed the equity roll-up (share capital + reserves + retained earnings + annual profit), and left the tax-dimension contexts untouched because they already matched. Fifteen minutes after we started, the file was ready to upload. Compliance done. When the business picks up again, the company is in good standing and ready to be used.

Why This Matters More Than It Looks
This is a tiny case. One file, one inactive company, one filing that would have taken a professional accountant maybe half an hour. But it demonstrates something I keep coming back to in conversations about government innovation: the most used, simplest scenario is the right place to start.
Inactive companies are not an edge case. A huge portion of Estonia’s registered legal entities are in exactly this state at any given moment — dormant, parked, waiting for the next idea, used as holding vehicles, or slowly wound down. For all of them, the “copy last year” filing is the dominant pattern. Solving the boring majority first is where the leverage lies.
From there the iteration is natural. Next comes the micro-enterprise with a handful of invoices. Then the small company with real P&L structure, geographic revenue breakdowns, and tax detail. Then the group with consolidated accounts, related-party disclosures, and notes. At each step, you learn what the AI agent can reliably do, where human review is essential, and where the underlying government interface needs to improve. You don’t start with corner cases — you end with them, and by then you have a risk matrix instead of a panic.

What the Government System Already Supports
Here is the part worth underlining. I did not need a special API, a pilot program, or any kind of privileged access. The Business Register’s XBRL-based reporting has supported machine interaction for over fifteen years. The format is well-documented, the taxonomy is versioned, the validator is built into the portal. All of the ingredients an AI agent needs were already there.
What was missing was the user-friendly bridge — a way for a non-technical owner to have the XBRL work done for them in plain language. That bridge turned out to be a general-purpose AI assistant, given a clear instruction and a file. No custom integration required.
If you have an inactive company and you need to file the annual report, just do it. With a little help from Claude, the government system supports it. Agentic state.

The Road Ahead
My next step is to run the same experiment with real, active data — a company with actual transactions, a real revenue breakdown, actual tax liabilities — and see how far the positive-scenario pattern carries. Then the next company profile, and the next, until the routine filings can be safely delegated to an agent with a human approving the result.
That is the iteration loop: happy path first, then complexity, then the corner cases. Each step teaches you something the previous one couldn’t. And each step makes the next entrepreneur’s life a little easier.
The Business Register was machine-readable before most of us were ready for it. Fifteen years later, the agents have finally caught up.

Tulepaak OÜ 
https://www.tulepaak.ee/
Ingmar Vali
CEO
