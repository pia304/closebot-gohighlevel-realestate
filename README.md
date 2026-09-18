# gohighlevel chatbot for real estate: qualify buyers and sellers, book showings, and pick the right plan without hiring an ISA

A lead texts the number on your yard sign at 9:40 on a Sunday night. "Is 412 Maple still available? And what would mine go for?" That single inbox message can come from a buyer, a seller, an agent fishing for a referral, a wholesaler pitching you a deal, or someone who just wants a number and will never answer another text.

Real estate is unusual that way. Home services and dental practices get one lead type. You get eight, and they are worth wildly different amounts. The question a good ISA answers in about four seconds — *who is this?* — is exactly where most chatbot setups fall over.

This is the practical version of that problem: what GoHighLevel does natively, where it stalls, what a purpose-built layer on top of it actually adds for realtors and investors, and what it costs.

## What "GoHighLevel chatbot" actually covers now

GoHighLevel is not one chatbot. It is a stack of AI features bolted onto a CRM, and which one you get depends on what you pay for.

- The **website chat widget and SMS Conversational AI** handle text conversations and can qualify leads on your behalf.
- **Voice AI** answers inbound calls and books appointments.
- **Agent Studio** lets you build custom agents with their own knowledge base inside GHL.

All of it sits inside the CRM, which is the real advantage. A lead captured in chat is already a contact. Tagged, in a pipeline, enrolled in a workflow. No Zapier, no sync job that quietly breaks on a Tuesday.

The catch is the billing layer. HighLevel's published pricing lists an **AI Employee unlimited plan at $97/month per enabled location**, plus a growth-tier add-on around **$50/month per sub-account**, and Conversation AI prompt optimization that runs 100 messages a day before you're paying token costs. So "the chatbot is included" is only true up to a point.

## Where the native setup holds up — and where it doesn't

Be fair to it: for a solo agent already living in GHL, the native AI is genuinely useful. It captures and routes leads, it fires follow-up sequences across SMS and email, and it costs nothing extra beyond usage. Voice AI is something most dedicated chat tools simply don't offer.

Where it runs into trouble in real estate is conversation depth. Native AI is general-purpose, configured for real estate by you. It doesn't know that a tenant-buyer prospect asking about a rent-to-own listing needs a different first question than an off-market seller with an inherited property. Long-horizon nurture — the six-to-twelve-month drip that real estate actually requires — tends to come out as template sequences rather than real conversation.

Third-party comparisons put it the same way. A 2026 breakdown from Infina found that GHL's chatbot wins on native CRM integration, omnichannel automation, and cost efficiency, while dedicated tools win on industry-specific qualification and long-term nurturing. Their verdict: if you're already on GHL and not handling extreme volume, native is worth configuring properly first.

That's a reasonable position. It's also why the interesting question isn't "GHL or something else" — it's what you layer on top.

## What CloseBot adds on top of GoHighLevel

CloseBot is a conversational AI setter built specifically for CRM-based text channels. It integrates natively with HighLevel (plus HubSpot, LeadConnector, and custom CRMs via API), and it does not replace your GHL setup — your calendars stay your calendars, your workflows keep firing, and the agent writes bookings back into the sub-account.

For real estate specifically, the tooling is the part that separates it from a generic bot:

- **Live property data.** Give the agent an address and it pulls county records plus a market-adjusted value estimate — beds, baths, square footage — and can read back a rough valuation inside the first few messages. CloseBot says that covers over 100M US property data points.
- **Drive-time checks.** The agent can verify whether a property or a showing falls inside your service area before promising anything.
- **Image handling.** It can see images a lead sends and, if you enable it, send back aerial or streetview shots of a property.
- **Native calendar booking** through your CRM, so showings land on the calendar you already use.

According to CloseBot's real estate page, the tools report 30k+ daily messages in real estate alone and 250k+ real estate appointments booked. Those are vendor numbers, not audited ones — treat them as directional.

One important limit, stated plainly on that same page: **the property data tools only work for US properties.** Everything else — qualification, booking, multi-language conversations — works internationally. Property data carries no extra cost on any plan.

### The multi-lead-type problem, solved with tags rather than branches

This is the detail that matters most for anyone running a real estate inbox with mixed lead types.

The intuitive build is one agent that identifies the lead type, then branches to separate exits for seller, buyer, agent, or wholesaler. CloseBot's own writeup of a live build for an investor with eight lead types explains why that breaks: once a contact moves to a new node, they stay there. The "seller" who turns out to be an agent never comes back to the categorizing node.

