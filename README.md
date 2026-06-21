# Risen

> *"It is you. It has always been you. The Scrolls were quite specific. Also, you have been a vampire for roughly four minutes."*

**Risen** is a comedic interactive-fiction game (built in [Twine](https://twinery.org/)) — a deadpan parody of gothic vampire fiction in the vein of *World of Darkness*, told with the mundane absurdity of *What We Do in the Shadows* and the gleefully over-solemn, stilted exposition of Brennan Lee Mulligan's *Never Stop Blowing Up*.

You play an ordinary present-day person who is offered immortality at their lowest, most vulnerable moment — and accepts. What follows is not damnation. It is something much sillier: you wake up absurdly, casually omnipotent, and an ancient secret society of equally omnipotent predators immediately decides you are the prophesied one who will rule the world.

This is a stub repository capturing the concept. Nothing is built yet.

---

## Logline

A nobody is seduced into vampirism with a pitch perfectly tailored to their deepest wish — then discovers that every vampire, from night one, is a reality-bending god-being, and that a doddering, self-important immortal aristocracy is utterly convinced *you* are the Chosen One destined to rule all of creation. You did not ask for this. The prophecy is very insistent.

## The Concept

### Chapter One — The Pitch

The game opens by letting the player choose an **archetypal wish-fulfillment background** — a familiar fantasy of who they are and what they lack. Each background is a wound, and the vampire who finds you knows exactly which one to press. The offer of immortality is never generic; it is the single most persuasive thing this specific person could possibly hear in this specific moment:

- **The Heartbroken Sad-Sack** — lonely, grieving, unloved — is promised eternal, unconditional, never-fading love.
- **The Bullied Outcast** — invisible, powerless, humiliated — is offered the power to be feared, adored, and unignorable.
- **The Terminally Ill** — out of time — is offered, simply, *never dying*.
- *(and more archetypes — the ambitious failure, the burned-out caretaker, the forgotten genius, etc.)*

The seduction is the heart of Chapter One: warm, intimate, flattering, and deeply manipulative. The player says yes. They always say yes — the question is only *why*.

### The Turn — Wait, This Is Ridiculous

Then they wake up.

The central comedic engine of **Risen** is the gap between **cosmic, effortless power** and **petty, out-of-touch banality**. Every vampire — the newest fledgling and the ten-thousand-year-old elder alike — is, from the very first night, *grotesquely* overpowered:

- mind control over any human, instantly, with no effort
- flight, teleportation, and transformation into bats, wolves, mist, whatever
- telepathy, hypnosis, and the kind of casual god-magic that should obviously let one person conquer the planet by Tuesday

And it is *immediately, blindingly obvious to the player* that they could, in fact, just take over the world. It would not even be hard. No one seems to have noticed this. They've had eternity to notice and they have simply... not.

### The Society — A Parody of Itself

The vampires are organized into an impossibly ancient, rigidly hierarchical secret society that has become a parody of itself: hopelessly out of touch, obsessed with arcane etiquette and millennia-old grudges, convinced of its own profound seriousness while being deeply, profoundly silly. These are beings who could rewrite reality, bickering about seating arrangements and whose turn it is to host the Conclave.

### The Prophecy — "Risen"

There is a long tradition among them of a foretold **vampire messiah** — a *Risen One* who will at last unite the clans and rule the world as was Written. And for reasons that are never quite convincing, *everyone instantly believes it is you.* Elder predators who have terrified continents fall over themselves to defer to a confused person who got turned on a Tuesday and still has a job. The prophecy is cited constantly, in increasingly stilted and grandiose terms, to explain things it very clearly does not explain.

The title carries the double meaning on purpose: **risen** as a vampire rises from death, and **risen** as in *He Is Risen* — the awaited savior. The joke is that the awaited savior is bewildered, ordinary, and never asked to be either.

## Tone & Influences

- **What We Do in the Shadows** — supernatural power rendered mundane, petty, and roommate-grade; ancient beings who are exhausting to be around.
- **World of Darkness / *Vampire: The Masquerade*** — the source being parodied: solemn gothic hierarchy, clans, elaborate lore, capital-letter Nouns. *Risen* plays it straight-faced and then lets the air out.
- **Brennan Lee Mulligan, *Never Stop Blowing Up*** — exposition delivered with intentionally stilted, over-pompous grandeur, where the *delivery* is the joke. The prophecy and the elders should narrate themselves like this.
- **Self-insert / "Chosen One" power-fantasy fanfiction** — knowingly leaned into. Everyone believing the player is special, instantly and without earning it, is the bit. The wish-fulfillment is the satire.

The register to hold throughout: **deadpan**. Cosmic stakes and absurd reverence, played with a completely straight face. The player is the only one who finds any of this strange.

## Format

- A branching **Twine** game (Twee source; Harlowe or SugarCube TBD).
- Authored with the [OpenStorySLOP](https://github.com/mackenzieclark/openstoryslop) toolkit (`/oss:*` workflow), exported to Twee/Twine.
- Choice-driven, replayable across the different opening archetypes — each wish-fulfillment background recolors the whole story.

## Status

🩸 **Stub / concept.** This repo currently holds the pitch and a placeholder story scaffold. Open design questions:

- The exact mechanism by which the prophecy "selects" the player — and how to keep it bewildering rather than explained.
- How (and whether) the player can lean into vs. resist the Chosen One role.
- Which archetypal backgrounds make the final cut, and how divergent their playthroughs are.
- Whether "ruling the world is trivially easy" becomes an actual gameplay axis or remains a running joke.

## Repository Layout

```
risen/
├── README.md          # this file — the concept
├── docs/
│   └── design-notes.md # open questions, archetype list, tone bible (WIP)
└── story/
    └── risen.twee      # placeholder Twee source for the Twine game
```

## License

TBD.
