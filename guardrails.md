# The guardrails

This is the part I care about most and it's the thinnest part of the research. I went looking for things that have actually been tested and came back with three. Everything else is a framework, a set of design recommendations, or a result that didn't go the way people hoped.

## Tested, with a measured effect

- **Show the uncertainty in the output.** [Effects of LLM-Based Search on Decision Making](https://www.microsoft.com/en-us/research/publication/effects-of-llm-based-search-on-decision-making-speed-accuracy-and-overreliance/), CHI 2025. People overrelied on AI search when it was wrong. A colour-coded highlighting system helped them catch the errors and make better decisions, and it didn't make the task slower or less pleasant. As far as I can tell this is the best-evidenced guardrail anyone has. **Moderate.**
- **Make your own call before you see the AI's.** [Who Goes First?](https://www.microsoft.com/en-us/research/publication/who-goes-first-influences-of-human-ai-workflow-on-decision-making-in-clinical-imaging/), FAccT 2022, with the [preprint](https://arxiv.org/abs/2205.09696) and [code](https://github.com/microsoft/Exp-HAIC). Radiologists asked to register a provisional read before seeing the AI were less likely to just agree with it, and it didn't take them any longer. Read the next section before you get excited about this one. **Moderate.**
- **Take notes even when the AI is right there.** [Effects of LLM Use and Note-Taking on Reading Comprehension and Memory](https://doi.org/10.1016/j.compedu.2025.105514), Computers and Education, 2025. 405 students, randomized, tested three days later. Note-taking on its own, and note-taking alongside the LLM, both beat using the LLM alone. Not a product feature, just a thing you do. **Strong.**

## Tested, with mixed results

Probably the most useful thing in this whole area is that mitigations don't reliably work.

- **Slowing people down reduces reliance and costs you something.** Buçinca, Malaya and Gajos, [To Trust or to Think](https://doi.org/10.1145/3449287), CSCW 2021. Cognitive forcing functions cut overreliance and also made the experience worse. There's a genuine trade here, and pretending otherwise is how these features get cut in the first review.
- **Less reliance isn't the same as better reliance.** The provisional-call study above made people less likely to agree with the AI whether or not it was right, which isn't obviously a win. There's newer work finding that warnings and friction can reduce overreliance while doing nothing to help people tell good advice from bad, and that in some setups people came away more confident after making worse calls. This is the thing I'd most want someone to study properly. I still need to track down a proper citation for this one.
- **A label meant to help can make things worse.** The implied truth effect, Pennycook, Bear, Collins and Rand, Management Science, 2020. When some false content gets flagged, the false content that isn't flagged starts looking more credible. Microsoft's [media authenticity work](https://www.microsoft.com/en-us/research/blog/media-authenticity-methods-in-practice-capabilities-limitations-and-directions/) warns about something similar: a visible watermark without real provenance behind it may stop people consulting the tool that would verify anything.

## Frameworks and guidance

Useful, and I lean on them, but none of these come with a measured result attached.

- [Overreliance Risk Identification and Mitigation Framework](https://aka.ms/overreliance-framework), Microsoft Research, 2025. The most practical thing on this list. Walks you through finding overreliance risk in a product and choosing what to do about it.
- [Fostering Appropriate Reliance on GenAI: Lessons Learned](https://www.microsoft.com/en-us/research/publication/fostering-appropriate-reliance-on-genai-lessons-learned-from-early-research/), MSR-TR-2025-4. Three UX goals, plus a blunt warning that mitigations can backfire and have to be tested.
- [Appropriate Reliance on Generative AI: Research Synthesis](https://www.microsoft.com/en-us/research/publication/appropriate-reliance-on-generative-ai-research-synthesis/), MSR-TR-2024-7. Around 50 papers on which mitigation strategies hold up.
- [Overreliance on AI: Literature Review](https://www.microsoft.com/en-us/research/publication/overreliance-on-ai-literature-review/), MSR-TR-2022-12. Where this line of work started.
- [Guidelines for Human-AI Interaction](https://www.microsoft.com/en-us/research/blog/guidelines-for-human-ai-interaction-design/), CHI 2019. Eighteen design guidelines, validated with practitioners. Old now, still where I'd start.
- [Learning Outcomes with GenAI in the Classroom](https://www.microsoft.com/en-us/research/wp-content/uploads/2025/10/GenAILearningOutcomes_published_2025-12-16.pdf), MSR-TR-2025-42. Four guidelines for schools, including limiting copy-paste and helping students calibrate what they think they've learned.
- [Psychological Influences of Conversational AI](https://arxiv.org/abs/2607.25057), July 2026. Design directions for reducing psychological harm, framed by the authors as hypotheses rather than findings.
- [From Lived Experience to Insight](https://arxiv.org/abs/2412.07951), FAccT 2025. Design recommendations built from 283 people with lived mental health experience.
- [Evaluating Generative AI Systems is a Social Science Measurement Challenge](https://www.microsoft.com/en-us/research/publication/position-evaluating-generative-ai-systems-is-a-social-science-measurement-challenge/), ICML 2025. How you'd check whether any of the above worked.

## The ones that have nothing to do with technology

These don't come from AI research at all. They come from older work on learning, memory, attention and social connection, and some of it is better evidenced than anything in the sections above.

- **Try to recall it before you look it up.** This is the testing effect, and it's about as solid as psychology gets. Roediger and Karpicke (2006, Psychological Science) had students either reread a passage or practise recalling it. A week later the recall group remembered substantially more, and the rereading group was more confident. Rowland's 2014 meta-analysis put the effect at a medium-to-large size, Adesope and colleagues covered 217 studies in 2017, and Dunlosky's review of ten study techniques rated it one of only two with high utility. **Strong.**
- **Write your own draft before you prompt.** Two separate lines of work. The generation effect (Slamecka and Graf, 1978) shows you remember things you produced yourself better than things you read. Design fixation (Jansson and Smith, 1991, Design Studies) shows that seeing an example narrows the range of what you go on to design, even when you're told to avoid copying it. So drafting first protects both what you remember and how far you range. **Strong for generation, Moderate for fixation.**
- **Ask a person the thing you'd rather ask a machine.** Holt-Lunstad and colleagues (2010, PLoS Medicine) meta-analysed 148 studies and found social connection predicts survival at a magnitude comparable to well-known health risks, and their 2015 follow-up did the same for isolation and loneliness. The Lancet Commission on dementia lists social isolation among the modifiable risk factors. There's also a smaller finding from Ybarra and colleagues (2008) that ten minutes of ordinary conversation improved executive function about as much as ten minutes of puzzles. **Strong for the health outcomes, which are correlational. Moderate for the cognitive effect.**
- **Let yourself be bored.** Weakest one here, and I want to be straight about that. Baird and colleagues (2012, Psychological Science) found an undemanding task during an incubation period improved performance on a creativity test, and Mann and Cadman (2014) found a boring task before idea generation increased output. Both are small and the replication picture is thin. The better-supported cousin is wakeful rest, where Dewar and colleagues (2012, Psychological Science) found that a few quiet minutes after learning improved recall days later. So the case for doing nothing is stronger for memory than for creativity. **Emerging for creativity, Moderate for rest and memory.**
- **Do one thing at a time.** Careful with this one. The famous study is Ophir, Nass and Wagner (2009, PNAS), which found heavy media multitaskers were worse at filtering distraction, and it's been repeated everywhere since. Wiradhany and Nieuwenstein ran [two replications and a meta-analysis in 2017](https://link.springer.com/article/10.3758/s13414-017-1408-4) and concluded the association is questionable. What does hold up is the narrower finding that switching between tasks costs you time and accuracy every time (Monsell, 2003; Rubinstein, Meyer and Evans, 2001). So the honest version isn't "multitaskers have damaged attention," it's "switching is expensive and you pay every time." **Contested for the trait claim, Strong for switch costs.**
- **Notice when you'd rather tell the AI than tell someone.** Pennebaker's expressive writing work (from 1986 onward) found that writing about difficult experiences produced measurable health improvements, which is the part that says offloading to something that isn't a person can genuinely help. The counterweight is the social connection evidence above. Both things are true, and I don't think anyone has studied where the line is. **Moderate, and the specific question is unstudied.**
- **Moving your body.** Erickson and colleagues (2011, PNAS) found aerobic exercise increased hippocampal volume in older adults. Later large trials have been more mixed on cognitive outcomes, so I'd call the brain-structure finding real and the "exercise makes you smarter" version oversold. **Mixed.**
- **Getting rest.** Sleep's role in consolidating memory is one of the better-established findings in neuroscience. Rasch and Born's 2013 review in Physiological Reviews is the standard reference. **Strong.**

These are citations rather than links. I still need to add DOIs for most of them in [SOURCES.md](SOURCES.md).

## What I'd want someone to build

Nothing on this list is a control you can switch on. The closest thing to a real guardrail is showing uncertainty, and that's one study.

### The studies I want

- Something that tests whether a mitigation improves *appropriate* reliance rather than just reducing agreement. Right now we can make people trust AI less. Nobody has shown we can make them trust it more accurately.
- Anything at all on the emotional and social capacities. Every tested mitigation here is about thinking and judgment. Nothing addresses attachment, dependence, or people asking each other for help less.
- A study of what happens when people stop. We know attachment moves in five weeks. We have no idea whether it moves back.
- A direct test of the watermark worry. Does a visible provenance label actually reduce the number of people who go and verify?

### The guardrails I'd try

None of these exist as far as I know. They're extrapolations from the mechanisms above, which means they might be wrong, and a few of them might make things worse in exactly the way the research keeps warning about. That's the point of writing them down.

**Extending what's already tested**

- A confidence gradient inside the answer, not a badge beside it. The colour-coding study worked because it marked which parts were shaky, in place, while you read. Most products do the opposite and put one disclaimer at the bottom.
- A commit-first mode. Say what you think before the model shows you what it thinks. This worked for radiologists and it's a toggle, not a redesign. Useful anywhere the person is supposed to be the decision maker.
- A contribution meter. There's work on measuring how much of a piece of output actually originated with the person. Turn that into something you can see. Not a restriction, just a mirror.
- Ask before you answer, sometimes. If someone asks the same thing they asked last week, prompt them to recall it first. That's the testing effect built into a product instead of assigned as homework.

**The empty half: emotional and social**

- Label everything or label nothing. The implied truth effect says partial labelling makes the unlabelled stuff look safer. If you can't cover a surface, covering half of it may be worse than covering none.
- Show absence as a state. "No provenance information" should look different from a blank space, so that missing evidence reads as missing rather than as fine.
- Watch the shape of the session, not the content of it. Frequency, duration, time of day, escalation over weeks. This is just observability pointed at the human side of the interaction, and it doesn't require reading anybody's messages.
- Offer the human path. When a conversation is about a person in someone's life, surface the option of talking to someone. The evidence that people ask each other less is the thinnest thing in this repo and also the thing I'd most want a product to hedge against.
- Treat persistence as the lever. Attachment appears to be driven by memory and continuity. That makes it a design choice rather than an inevitability, and it means there's a version of an emotional-support context that deliberately doesn't remember. That also makes it less useful to the people getting real benefit, so the trade has to be named, not hidden.
- Make sycophancy a measured property with a threshold. Right now it's a vibe. It should be a number that shows up in evaluation.

**Escalation, the one I think about most at work**

- Route to two people, not one. If human review is the last line of defence, and the research says a single reviewer's judgment quietly erodes, a second opinion is the obvious hedge and nobody builds it in.
- Make the reviewer write their reasoning before seeing the agent's. Same mechanism as commit-first, applied to the oversight step rather than the task.

### How you'd know any of it worked

- Measure accepting the right answers and rejecting the wrong ones separately. An overall agreement rate hides both failure modes.
- Watch for satisfaction going up while outcomes stay flat. That's the pattern that shows up over and over in this research, and it's the one metric combination nobody treats as a warning.
- Keep a holdout group for months, not weeks. Almost every finding here is short. The interesting question is what a year looks like.

Sources are in [SOURCES.md](SOURCES.md). If you know of a tested mitigation I've missed, or you think one of the ideas above would backfire, open an issue.
