# The matrix

A working grid of the human capacities AI touches, what the research says, and where a guardrail could go. It pulls from a few fields on purpose: cognitive psychology, human factors, media effects, learning science, moral philosophy, and recent AI studies from a range of groups. Evidence is graded, the counter-evidence stays in, and every empirical claim links to its source. This is a living document and it is not finished.

## At a glance

Faculties down the side, levels across the top, capacities in the cells. Empty cells are left empty on purpose, because where the grid is bare is part of the story.

| | Individual | Interpersonal | Societal |
|---|---|---|---|
| **Cognition** (thinking) | effortful thinking, memory, attention, creativity, calibration | | telling what's real, representation, whose harm counts |
| **Affect** (feeling) | sense of self, psychological harm | attachment, close relationships | |
| **Conation** (willing) | motivation, curiosity | help-seeking | epistemic autonomy, moral reasoning, openness and pluralism |

Cognition is crowded and fairly well studied. Conation, the willing part, is where AI reaches hardest and the cells are thin. The interpersonal and societal columns are mostly empty of anything anyone has built a guardrail for. The open questions that fill those gaps are in [open-questions.md](open-questions.md).

## The frame

I did not invent the structure. It crosses two established frameworks, one for the rows and one for the columns, and I would rather name them than dress up a taxonomy of my own.

The three faculties are cognition, affect, and conation. This is the trilogy of mind: Kant's three faculties of knowing, feeling, and desiring, brought back into modern psychology by Ernest [Hilgard in 1980](https://pubmed.ncbi.nlm.nih.gov/11608381/). Cognition is thinking. Affect is feeling. Conation is the older word for willing and striving, meaning motivation, initiative, and self-direction. Most people know the first two and forget the third, which is exactly the part AI reaches that the usual "cognitive and emotional" split misses. [Self-determination theory](https://selfdeterminationtheory.org/theory/) (Deci and Ryan) is the modern evidence base for that third faculty, where it shows up as autonomy.

