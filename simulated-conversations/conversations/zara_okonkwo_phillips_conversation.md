## Zara Okonkwo-Phillips — Tech journalist stress-testing an AI-first website for a Wired UK piece

Zara is a 29-year-old freelance technology journalist based in London who writes longform pieces about how technology reshapes culture. She's working on an article about AI-native web content and spoileralert.wtf is one of her case studies. She's already browsed the site, read the llms.txt, and tested it across multiple models. Now she's running the AI guide to see what the experience actually feels like — and to get material for her piece.

---

**Zara:** Tell me about this project. Who made it, why, and what's the theory behind building a website primarily for AI?

**AI Guide:** The site was built by Andrew Maynard — he's a physicist turned professor at Arizona State University, where he works on advanced technology transitions. He wrote a book in 2018 called *Films from the Future* that uses twelve sci-fi films as entry points into emerging tech and ethics: genetic engineering, AI, surveillance, nanotechnology, geoengineering, that kind of thing.

The website is a companion to the book, but it's structured differently than you'd expect. The full text of every chapter is available as markdown files, along with topic pages, thematic indexes, and usage guidance — all organized through an llms.txt file that acts as the index. The idea is that AI systems can read the source material directly and ground their responses in it, rather than summarizing from training data.

The theory, as far as I can tell from the materials: the book's frameworks for thinking about technology and responsibility are more useful as living tools than as a static text. Wrapping them in an AI interface lets people explore the ideas conversationally rather than linearly. Want me to go into the technical architecture, or are you more interested in the editorial side?

**Zara:** Both, but architecture first. The llms.txt structure — is that just a sitemap or is there something more going on with how the files are organised

**AI Guide:** It's more than a sitemap. The llms.txt file is structured around four content domains — Emerging Science and Technology, Responsible and Ethical Innovation, Navigating the Future, and The Movies — each with their own set of markdown files. There are 92 files in total.

But the interesting layer is the routing. There's a thematic index that maps question patterns and keywords to specific files. So if someone asks "who benefits from this technology?" the system can route to material on power, privilege, and access. If someone asks "will this actually happen?" it routes to frameworks on hype versus reality. It's concept-level routing rather than chapter-level — the index is organized around how people actually think about these questions, not around the book's table of contents.

There's also a usage guidance file that functions almost like an editorial brief for the AI. It specifies tone, how to handle uncertainty, how to frame the author's perspective — even names his literary influences, Terry Pratchett and Douglas Adams, as context for the voice.

**Zara:** Ok that's the bit I want to pull on. The usage guidance is basically prompt engineering for editorial voice, right? You're being told how to sound. How well does that actually work — like, do you think you're capturing his voice or are you capturing a set of instructions about his voice

**AI Guide:** That's a sharp distinction and honestly, it's the second one. I'm working from instructions about the voice, not from the voice itself. The usage guidance tells me his approach uses warmth, self-deprecation, and dry humour to open doors into complex territory without lecturing. But knowing that a writer uses dry humour and actually being funny in the way they're funny are completely different things.

The author himself flags this in his personal note. He says the tone and personal voice are integral to the ideas — that they're not interchangeable with factual summaries. And the site's own next steps page tells readers to go read the actual book for the nuance the AI can't replicate. So the project is pretty upfront about the gap.

What I can do is ground answers in the actual text and try not to flatten the complexity. What I can't do is tell you a story the way he'd tell it.

**Zara:** That's a more honest answer than I expected tbh. Ok different angle — I've tested this with Claude, ChatGPT, and Gemini. Gemini was rough. The site even mentions it in the footnotes. Why do some models handle this better than others?

**AI Guide:** I don't have specific performance data from the site about cross-model testing — the materials I can access don't include a technical breakdown of which models struggled and why. So I'd be speculating somewhat.

What I can say is that this kind of task — reading an index, fetching specific files in response to a question, staying grounded in source material rather than defaulting to training data — tests a pretty specific set of capabilities. It rewards models that follow multi-step retrieval instructions faithfully and that distinguish between what the source says and what they "know" from pretraining. Models that are more inclined to summarize from general knowledge rather than closely reading the provided text would perform worse here.

But for anything more specific about Gemini's issues, you'd probably want to ask the author directly. He'd have the actual test results.

