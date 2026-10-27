# Making Tax Services Understandable

**Hackathon problem statement 08:** Help users understand tax-related steps, identify inconsistencies in their information, and find appropriate next actions.

**Core idea:** An *understanding layer* on top of tax portals. The interface explains at the point of confusion, so users have to ask fewer questions.

---

## Slide 1: The Problem
- Users often don't know what a tax step means or what to do next.
- The usual fix is to add a chatbot.

## Slide 2: Why Chatbots Seem Like the Answer
- Always available, with no waiting for a helpline
- Instant replies
- Common questions answered without a human
- On paper, a chatbot fits the problem.

## Slide 3: Where Chatbots Fall Short
- **Scripted chatbots:** limited by what the developer predicted users would ask. Unexpected wording gets a generic answer.
- **LLM chatbots:** users still need to know what to ask. Answers can be long, generic or wrong, and sit away from the confusing field.
- **Both kinds:** one fixed explanation, even though users need different levels of detail.

> Speaker tip: give one concrete example, such as a user who sees "TDS mismatch" and has no idea what to type into a chatbot.

## Slide 4: Our Insight
> The confusion doesn't start at the form. It starts at the front door.

- Evidence: the Income Tax e-Filing home page shows a rotating banner, a scrolling ticker, long announcements and seven top-level menus before a new user finds where to start.
- Tone: the portal serves many audiences, so the answer is personalization, not criticism.

## Slide 5: The Understanding Layer
1. **Guided start:** "What would you like to do today?" opens short paths (file my return, I received a notice, check refund or status, I'm new) into the right section.
2. **Contextual help:** a "?" at the exact field, with a short hint, a "learn more" option and an example.
3. **Mismatch flags:** inline notes beside data that doesn't line up, with a plain-language reason.
4. **Next-steps panel:** a prioritized checklist of what to do, and by when.
5. **Progress cues:** users always see where they are in the process.

## Slide 6: Live Demo
1. Start at the guided landing page
2. Take a guided path
3. Click a "?" for a plain-language explanation
4. See a caught mismatch and why it matters
5. End on the prioritized action list

## Slide 7: Why It Matters
- **Faster starts:** quicker time to the first correct action, with fewer wrong turns.
- **Fewer errors:** mismatches caught before submission, so fewer abandoned filings and less reliance on helplines and accountants.
- **Easy to adopt:** a layer on top of existing portals, so nothing has to be rebuilt.
- **Scalable:** "explain at the point of confusion" works for any government or financial service.

> If you have test numbers, even from a handful of people, add one here. If not, say these are the outcomes you would measure.

## Slide 8: Closing
> Chatbots answer questions well, but the best help is the kind users never have to ask for. That's what an understanding layer delivers.

> We're not adding tooltips. We're changing who does the work of understanding: from the user to the interface.

*Delivery tip: pause after "ask for."*

---

## Build plan for the demo (hackathon scope)
- Build a clickable prototype of your own, not an integration with the real portal.
- One persona: a first-time salaried filer.
- Three guided paths: file my return (deepest), I received a notice, I'm new.
- Sample data with about five hard-coded mismatch rules (for example, income on the salary slip vs. the tax statement, or TDS claimed vs. deducted).
- Pre-written explanations for the "?" help and mismatch flags. If an LLM is used, generate them ahead of time or make it optional so the demo can't break.
- Stretch goals: a browser-extension overlay on the real portal, and a quick test with 3-5 people for one real number.
- Suggested time split: 20% design and flow, 50% prototype, 15% demo script and rehearsal, 15% slides.
