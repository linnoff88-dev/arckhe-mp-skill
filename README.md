<p align="center">
  <img alt="MP SKILL â€” Skills para agentes de IA" src="assets/readme-hero.png" />
</p>

# mp-skill â€” Skills para Agentes de IA (PT-BR)

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Fork em portuguÃªs do repositÃ³rio **[mattpocock/skills](https://github.com/mattpocock/skills)** â€” uma coleÃ§Ã£o de skills (slash commands e behaviors) para Claude Code, Codex e outros agentes â€” com traduÃ§Ã£o PT-BR e um **curso completo** sobre como usar tudo isso na prÃ¡tica.

> _"NÃ£o Ã© sobre 'promptar melhor'. Ã‰ sobre construir sistemas reutilizÃ¡veis de raciocÃ­nio."_

---

## ðŸŽ“ Curso: Skills For Real Engineers (PT-BR)

Curso completo em portuguÃªs explicando os fundamentos, a estrutura do repositÃ³rio e o uso avanÃ§ado das skills. **14 pÃ¡ginas HTML** divididas em 3 trilhas:

| Trilha | Cor | ConteÃºdo |
|--------|-----|----------|
| **T1 â€” Fundamentos** ðŸŒ± | Emerald | Os 4 problemas que skills resolvem (desalinhamento, verbosidade, cÃ³digo quebrado, ball of mud). 6 mÃ³dulos sobre grilling, linguagem ubÃ­qua, TDD+diagnose, arquitetura e workflow completo. |
| **T2 â€” Sobre o RepositÃ³rio** ðŸ“¦ | Blue | Origem do projeto, filosofia, estrutura de pastas e instalaÃ§Ã£o. 3 mÃ³dulos. |
| **T3 â€” Uso AvanÃ§ado** ðŸ§© | Purple | ComposiÃ§Ã£o de skills, customizaÃ§Ã£o e integraÃ§Ã£o cross-runtime (Claude Code, Codex, MCP, CI/CD). 3 mÃ³dulos. |

**ðŸ‘‰ Acesse o curso: [inematds.github.io/mp-skill/curso-skills/](https://inematds.github.io/mp-skill/curso-skills/)**

Os arquivos do curso ficam em [`curso-skills/`](./curso-skills/).

---

## ðŸ“‚ O que tem neste repositÃ³rio

| Pasta | ConteÃºdo |
|-------|----------|
| **[`skills/`](./skills/)** | As skills propriamente ditas, organizadas em buckets: `engineering/` (10 skills de cÃ³digo diÃ¡rio), `productivity/` (workflow nÃ£o-cÃ³digo), `misc/` (uso raro), `personal/`, `in-progress/`, `deprecated/`. |
| **[`curso-skills/`](./curso-skills/)** | Curso PT-BR em HTML estÃ¡tico no formato INEMA.CLUB â€” landing + 3 trilhas + 12 mÃ³dulos. |
| **[`docs/pt-BR/`](./docs/pt-BR/)** | TraduÃ§Ã£o PT-BR do README, do CONTEXT.md e Ã­ndice de todas as skills. |
| **[`CONTEXT.md`](./CONTEXT.md)** | Linguagem ubÃ­qua do repo â€” termos canÃ´nicos (Issue tracker, Issue, Triage role). |
| **[`CLAUDE.md`](./CLAUDE.md)** | ConvenÃ§Ãµes do projeto carregadas automaticamente pelo Claude Code. |
| **[`.claude-plugin/plugin.json`](./.claude-plugin/plugin.json)** | Manifest do plugin pra Claude Code descobrir as skills. |

### Skills disponÃ­veis (resumo)

**Engineering** â€” `diagnose`, `grill-with-docs`, `triage`, `improve-codebase-architecture`, `setup-matt-pocock-skills`, `tdd`, `to-issues`, `to-prd`, `zoom-out`, `prototype`

**Productivity** â€” `grill-me`, `handoff`, e outras de workflow

**Misc** â€” skills mantidas para uso raro

Lista completa traduzida em [`docs/pt-BR/skills-pt-BR.md`](./docs/pt-BR/skills-pt-BR.md).

---

## ðŸš€ InstalaÃ§Ã£o rÃ¡pida

```bash
npx skills@latest add mattpocock/skills
```

Selecione `/setup-matt-pocock-skills` na lista, depois rode esse comando dentro do seu agente. Detalhes no [MÃ³dulo 2.3 do curso](https://inematds.github.io/mp-skill/curso-skills/curso/trilha2/modulo-2-3.html).

---

## ðŸŒ VersÃµes em outros idiomas

- **ðŸ‡§ðŸ‡· README em PT-BR (estendido):** [`docs/pt-BR/README.pt-BR.md`](./docs/pt-BR/README.pt-BR.md)
- **ðŸ‡ºðŸ‡¸ README original em inglÃªs:** seguir abaixo â†“

---

<p>
  <a href="https://www.aihero.dev/s/skills-newsletter">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://res.cloudinary.com/total-typescript/image/upload/v1777382277/skills-repo-dark_2x.png">
      <source media="(prefers-color-scheme: light)" srcset="https://res.cloudinary.com/total-typescript/image/upload/v1777382277/skill-repo-light_2x.png">
      <img alt="Skills" src="https://res.cloudinary.com/total-typescript/image/upload/v1777382277/skill-repo-light_2x.png" width="369">
    </picture>
  </a>
</p>

# Skills For Real Engineers

[![skills.sh](https://skills.sh/b/mattpocock/skills)](https://skills.sh/mattpocock/skills)

My agent skills that I use every day to do real engineering - not vibe coding.

Developing real applications is hard. Approaches like GSD, BMAD, and Spec-Kit try to help by owning the process. But while doing so, they take away your control and make bugs in the process hard to resolve.

These skills are designed to be small, easy to adapt, and composable. They work with any model. They're based on decades of engineering experience. Hack around with them. Make them your own. Enjoy.

If you want to keep up with changes to these skills, and any new ones I create, you can join ~60,000 other devs on my newsletter:

[Sign Up To The Newsletter](https://www.aihero.dev/s/skills-newsletter)

## Quickstart (30-second setup)

1. Run the skills.sh installer:

```bash
npx skills@latest add mattpocock/skills
```

2. Pick the skills you want, and which coding agents you want to install them on. **Make sure you select `/setup-matt-pocock-skills`**.

3. Run `/setup-matt-pocock-skills` in your agent. It will:
   - Ask you which issue tracker you want to use (GitHub, Linear, or local files)
   - Ask you what labels you apply to tickets when you triage them (`/triage` uses labels)
   - Ask you where you want to save any docs we create

4. Bam - you're ready to go.

## Why These Skills Exist

I built these skills as a way to fix common failure modes I see with Claude Code, Codex, and other coding agents.

### #1: The Agent Didn't Do What I Want

> "No-one knows exactly what they want"
>
> David Thomas & Andrew Hunt, [The Pragmatic Programmer](https://www.amazon.co.uk/Pragmatic-Programmer-Anniversary-Journey-Mastery/dp/B0833F1T3V)

**The Problem**. The most common failure mode in software development is misalignment. You think the dev knows what you want. Then you see what they've built - and you realize it didn't understand you at all.

This is just the same in the AI age. There is a communication gap between you and the agent. The fix for this is a **grilling session** - getting the agent to ask you detailed questions about what you're building.

**The Fix** is to use:

- [`/grill-me`](./skills/productivity/grill-me/SKILL.md) - for non-code uses
- [`/grill-with-docs`](./skills/engineering/grill-with-docs/SKILL.md) - same as [`/grill-me`](./skills/productivity/grill-me/SKILL.md), but adds more goodies (see below)

These are my most popular skills. They help you align with the agent before you get started, and think deeply about the change you're making. Use them _every_ time you want to make a change.

### #2: The Agent Is Way Too Verbose

> With a ubiquitous language, conversations among developers and expressions of the code are all derived from the same domain model.
>
> Eric Evans, [Domain-Driven-Design](https://www.amazon.co.uk/Domain-Driven-Design-Tackling-Complexity-Software/dp/0321125215)

**The Problem**: At the start of a project, devs and the people they're building the software for (the domain experts) are usually speaking different languages.

I felt the same tension with my agents. Agents are usually dropped into a project and asked to figure out the jargon as they go. So they use 20 words where 1 will do.

**The Fix** for this is a shared language. It's a document that helps agents decode the jargon used in the project.

<details>
<summary>
Example
</summary>

Here's an example [`CONTEXT.md`](https://github.com/mattpocock/course-video-manager/blob/076a5a7a182db0fe1e62971dd7a68bcadf010f1c/CONTEXT.md), from my `course-video-manager` repo. Which one is easier to read?

- **BEFORE**: "There's a problem when a lesson inside a section of a course is made 'real' (i.e. given a spot in the file system)"
- **AFTER**: "There's a problem with the materialization cascade"

This concision pays off session after session.

</details>

This is built into [`/grill-with-docs`](./skills/engineering/grill-with-docs/SKILL.md). It's a grilling session, but that helps you build a shared language with the AI, and document hard-to-explain decisions in ADR's.

It's hard to explain how powerful this is. It might be the single coolest technique in this repo. Try it, and see.

> [!TIP]
> A shared language has many other benefits than reducing verbosity:
>
> - **Variables, functions and files are named consistently**, using the shared language
> - As a result, the **codebase is easier to navigate** for the agent
> - The agent also **spends fewer tokens on thinking**, because it has access to a more concise language

### #3: The Code Doesn't Work

> "Always take small, deliberate steps. The rate of feedback is your speed limit. Never take on a task thatâ€™s too big."
>
> David Thomas & Andrew Hunt, [The Pragmatic Programmer](https://www.amazon.co.uk/Pragmatic-Programmer-Anniversary-Journey-Mastery/dp/B0833F1T3V)

**The Problem**: Let's say that you and the agent are aligned on what to build. What happens when the agent _still_ produces crap?

It's time to look at your feedback loops. Without feedback on how the code it produces actually runs, the agent will be flying blind.

**The Fix**: You need the usual tranche of feedback loops: static types, browser access, and automated tests.

For automated tests, a red-green-refactor loop is critical. This is where the agent writes a failing test first, then fixes the test. This helps give the agent a consistent level of feedback that results in far better code.

I've built a **[`/tdd`](./skills/engineering/tdd/SKILL.md) skill** you can slot into any project. It encourages red-green-refactor and gives the agent plenty of guidance on what makes good and bad tests.

For debugging, I've also built a **[`/diagnose`](./skills/engineering/diagnose/SKILL.md)** skill that wraps best debugging practices into a simple loop.

### #4: We Built A Ball Of Mud

> "Invest in the design of the system _every day_."
>
> Kent Beck, [Extreme Programming Explained](https://www.amazon.co.uk/Extreme-Programming-Explained-Embrace-Change/dp/0321278658)

> "The best modules are deep. They allow a lot of functionality to be accessed through a simple interface."
>
> John Ousterhout, [A Philosophy Of Software Design](https://www.amazon.co.uk/Philosophy-Software-Design-2nd/dp/173210221X)

**The Problem**: Most apps built with agents are complex and hard to change. Because agents can radically speed up coding, they also accelerate software entropy. Codebases get more complex at an unprecedented rate.

**The Fix** for this is a radical new approach to AI-powered development: caring about the design of the code.

This is built in to every layer of these skills:

- [`/to-prd`](./skills/engineering/to-prd/SKILL.md) quizzes you about which modules you're touching before creating a PRD
- [`/zoom-out`](./skills/engineering/zoom-out/SKILL.md) tells the agent to explain code in the context of the whole system

And crucially, [`/improve-codebase-architecture`](./skills/engineering/improve-codebase-architecture/SKILL.md) helps you rescue a codebase that has become a ball of mud. I recommend running it on your codebase once every few days.

### Summary

Software engineering fundamentals matter more than ever. These skills are my best effort at condensing these fundamentals into repeatable practices, to help you ship the best apps of your career. Enjoy.

## Reference

### Engineering

Skills I use daily for code work.

- **[diagnose](./skills/engineering/diagnose/SKILL.md)** â€” Disciplined diagnosis loop for hard bugs and performance regressions: reproduce â†’ minimise â†’ hypothesise â†’ instrument â†’ fix â†’ regression-test.
- **[grill-with-docs](./skills/engineering/grill-with-docs/SKILL.md)** â€” Grilling session that challenges your plan against the existing domain model, sharpens terminology, and updates `CONTEXT.md` and ADRs inline.
- **[triage](./skills/engineering/triage/SKILL.md)** â€” Triage issues through a state machine of triage roles.
- **[improve-codebase-architecture](./skills/engineering/improve-codebase-architecture/SKILL.md)** â€” Find deepening opportunities in a codebase, informed by the domain language in `CONTEXT.md` and the decisions in `docs/adr/`.
- **[setup-matt-pocock-skills](./skills/engineering/setup-matt-pocock-skills/SKILL.md)** â€” Scaffold the per-repo config (issue tracker, triage label vocabulary, domain doc layout) that the other engineering skills consume. Run once per repo before using `to-issues`, `to-prd`, `triage`, `diagnose`, `tdd`, `improve-codebase-architecture`, or `zoom-out`.
- **[tdd](./skills/engineering/tdd/SKILL.md)** â€” Test-driven development with a red-green-refactor loop. Builds features or fixes bugs one vertical slice at a time.
- **[to-issues](./skills/engineering/to-issues/SKILL.md)** â€” Break any plan, spec, or PRD into independently-grabbable GitHub issues using vertical slices.
- **[to-prd](./skills/engineering/to-prd/SKILL.md)** â€” Turn the current conversation context into a PRD and submit it as a GitHub issue. No interview â€” just synthesizes what you've already discussed.
- **[zoom-out](./skills/engineering/zoom-out/SKILL.md)** â€” Tell the agent to zoom out and give broader context or a higher-level perspective on an unfamiliar section of code.
- **[prototype](./skills/engineering/prototype/SKILL.md)** â€” Build a throwaway prototype to flesh out a design â€” either a runnable terminal app for state/business-logic questions, or several radically different UI variations toggleable from one route.

### Productivity

General workflow tools, not code-specific.

- **[caveman](./skills/productivity/caveman/SKILL.md)** â€” Ultra-compressed communication mode. Cuts token usage ~75% by dropping filler while keeping full technical accuracy.
- **[grill-me](./skills/productivity/grill-me/SKILL.md)** â€” Get relentlessly interviewed about a plan or design until every branch of the decision tree is resolved.
- **[handoff](./skills/productivity/handoff/SKILL.md)** â€” Compact the current conversation into a handoff document so another agent can continue the work.
- **[write-a-skill](./skills/productivity/write-a-skill/SKILL.md)** â€” Create new skills with proper structure, progressive disclosure, and bundled resources.

### Misc

Tools I keep around but rarely use.

- **[git-guardrails-claude-code](./skills/misc/git-guardrails-claude-code/SKILL.md)** â€” Set up Claude Code hooks to block dangerous git commands (push, reset --hard, clean, etc.) before they execute.
- **[migrate-to-shoehorn](./skills/misc/migrate-to-shoehorn/SKILL.md)** â€” Migrate test files from `as` type assertions to @total-typescript/shoehorn.
- **[scaffold-exercises](./skills/misc/scaffold-exercises/SKILL.md)** â€” Create exercise directory structures with sections, problems, solutions, and explainers.
- **[setup-pre-commit](./skills/misc/setup-pre-commit/SKILL.md)** â€” Set up Husky pre-commit hooks with lint-staged, Prettier, type checking, and tests.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>