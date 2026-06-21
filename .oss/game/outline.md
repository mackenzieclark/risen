---
name: outline
type: game-outline
description: Branching outline for Risen (Twine/Harlowe)
format: twine
status: draft
---

# Risen — Game Outline (Twine/Harlowe)

**POV / tense:** second person, present.
**Structure:** a branching Chapter One (archetype seductions) that converges on the Bite, then a mostly-linear escalation through the Turn and the Anointing, with a persistent choice axis (how you regard your "destiny") that recolors reactions rather than forking the whole tree.

Legend: `[PASSAGE]` = Twine passage. `→` = link/choice. ⟡ = convergence point.

---

## ACT 0 — THE PITCH *(Chapter One: the tailored seduction)*

`[Start]` — Worst night of the player's life. The Sire sits down. "I'm going to make you an offer, and I think you're going to say yes."
→ `[Backgrounds]`

`[Backgrounds]` — Player chooses an **archetypal wish-fulfillment background**. This sets the `archetype` variable and routes to a tailored pitch. Each pitch is intimate, specific, and genuinely persuasive — the satire is sharper when the manipulation lands.

| Choice | Wound | Tailored Offer | Passage |
|---|---|---|---|
| The Heartbroken Sad-Sack | lonely, grieving, unloved | eternal, unconditional, never-fading love | `[Pitch: Love]` |
| The Bullied Outcast | invisible, powerless, humiliated | to be feared, adored, unignorable | `[Pitch: Power]` |
| The Terminally Ill | out of time | simply never dying | `[Pitch: Forever]` |
| *(stretch)* The Ambitious Failure | overlooked, broke, talented | limitless time and power to finally "make it" | `[Pitch: Glory]` |
| *(stretch)* The Burned-Out Caretaker | drained, taken for granted | strength without end; never the weak one again | `[Pitch: Strength]` |

Each `[Pitch: *]` passage: the Sire presses the wound, makes the offer, gives the player a beat of hesitation, then:
→ `[The Bite]` (all branches converge ⟡)

**Design note:** record the archetype; it should echo later as a thematic thread (e.g. the love-promised player keeps being offered hollow versions of love; the power-promised player keeps being handed power they didn't want *this* badly).

`[The Bite]` ⟡ — Player accepts. "You say yes. You always say yes. The only question was ever *why*." End of Chapter One.
→ `[Waking]`

---

## ACT 1 — THE TURN *(wait, this is ridiculous)*

`[Waking]` — Player wakes up changed. First, the comedy of the new senses/body, played mundane.
→ `[First Powers]`

`[First Powers]` — Low-stakes discovery of absurd, casual omnipotence. Accidentally compels a barista. Drifts off the ground. Hears a stranger's thoughts and wishes they hadn't. The tone: this is *easy*, and no one warned you it would be this easy.
→ `[The Realization]`

`[The Realization]` — The load-bearing beat. The player clocks it: *with this, I could run the entire world. Trivially. Why hasn't anyone?* The narration lets the thought sit. (Theme 2.) 
→ `[Summoned]`

`[Summoned]` — First contact with the society: the Sire (anxious) explains the player is wanted. The ancient world intrudes on the modern one (a summons delivered by bat, or a centuries-old courier baffled by a doorbell).
→ `[The Conclave]`

---

## ACT 2 — THE ANOINTING *(everyone is certain it's you)*

`[The Conclave]` — The player is brought before the out-of-touch immortal society. Establish the gravitas, the etiquette, the petty grudges (Lord Aurelius Vane mid-feud). Pure deadpan grandeur.
→ `[The Declaration]`

`[The Declaration]` — **Brother Pelagius** takes one look and declares the player the prophesied **Risen One**. Instant, unanimous, tearful belief. The "evidence" from the Scrolls explains nothing. Marguerite raises an obvious objection and is serenely ignored.
→ `[How You Take It]`

`[How You Take It]` — **Introduces the persistent destiny axis** (`stance` variable). The player chooses how to regard the absurd anointing. This colors NPC reactions and dialogue from here on rather than forking the whole story:
- → **Play along** (`stance: believer/opportunist`) — let them believe it; see where it goes.
- → **Protest** (`stance: skeptic`) — insist there's been a mistake; no one accepts this, which is funnier.
- → **Test it** (`stance: pragmatist`) — give an absurd "command" to see if they'll actually obey. They will, instantly and completely. This is alarming.

All three →  `[The Easy Throne]`

`[The Easy Throne]` — Escalation beat: it becomes clear the society will hand the player the world if asked, and that ruling it would be *effortless and boring*. The horror-comedy of getting everything, unearned, instantly. Set the central tension for Chapter Two: **what do you do when omnipotence and a throne are simply handed to a bewildered nobody?**
→ `[End of Chapter One — To Be Continued]`

`[End of Chapter One — To Be Continued]` — Button on the opening arc; tease the politics, the rival claimants, the question of whether the player wants any of this.

---

## Candidate Variables (for `/oss:gamify design`)
- `archetype` — the Chapter One background (love / power / forever / glory / strength). Echoes thematically throughout.
- `stance` — regard for the destiny (believer / skeptic / opportunist / pragmatist). Colors NPC reactions.
- `sire_bond` — trust / resentment / dependence toward the Sire.
- `doubt` *(hidden counter)* — how much the player has poked holes in the Prophecy; could unlock Marguerite as an ally.

## Open Structural Questions
- How divergent should the archetype branches be after the Bite — pure flavor reskin, or genuinely different beats?
- Is "world domination is trivially easy" a real mechanic later, or a sustained gag?
- Does `stance` ever converge into distinct endings, or remain tonal coloring through Chapter Two?
- Engine: Harlowe is fine for this branch-and-flag scope; revisit SugarCube only if `doubt`/relationship stats grow into real systems.
