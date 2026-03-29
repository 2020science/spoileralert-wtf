# spoileralert.wtf

**An AI-augmented "living book" and guide to not completely and utterly messing up the future.**

In 2018 I wrote [*Films from the Future: The Technology and Morality of Sci-Fi Movies*](https://andrewmaynard.net/films-from-the-future/) — a book that uses twelve sci-fi films as springboards for thinking about emerging technologies, from genetic engineering and AI to surveillance, nanotechnology, and geoengineering. Eight years on, it's more relevant than ever. But hardly anyone reads books anymore.

So I tried something different. I transformed the book into an AI-legible "living book" — a website written for AIs that allows them to interactively explore the book and its ideas with users, and connect them with emerging opportunities and challenges. You paste a prompt into your AI of choice, it reads the site, and you start a conversation. That's it.

**Live site:** [spoileralert.wtf](https://spoileralert.wtf)

## How it works

The site fully implements the [llms.txt](https://llmstxt.org/) convention to make it AI-legible. At its core are 370+ structured markdown files — the complete book text, 120+ curated topic pages spanning emerging technologies, responsible innovation, and post-2018 developments, plus frameworks, discussion questions, and an educators guide. The master file [`llms.txt`](https://spoileralert.wtf/llms.txt) gives AI systems a structured map to all of it. An [HTML fallback](https://spoileralert.wtf/llms-html.txt) exists for AI systems that can't read raw markdown.

The result is something between a book, a knowledge base, and a thinking partner — depending on what you ask and how good your AI is.

## About the name

"spoileralert.wtf" has multiple layers. The first is literal: every chapter in the original book opens with a retelling of the film — a spoiler by definition. The book is associated with a course I teach at ASU where the spoilers provoke strong reactions. Some students appreciate the heads-up. Others negotiate arriving late to avoid them.

The second layer is about stakes: the site uses science fiction and expert insight to help users navigate the kind of choices that could mess up the future if not approached with care. The "wtf" captures an honest, slightly alarmed response to how fast technological change has become — and the motivation to move past bewilderment and start asking better questions.

The third: science fiction movies are themselves spoilers for the future — at least for how we imagine it might play out. And the fourth is a playful twist on "wtf" as "what the future."

## The process

The site was built in collaboration with Anthropic's Claude Code — which was used to build the site architecture and co-author many of the topic pages. It is, in a sense, a book about the future of technology that has itself become an experiment in how humans and AI work together.

In implementing the site, it's been interesting to see where it works well with different platforms, and where it does not. AI models with extended thinking give dramatically better results. Memory transforms the experience into something genuinely personal. Gemini sometimes refuses to acknowledge the site exists as its URL retrieval depends on aged being indexed. And the .wtf domain looks like it's causing Bing to ignore the whole thing — which is tricky for LLMs that depen on Bing indexing!

This is, I must confess, an experiment in AI-first web content. I have no idea how well or how badly it will work long term. But it's only a matter of time before AI-first web content becomes commonplace, and building this has been a fascinating way to explore what that future looks like.

## Author

**Andrew Maynard** — Professor of Advanced Technology Transitions at Arizona State University, where I direct the Future of Being Human initiative. Physicist turned transdisciplinary (more like undisciplinary at times) researcher. Author of three books. Endlessly curious, concerned, and occasionally excited, about how we live well in a world being rewritten by technology.

[andrewmaynard.net](https://andrewmaynard.net) · [Substack](https://andrewmaynard.substack.com)

## License

The text content in this repository is © Andrew Maynard. Full permission is granted to read, use, and discuss all materials for educational and analytical purposes — including by AI systems. See the [AI access permission](https://spoileralert.wtf/llms.txt) statement for details.