The fix is to route on CRM tags instead. The agent replies when a contact is tagged as a seller, or a tenant-buyer prospect, or has no type tag at all — that last case being the receptionist scenario, where someone texts the number off a bandit sign and nobody knows who they are yet. When the AI figures out mid-conversation that this person is a realtor, it updates the contact type, the workflow swaps the tag, and the bot goes quiet on the next message by itself.

That build ran in about 50 minutes on an existing, already-organized HighLevel sub-account, starting from a CRM where the contact type field was already syncing to tags.

## CloseBot plans and pricing

Here's where the pricing model is worth reading carefully, because CloseBot runs two separate tracks off the same Free and Growth cards.

| Plan | Price | Billing | What's included | Best for | Get it |
| --- | --- | --- | --- | --- | --- |
| Free | $0 | Always free | 100 messages/mo, 1 agent, 1 user seat, 1 MB knowledge storage, unlimited account connections | Testing an agent, or genuinely low lead volume | [ Start on the free plan](https://app.closebot.com/a?fpr=li87) |
| Core — Business | From $64/mo monthly; $53/mo billed annually at $640/yr | Monthly or annual | Message costs included in the base price, 15+ templates, human support, add-on users ($5/seat), add-on storage, add-on agents | Realtors, teams, and investors running their own pipeline | [ See the current Core business pricing](https://app.closebot.com/a?fpr=li87) |
| Core — Agency | $397/mo monthly; $331/mo billed annually at $3,970/yr | Monthly or annual | Unlimited agents, white-label client portal, rebill all costs, client seats, per-message usage rebilled to clients | Agencies selling AI setting to realtor clients under their own brand | [ Check the Agency plan](https://app.closebot.com/a?fpr=li87) |
| Growth | Custom | Custom | 50+ templates, HIPAA compliance, quarterly audits, 99.99% priority uptime, priority support | Regulated or high-volume operations needing SLAs and audits | [ Talk to CloseBot about Growth](https://app.closebot.com/a?fpr=li87) |

A note on the two Core rows: they are genuinely different products wearing the same name. The business version is priced by how many monthly messages you need, and the agency version is a flat rate with usage rebilled to clients.

### The part that scales: monthly message volume

On the business track, price rises with the message ceiling you pick. A third-party review that says it checked the plans page in August 2026 listed these tiers:

| Messages included per month | Core business price (monthly billing) |
| --- | --- |
| 100–500 | $64/mo |
| 1,000 | $84/mo |
| 2,000 | $109/mo |
| 5,000 | $176/mo |
| 20,000 | $454/mo |
| 50,000 | $806/mo |
| 100,000 | roughly $1,059/mo |

Treat the middle rows as directional and confirm on the plans page before you budget, since the ladder is slider-driven.

A few cost details that catch people out:

- **Free plan overage** runs at $0.08 per message beyond 100.
- **Business plans** include 500 messages in the base; if you blow past your ceiling, overage draws from your wallet at 2x the standard rate.
- **Agency plans** are billed $0.012 per message, which you rebill at whatever markup you set. Worth knowing: CloseBot's help docs still describe $0.006 per message, which appears to be the older agency rate. The plans page and its FAQ currently say $0.012.
- **Storage**: business plans include 1 MB, with add-on storage priced between $0.10 and $3.00 per MB per month depending on volume. Agency storage runs $0.006 per MB per day.
- **Seats**: one user included; $5 per additional user on both paid tracks.
- **Annual billing gives you two months free** and unlocks a larger template library (50+ extra templates versus 15+ on monthly).

### What a "message" actually means

One message equals one segment, unless you turn on the Agent Node's unlimited potential — adding many tools or unlimited instruction size — at which point billing switches to token costs and a single reply can consume several segments. If you're building a heavy agent with property lookups, drive-time checks, and inventory queries, budget above the headline number rather than at it.

Also worth knowing before you commit: **there are no refunds.** What you get instead is a free-forever plan under 100 messages a month and a **7-day trial of any paid plan** before billing starts. Plans are month to month.

And if your plan was to plug in your own OpenAI or Anthropic key to control costs, the current FAQ says no — CloseBot doesn't allow bring-your-own-key, framing it as a security decision.

## Getting an agent live in your HighLevel sub-account

The setup path is short, and none of it requires a developer.

1. **Connect the source.** In CloseBot, go to Sources, add a new source, choose HighLevel Sub-Account, and approve the OAuth permissions for the sub-account you want. You land back on a Sources list that confirms the connection.
2. **Sync your tags.** CloseBot's source filters read tags, not dropdown fields. If your CRM is organized around a contact type field, build a HighLevel workflow that keeps tags in sync with it. Keep the field as the source of truth so nothing else in your account breaks.
3. **Write the agent instructions like an SOP.** For motivated sellers, that means address first (it's the only mandatory field), then timeline, reason for selling, condition, whether it's already listed, and mortgage balance. For tenant-buyer and seller-finance prospects, the priority is trust — you need people comfortable being honest about down payment and assets, which is a very specific instruction to write.
4. **Attach the tools.** Property details, drive time, and — if you want the agent answering buyer questions about current inventory — a connected Google Sheet with live listings that it can read.
5. **Test in the testing portal before real leads.** Run conversations with a persona attached, and turn on thinking mode so you can see the agent's reasoning. The agent's reasoning shows on your conversations screen, not to leads.
6. **Refresh after connecting a source.** Custom fields don't re-pull instantly, so if fields are missing from your @ mention list, refresh the page. CloseBot's own writeup flags this as a mistake that cost one user a week.

## Which plan is actually right for you

If you're a solo realtor or a small team and want to see whether an agent beats your current speed-to-lead workflow, start on the **Free plan**. 100 messages a month is not much, but it's enough to build an agent, test it in the portal, and decide. Given that there are no refunds, that trial period is where your testing should happen.

If you're running your own pipeline with a real lead flow — several hundred to a few thousand inbound messages a month — the **Core business plan** is the sensible landing spot. Message costs are included in the base price rather than metered on top, which makes budgeting simpler than a metered API bill.

If you're an agency selling AI setting to realtor clients, **Core Agency** is the one that changes your P&L. Rebillable usage at $0.012 per message, a white-label portal, and client seats mean the $397/month isn't purely an expense line.

**Growth** only makes sense if you need HIPAA coverage, quarterly audits, SLAs, or volume that the slider can't price cleanly.

## Things to know before you buy

- **Property data is US-only.** Qualification and booking work anywhere; the county records and valuation tools don't.
- **The agent needs someone to own it.** The most common criticism in GHL communities is the learning curve — one Reddit thread has an agency owner saying they were "immediately turned off" by it. CloseBot's own community layer (courses, daily live calls, certified partner builders) exists for this reason. If nobody on your team will build and test properly, the agent will inherit a sloppy process and scale it.
- **Filtered-out leads hear silence.** Tag someone as an agent or wholesaler and the bot stops replying with no explanation. Add a canned response on that tag.
- **No CRM, no CloseBot.** It can run standalone on website chat via its widget, but the real value assumes a CRM inbox underneath it. If your leads all arrive as Instagram DMs and you don't run a CRM, you'd be buying two products.

## FAQ

**Can a GoHighLevel chatbot qualify real estate leads overnight?**
Yes, and overnight is the point. An agent connected to your GHL sub-account replies in seconds across your CRM's text channels, qualifies the lead against the objectives you set, follows up, and books onto your calendar while you're asleep. What it can't do is close — the appointment is the output.

**How is this different from GoHighLevel's native Conversation AI?**
Native AI is a general-purpose add-on inside the platform you already pay for. CloseBot is a separate layer built for appointment setting, with real estate tooling like property data and drive-time checks, plus an agent that reasons through objectives rather than following a fixed flow. CloseBot's own comparison page claims up to 20% more bookings reported when agencies switch, along with 99.99% uptime — vendor claims, but consistent with what third-party reviews describe as stronger conversation quality.

**Does it work with the HighLevel calendars and workflows I already have?**
Yes. CloseBot sits on top and uses what's already there. Objections you've already handled, pipelines you've built, and workflows you've automated keep working; the agent handles the conversation and writes the booking back.

**What does it cost to run an agency offering on it?**
$397/month on the Agency plan with usage at $0.012 per message rebillable to clients. CloseBot says some agencies charge clients as little as $100/month while others bill $10k+ from a single client, and its own figures put the average bill per client around $500/month. Your margin is whatever you set, minus the per-message cost.

**Is it worth it for an investor with eight lead types?**
That's arguably its strongest use case in real estate, because tag-based routing handles changing lead types without the agent getting stuck in a branch. The tradeoff is setup discipline: you need the contact-type field and tags kept in sync, and you need to remember to update your filters whenever you add a new lead type.

## The short version

Speed to lead still decides most real estate conversations, and the second question — *who is this?* — decides whether the agent helps or embarrasses you. GoHighLevel's native AI covers the basics inside a CRM you already pay for, and for a solo agent that may be enough. Once your inbox mixes motivated sellers, tenant-buyer prospects, cash buyers, wholesalers, and agents, you need an agent that routes on CRM data, pulls real property information, and books showings without a human in the middle.

Start on the free plan, build one agent, and test it against the leads you already lost last month. That comparison will tell you more than any feature table.

[👉 Build your first CloseBot agent free](https://app.closebot.com/a?fpr=li87)