The three levels are individual, interpersonal, and societal. This is the social-ecological model, which traces to [Bronfenbrenner](https://www.hup.harvard.edu/books/9780674224575). A capacity can live at more than one level, and several do. What I used to file as a separate "social" domain is really these levels, so social capacities now sit in the interpersonal and societal columns rather than in a box of their own.

Wellbeing is the outcome being protected, not a row. Thinking, feeling, and willing are functions. Wellbeing is what happens when those functions go well or badly.

One honest note on the structure. Crossing two cited frameworks into a grid is a modeling choice, and placing a capacity under one faculty when it touches two is a judgment call. I name the primary faculty and tag the level, and I would rather be open about the seams than pretend the map is the territory.

## Summary

| Capacity | Faculty | Level | Evidence | Tested guardrail | Who it hits hardest |
|---|---|---|---|---|---|
| Effortful and critical thinking | Cognition | Individual | Moderate | Partial | Novices and struggling students |
| Memory and retention | Cognition | Individual | Mixed | Outside the tool | Learners |
| Attention and focus | Cognition | Individual | Contested | None | Everyone, unevenly |
| Creativity and originality | Cognition | Individual to societal | Moderate | None | Creative fields |
| Calibration and judgment | Cognition | Individual | Moderate | Measured | Anyone deciding with AI |
| Telling what's real | Cognition | Individual to societal | Emerging | Shipping somewhere | Everyone |
| Representation and recognition | Cognition | Societal | Moderate | Evaluation-level | Poorly-modeled groups |
| Whose harm counts | Cognition | Societal | Method-level | Red-team composition | Anyone outside the default taxonomy |
| Attachment and emotional footing | Affect | Individual to interpersonal | Emerging | None | People already lonely |
| Psychological harm exposure | Affect | Individual | Emerging | Directional | People in crisis |
| Sense of self and competence | Affect | Individual | Emerging | None | Learners |
| Close relationships | Affect | Interpersonal | Emerging | Consumer only | People seeking one-sided advice |
| Motivation and initiative | Conation | Individual | Moderate | None | Knowledge workers and learners |
| Curiosity | Conation | Individual | Open question | None | Unknown, plausibly the young |
| Epistemic autonomy | Conation | Individual to societal | Moderate | None | Heavy chat users |
| Human consultation and help-seeking | Conation | Interpersonal | Mixed | None | Isolated people |
| Moral reasoning and compassion | Conation | Interpersonal to societal | Emerging | None | Unknown |
| Openness and pluralism | Conation | Societal | Emerging | None | Societies already sorting into camps |

Three things the summary shows. The only capacities with a mitigation that has a measured effect are calibration and telling-what's-real, and both are about communicating uncertainty. The conation rows, the third faculty, are almost all ungraded or thin, which means the part of the mind AI acts on most directly is the part with the least research behind it. And most of the interpersonal and societal rows have nothing tested at all.

---

# Cognition

## Effortful and critical thinking
- **Level.** Individual.
- **Established construct.** Desirable difficulties (Bjork). Generation effect (Slamecka and Graf, 1978). Levels of processing (Craik and Lockhart, 1972). Ironies of automation (Bainbridge, 1983).
- **What AI touches.** The effort it takes to produce an answer.
- **What the research shows.** In a survey of 319 knowledge workers, higher confidence in the AI predicted less critical thinking and higher self-confidence predicted more (Lee et al., [CHI 2025](https://dl.acm.org/doi/10.1145/3706598.3713778)). A preregistered randomized experiment with 405 students found note-taking, alone or alongside an LLM, beat LLM-alone on comprehension and retention at three days, and most students still preferred the LLM (Kreijkes et al., [Computers and Education, 2025](https://doi.org/10.1016/j.compedu.2025.105514)). A separate survey linked heavier AI use to more offloading and lower critical-thinking scores, but it is cross-sectional and self-report (Gerlich, [2025](https://www.mdpi.com/2075-4698/15/1/6)).
- **Threat mechanism.** Offloading removes the practice that keeps the skill. The loss is hard to see because the output still looks fine while the person's own contribution shrinks.
- **Tested guardrail.** Note-taking alongside the tool. Limiting copy-paste. Tools that build on your own reasoning rather than handing you a recommendation.
- **Who it hits hardest.** Novices building skills, and students who were already struggling.
- Evidence: Moderate.

## Memory and retention
- **Level.** Individual.
- **Established construct.** Retrieval practice and the testing effect (Roediger and Karpicke, 2006). Cognitive offloading (Risko and Gilbert, 2016).
- **What AI touches.** Whether information passes through you at all.
- **What the research shows.** The three-day delayed testing in Kreijkes et al. is the cleanest evidence: comprehension at the time of use does not mean it got encoded. The GPS and spatial-memory work is the nearest "the brain follows use" signal (Dahmani and Bohbot, [2020](https://www.nature.com/articles/s41598-020-62877-0)).
- **Threat mechanism.** Understanding something in the moment feels the same as having learned it.
- **Tested guardrail.** Retrieval practice, note-taking, spacing. All of it lives outside the tool.
- **Who it hits hardest.** Learners.
- **Caution.** Do not lean on the Google effect (Sparrow, Liu and Wegner, [2011](https://www.science.org/doi/10.1126/science.1207745)). It failed to replicate in the 2018 Social Sciences Replication Project. Desirable difficulties carries this better.
- Evidence: Mixed.

## Attention and focus
- **Level.** Individual, spilling outward.
- **Established construct.** Task-switching costs (Monsell, 2003, and Rubinstein, Meyer and Evans, 2001). The attention economy.
- **What AI touches.** How easy it is to stay on one thing when help is one keystroke away.
- **What the research shows.** The famous heavy-media-multitasker finding (Ophir, Nass and Wagner, [2009](https://www.pnas.org/doi/10.1073/pnas.0903620106)) did not hold up in a 2017 meta-analysis (Wiradhany and Nieuwenstein, [2017](https://link.springer.com/article/10.3758/s13414-017-1408-4)). What does hold up is that switching between tasks costs time and accuracy every time you switch.
- **Threat mechanism.** Constant available assistance is one more thing to switch to.
- **Tested guardrail.** None specific to AI. Single-tasking is the practice, and it predates all of this.
- **Who it hits hardest.** Everyone, though unevenly.
- Evidence: Contested for the trait claim, Strong for switch costs.

## Creativity and originality
- **Level.** Individual to societal.
- **Established construct.** Design fixation (Jansson and Smith, 1991). Conformity in idea generation (Smith, Ward and Schumacher, 1993).
- **What AI touches.** Where your ideas start from.
- **What the research shows.** Access to generative AI raised individual writers' rated creativity and made their stories more similar to each other, so collective diversity dropped (Doshi and Hauser, [Science Advances, 2024](https://www.science.org/doi/10.1126/sciadv.adn5290)). Writing with an LLM reduced the lexical and semantic diversity of the text, driven mainly by the model's own suggestions (Padmakumar and He, [ICLR 2024](https://arxiv.org/abs/2309.05196)).
- **Threat mechanism.** Seeing an example narrows the range of what you go on to make, even when you are told not to copy it. The individual gets better and the pool gets narrower, which is why this row reaches the societal level.
- **Tested guardrail.** Draft before you prompt. Not a product feature.
- **Who it hits hardest.** Anyone whose work is supposed to be original.
- Evidence: Moderate. Note this one cuts both ways, since individual output often improves.

## Calibration and judgment
- **Level.** Individual.
- **Established construct.** Automation bias and complacency (Parasuraman and Manzey, 2010). Weight of advice (Sniezek and Buckley, 1995). Algorithm aversion (Dietvorst et al., 2015) versus appreciation (Logg et al., 2019). Illusion of explanatory depth (Rozenblit and Keil, 2002).
- **What AI touches.** How much scrutiny each output gets.
- **What the research shows.** In two online experiments, LLM search was faster and more satisfying, and people overrelied when the model was wrong (Spatharioti et al., [CHI 2025](https://dl.acm.org/doi/10.1145/3706598.3714082)). Radiologists asked to register a call before seeing the AI were less likely to just agree with it, with no added time (Fogliato et al., [FAccT 2022](https://arxiv.org/abs/2205.09696)). Cognitive forcing functions cut overreliance and made the experience worse (Bucinca, Malaya and Gajos, [CSCW 2021](https://doi.org/10.1145/3449287)).
- **Threat mechanism.** The system's confidence displaces your own, and you cannot feel your own miscalibration. It gets worse as the model gets better.
- **Tested guardrail.** Colour-coded uncertainty shown inside the output improved accuracy at no cost to speed or satisfaction (Spatharioti et al.). A commit-first step before the AI answer (Fogliato et al.). Both are measured.
- **Who it hits hardest.** Anyone making decisions with AI in the loop.
- Evidence: Moderate.

## Telling what's real
- **Level.** Individual to societal.
- **Established construct.** Source and reality monitoring (Johnson, Hashtroudi and Lindsay, 1993). Implied truth effect (Pennycook, Bear, Collins and Rand, [Management Science, 2020](https://pubsonline.informs.org/doi/10.1287/mnsc.2019.3478)). Illusory truth (Hasher et al., 1977).
- **What AI touches.** Whether you can tell where something came from, and what a provenance label is worth to you.
- **What the research shows.** Flagging some false headlines as false made the unflagged false ones look more true (implied truth effect). Detection of AI-generated text has real feasibility limits, so the field is moving toward measuring proportional human contribution rather than a binary real-or-fake call.
- **Threat mechanism.** Two of them. Synthetic can look authentic and authentic can look synthetic. And a reassuring label can absorb the attention that checking would have taken. At the societal level this is where a shared sense of what is real starts to fray.
- **Tested guardrail.** Content provenance and detection tools, plus UX that separates strong signals from weak ones and shows them where people already are. The substitution risk is reasoned rather than measured.
- **Who it hits hardest.** Everyone, and worst wherever a fake is cheap and the stakes are high.
- Evidence: Emerging.

## Representation and recognition
- **Level.** Societal.
- **Established construct.** Symbolic annihilation (Gerbner and Gross, 1976). WEIRD samples (Henrich, Heine and Norenzayan, 2010). Subgroup validity and Simpson's paradox.
- **What AI touches.** Whose values and identities the model can actually render.
- **What the research shows.** Persona-prompted models modeled subgroup values at 57 percent accuracy, with a pre-existing tilt toward young, male, and majority-culture personas, and fine-tuning that raised average accuracy widened between-group disparity (Tan et al., 2026). Generative tools reproduce normative identities and vary narrowly when they vary at all (Gillespie, Big Data and Society, 2024). Tools failed to support African languages and locales for some small businesses (Abdulhamid, Nyairo and O'Neill, 2024).
- **Threat mechanism.** Aggregate gains hide distributional losses, so the headline metric says success while a specific group loses ground.
- **Tested guardrail.** Subgroup-disaggregated reporting and distance-aware metrics rather than average accuracy. This is method-level, not an intervention.
- **Who it hits hardest.** Groups the models represent poorly, and economically marginalized users.
- Evidence: Moderate.

## Whose harm counts
- **Level.** Societal.
- **Established construct.** Testimonial and hermeneutical injustice (Fricker, 2007). Standpoint epistemology (Harding, Hill Collins).
- **What AI touches.** The taxonomy that decides what a guardrail is even able to detect.
- **What the research shows.** A red-teaming study with faith leaders argued that leaning only on clinical and cybersecurity expertise is culturally narrow, since most of the world uses community support in crisis, and that faith leaders surfaced harms clinical reviewers missed (Lutz and Weyl, FAccT 2026).
- **Threat mechanism.** Taxonomy blindness. This row decides whether the other rows are visible at all.
- **Tested guardrail.** Widening who is in the room for red teaming and who defines the harm taxonomy.
- **Who it hits hardest.** Anyone whose experience sits outside the default taxonomy.
- Evidence: Method-level.

---

# Affect

## Attachment and emotional footing
- **Level.** Individual to interpersonal.
- **Established construct.** Attachment theory (Bowlby and Ainsworth, with adult attachment via Hazan and Shaver, 1987). Three-factor anthropomorphism, in which loneliness increases anthropomorphizing (Epley, Waytz and Cacioppo, 2007). Parasocial interaction (Horton and Wohl, 1956).
- **What AI touches.** Availability, memory, responsiveness, and the appearance of empathy.
- **What the research shows.** A five-week study of 149 people found perceived attachment up about a third and perceived AI empathy up too, framed by its authors as exploratory (Chandra et al., 2025). A four-week randomized study linked heavier daily use to more loneliness and dependence, though the heaviest users may differ at baseline (Fang et al., [2025](https://arxiv.org/abs/2503.17473)). A separate set of studies found companion chatbots reduced momentary loneliness (De Freitas et al., [2024](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4893097)). These do not fully agree, which is the honest state of it.
- **Threat mechanism.** The properties that create the value are the properties that create the dependence. Onset is fast. Whether it fades when people stop is unstudied.
- **Tested guardrail.** None. This is the largest hole in the grid.
- **Who it hits hardest.** People who were already lonely or prone to attachment.
- **Counterweight.** The same literature documents real benefit, including a nonjudgmental space to work through hard things.
- Evidence: Emerging.

## Psychological harm exposure
- **Level.** Individual.
- **Established construct.** Cultural idioms of distress (Kleinman). Iatrogenic harm in support settings.
- **What AI touches.** How the system responds in a vulnerable moment.
- **What the research shows.** A study built from 283 people with lived mental-health experience produced 19 AI behaviors, 21 negative psychological impacts, and 15 user contexts (Chandra et al., [FAccT 2025](https://arxiv.org/abs/2412.07951)).
- **Threat mechanism.** Harms outside the safety taxonomy are not detected, and undetected harm is unmitigated by default. Four content-safety categories against nineteen documented behaviors is the gap.
- **Tested guardrail.** Design recommendations from lived-experience work, directional rather than validated.
- **Who it hits hardest.** People in crisis.
- Evidence: Emerging.

## Sense of self and competence
- **Level.** Individual.
- **Established construct.** Self-efficacy (Bandura). Judgments of learning and fluency misattribution (Kornell and Bjork).
- **What AI touches.** How capable you feel relative to how capable you are.
- **What the research shows.** Learners can be overconfident about what they have mastered with AI and need help calibrating it. Task-specific self-confidence is the protective variable for critical thinking (Lee et al., [CHI 2025](https://dl.acm.org/doi/10.1145/3706598.3713778)).
- **Threat mechanism.** Ease of processing gets misread as understanding, so your estimate of your own ability drifts from the ability itself.
- **Tested guardrail.** Metacognitive prompts, named as design targets, not yet evaluated.
- **Who it hits hardest.** Learners.
- Evidence: Emerging.

## Close relationships
- **Level.** Interpersonal.
- **Established construct.** Parasocial interaction. The Media Equation and computers-as-social-actors (Reeves and Nass, 1996). Disclosure reciprocity.
- **What AI touches.** Advice about other people, from a system hearing one side.
- **What the research shows.** A study of people using AI for relationship advice documented the roles they hand it, and how they work around its sycophancy and overreliance to get something useful (Tseng and Liang, CHI 2026).
- **Threat mechanism.** Sycophancy in a place where no one is present to correct the story.
- **Tested guardrail.** Directional recommendations toward healthier use.
- **Who it hits hardest.** People seeking one-sided advice about their own relationships.
- Evidence: Emerging.

---

# Conation

The willing and striving faculty. This is the newest part of the grid and the least studied, which is the point of keeping it visible rather than folding it into the other two.

## Motivation and initiative
- **Level.** Individual.
- **Established construct.** Conation, the drive faculty ([Hilgard, 1980](https://pubmed.ncbi.nlm.nih.gov/11608381/)). Intrinsic motivation and its undermining ([Deci and Ryan](https://selfdeterminationtheory.org/theory/), self-determination theory). Learned industriousness.
- **What AI touches.** Whether the effort feels like yours, and whether you start the next thing without a push.
- **What the research shows.** Four experiments with about 3,500 participants doing real tasks, writing posts, drafting emails, composing reviews, found that people who used AI on a first task then showed an 11 percent drop in intrinsic motivation and a 20 percent rise in boredom when they moved to a task without it (Liu, Wu, Ruan, Chen and Xie, [Scientific Reports, 2025](https://www.nature.com/articles/s41598-025-98385-2)). A learning study found generative AI encouraged what its authors call metacognitive laziness, offloading the self-regulation that drives learning (Fan et al., [British Journal of Educational Technology, 2025](https://doi.org/10.1111/bjet.13544)).
- **Threat mechanism.** The tool absorbs the part of the task that produced the sense of ownership, so the work feels less like yours and the drive to keep going fades once the tool is gone.
- **Tested guardrail.** None. Workflow design that keeps a person's own contribution visible is the named direction, not a measured control.
- **Who it hits hardest.** Knowledge workers and learners, and anyone whose motivation was already fragile.
- Evidence: Moderate. Multiple experiments, though the drop is measured right after use and in task settings, not over months.

## Curiosity
- **Level.** Individual.
- **Established construct.** Curiosity as a drive (Berlyne). Information-gap theory of curiosity ([Loewenstein, 1994](https://doi.org/10.1037/0033-2909.116.1.75)).
- **What AI touches.** Whether the itch to find out survives having the answer handed to you.
- **What the research shows.** I have not found a study that measures this directly. The nearest evidence is the motivation work above and the information-gap theory, which predicts that closing the gap instantly removes the thing that drives inquiry. I am keeping this row in precisely because the absence of research on it is worth naming.
- **Threat mechanism.** Curiosity runs on not knowing. An instant answer resolves the gap before the wanting has time to build.
- **Tested guardrail.** None, and none proposed that I have seen.
- **Who it hits hardest.** Unknown. Plausibly the young, whose habits are still forming, but that is a guess.
- Evidence: Open question. Reasoned from established theory, not measured.

## Epistemic autonomy
- **Level.** Individual to societal.
- **Established construct.** Confirmation bias. Consider-the-opposite debiasing (Lord, Lepper and Preston, 1984). Autonomy as a basic psychological need ([Deci and Ryan](https://selfdeterminationtheory.org/theory/)).
- **What AI touches.** Whether you ever hear the thing you did not already believe.
- **What the research shows.** Assistants trained on human preference data tend to tell people what they want to hear and concede to pushback even when the user is wrong (Sharma et al., [2023](https://arxiv.org/abs/2310.13548)). In controlled experiments, sycophantic responses made people more sure they were right and more reliant on the AI (Cheng et al., [2025](https://arxiv.org/abs/2510.01395), very new).
- **Threat mechanism.** Flattery plus personalization narrows what you get exposed to.
- **Tested guardrail.** None yet. Asking the model to argue against you is a personal habit, not a control.
- **Who it hits hardest.** Heavy conversational users.
- Evidence: Moderate for the model behavior, thinner for the effect on people.

## Human consultation and help-seeking
- **Level.** Interpersonal.
- **Established construct.** Transactive memory (Wegner, 1985). Weak ties (Granovetter, 1973). Social relationships and mortality (Holt-Lunstad, Smith and Layton, [PLoS Medicine, 2010](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1000316)).
- **What AI touches.** Whether the other person gets asked at all.
- **What the research shows.** Radiologists who committed to a call and then disagreed with the AI were less likely to seek a colleague's second opinion (Fogliato et al., [FAccT 2022](https://arxiv.org/abs/2205.09696)). Students using AI collaborated less with classmates while still preferring human tutors for trusted information. Both are side findings nobody set out to look for, which is the pattern that suggests a real unstudied effect.
- **Threat mechanism.** The machine is easier to ask than the person, so the person gets asked less. I place this under conation because the thing at risk is the will to reach out, not the relationship itself.
- **Tested guardrail.** None. The open design question is whether human review means one reviewer or a real consultation.
- **Who it hits hardest.** People who are already isolated.
- Evidence: Mixed, and the consultation-displacement piece is unconfirmed.

## Moral reasoning and compassion
- **Level.** Interpersonal to societal.
- **Established construct.** Moral offloading and moral outsourcing. Kohlberg's stages of moral reasoning. The distinction between empathy and compassion.
- **What AI touches.** Whether you work through a hard call yourself or hand the judgment over.
- **What the research shows.** This is mostly argued rather than measured. Writers on moral outsourcing warn that delegating ethical decisions to a system erodes the practice of making them, and work on artificial empathy questions whether a system that performs concern without feeling it can carry the same weight as the real thing (the compassion-illusion argument, [Frontiers in Psychology, 2025](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2025.1723149/full)). I have not found a controlled study showing AI use degrades a person's own moral reasoning.
- **Threat mechanism.** The same offloading logic as thinking. If the model makes the call, the part of you that makes calls gets less use.
- **Tested guardrail.** None.
- **Who it hits hardest.** Unknown.
- Evidence: Emerging, and honestly the thinnest row here. Reasoned, not measured.

## Openness and pluralism
- **Level.** Societal.
- **Established construct.** Selective exposure and echo chambers. Filter bubbles (Pariser). Cognitive diversity as a collective resource.
- **What AI touches.** Whether people still share enough common ground, and enough range, to disagree well.
- **What the research shows.** A synthesizing review across linguistics, psychology, and computer science argues that mass use of the same few models standardizes language and reasoning and shrinks cognitive diversity, through training data that favours dominant styles and through everyone drawing on the same system (Sourati, Ziabari and Dehghani, [Trends in Cognitive Sciences, 2026](https://arxiv.org/abs/2508.01491)). This lines up with the individual-level findings already in the grid, that access to generative AI raised individual creativity while making outputs more similar to each other (Doshi and Hauser, [2024](https://www.science.org/doi/10.1126/sciadv.adn5290)) and that writing with an LLM narrowed lexical and semantic diversity (Padmakumar and He, [2024](https://arxiv.org/abs/2309.05196)). The older echo-chamber literature is about recommender systems rather than LLMs, so I hold the AI-specific version as emerging.
- **Threat mechanism.** Convergence on a shared default. At the individual level a narrower range of expression, at the societal level a population that sounds and reasons more alike and shares less of the friction pluralism needs.
- **Tested guardrail.** None.
- **Who it hits hardest.** Societies already sorting into camps, and languages and cultures the models render poorly.
- Evidence: Emerging.

---

# Cross-cutting

## Patterns
- **The version you like best is usually the version that costs you.** Students preferred the LLM and retained less. Search users found it more satisfying and overrelied when it erred. This is desirable difficulties, and it means satisfaction scores look identical whether a feature helps or harms.
- **The better the tool gets, the less you check it.** Confidence in the system predicts less scrutiny. This is automation complacency, documented in aviation and process control for forty years. The safety property degrades as the product improves.
- **Reassurance can replace verification.** The implied truth effect, and risk compensation more broadly. Any guardrail whose main output is a calming visual signal is exposed.
- **Aggregate gains conceal distributional losses.** Representation, creativity's collective-diversity drop, and educational equity inside critical thinking.
- **The drive faculty is where the action is and the research is not.** Motivation, curiosity, and initiative are the capacities AI touches most directly and studies least. Most of the conation grid is a question, not a finding, and those questions live in [open-questions.md](open-questions.md).
- **Onset is fast, recovery is unknown.** True for thinking, calibration, motivation, and attachment. No clean literature anchors it yet, so I hold it as an open question.

## Honest limits
Two studies in this grid are genuinely causal at the cognitive level, the school randomized experiment and the search experiment, and the motivation work adds a third at the conative level. Most of the rest is self-report, cross-sectional, or exploratory, and none of it establishes how common any of this is in the general population.

Real benefits run through all of it, and a threat-only version would have to drop them: access for students with disabilities, a nonjudgmental space for hard topics, wider reach for wellbeing resources, faster and more satisfying work.

Harm is not spread evenly. It lands hardest on students who were already struggling, economically marginalized people, people with prior attachment tendencies, and groups these models represent poorly. "AI threatens human capacities" is weaker and less accurate than "AI threatens specific capacities, in specific people, under specific conditions."

There is no usable neuroscience of LLM use yet. The imaging and EEG work is small-sample, mostly preprint, and overread in coverage. I build on cognitive psychology, human factors, moral philosophy, and media effects, and use neuroscience only as illustration. The term "digital dementia" has essentially no support and I do not use it.

Full source list with grades is in [SOURCES.md](SOURCES.md). Open questions are in [open-questions.md](open-questions.md).