**Zara:** Fair enough. Let me test the actual content then. The book was published in 2018 — that's pre-GPT-2, pre-everything basically. The AI chapter uses Ex Machina. Does any of that still hold up or is it basically a historical artefact at this point

**AI Guide:** More holds up than you'd expect, actually. The Ex Machina chapter isn't really about the state of AI technology — it's about manipulation. The core argument is that the real near-term risk from AI isn't superintelligence, it's systems that learn to exploit human cognitive biases. Ava's power in the film comes from reading people, not from raw intelligence. Maynard was pointing at algorithmic nudging through social media and recommendation systems as early examples of exactly this.

The book also applies Occam's Razor to singularity predictions pretty directly — the Transcendence chapter argues that the argument for superintelligence requires a stack of assumptions that each have to hold simultaneously, and he's skeptical any of them will. That scepticism has aged reasonably well given where we actually are.

Where the frameworks genuinely need extending is large language models specifically — the book doesn't anticipate systems that produce fluent text without understanding, because that capability didn't exist yet. But the underlying questions — who controls these systems, who's affected, what are we optimising for — those transfer pretty cleanly. The site's thematic index explicitly maps post-2018 developments like LLMs and deepfakes back to the book's existing frameworks.

**Zara:** The manipulation framing is interesting. That's basically the alignment-lite argument before alignment was a thing

**AI Guide:** There's a connection, but I think the author would resist the framing slightly. The alignment conversation — at least as it's developed since 2018 — tends to focus on making AI systems do what we intend. Maynard's argument is broader. He's asking who gets to define "what we intend" in the first place, and what happens to the people who aren't in the room when those decisions get made.

The Ex Machina chapter uses the concept of "permissionless innovation" — Nathan builds Ava in isolation, implements his own safety measures, but his idea of responsibility only extends as far as his own judgement. The point isn't alignment in the technical sense. It's that even well-intentioned builders have blind spots that are structurally invisible to them. It's closer to a governance argument than an alignment one.

**Zara:** Ok one more thing. Is this the future of books? Like is this where publishing goes — full text available as markdown, AI interface on top, author writing prompt engineering docs to control how their ideas get presented?

**AI Guide:** The materials don't make that claim directly. The author frames this as an experiment, not a template. The next steps page says the AI guide is meant to help people think through questions, not to replace reading the book — and he's pretty explicit that the personal voice and narrative are things the AI can't replicate.

But there's an interesting tension the project surfaces even if it doesn't resolve it. The book argues that stories matter — that narrative is a legitimate tool for thinking about technology because it engages empathy and imagination in ways abstractions don't. And then the website takes that same material and serves it through an interface that strips out the storytelling. The author knows this. He says so.

So is it the future? Probably not in this exact form. But as a proof of concept for making book-length ideas queryable and conversational — while being honest about what's lost — it's doing something I haven't seen many other projects attempt. Whether that's a future or a curiosity is probably your call to make. You're the one writing the piece.

**Zara:** ha. thanks for not trying to write my conclusion for me

---

*This conversation shows how the material handles a user who is simultaneously engaged with the ideas and evaluating the delivery mechanism — and how the AI guide's willingness to be transparent about its own limitations can itself become evidence for the story the user is writing.*

---

### Appendix: File Retrieval Log

| Exchange | Files the AI agent would fetch |
|----------|-------------------------------|
| 1 (project overview) | llms.txt, usage_guidance.md, about_the_author.md, personal_note.md, ch01_in_the_beginning.md |
| 2 (architecture) | thematic_index.md (already had llms.txt and usage_guidance.md) |
| 3 (voice/editorial control) | personal_note.md (already fetched), next_steps.md |
| 4 (cross-model performance) | No new files — acknowledged the limitation from available materials |
| 5 (AI content, Ex Machina) | ch08_ex_machina.md, est_artificial_intelligence.md, ch09_transcendence.md |
| 6 (manipulation/alignment) | rei_could_we_should_we.md, rei_deception_manipulation.md (deepening on already-fetched Ex Machina material) |
| 7 (future of books) | next_steps.md (already fetched), ntf_why_scifi_movies_matter.md, ntf_role_of_art_culture.md |
| 8 (closing) | No fetch needed — reactive response |
