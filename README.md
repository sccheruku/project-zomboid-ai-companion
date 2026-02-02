# Project Zomboid Immersive Framework

An AI-assisted framework for immersive Project Zomboid playthroughs. Break the comfort loop. Add psychological weight to survival.

## The Problem

Meta play has a formula: do A, B, C, D in week one, establish foothold, repeat. Comfort kills tension. Every location feels the same. Zeds become XP.

This framework prevents comfort. Characters have flaws. Actions have consequences that persist beyond the game's default timers.

## How It Works

You play Project Zomboid normally, but with an AI companion (Claude or Gemini) acting as DM. The AI:

- **Tracks your world** - coordinates, vehicles, stashes, cleared zones
- **Enforces character consistency** - flags when you act out of character
- **Imposes psychological consequences** - violence has weight that accumulates
- **Writes your journal** - narrative voice that reflects who your character is becoming

## Quick Start

1. **Choose your AI** - Copy either `CLAUDE.md` or `GEMINI.md` to your project folder
2. **Start a conversation** - Tell the AI you're starting a new Project Zomboid playthrough
3. **Answer Day 1 questions** - The AI will ask about your character's backstory
4. **Play and report** - Tell the AI what happens, it tracks and responds
5. **End of day check** - The AI rolls for psychological consequences

## File Structure

```
CLAUDE.md / GEMINI.md   # AI instructions (pick one)
framework.md           # Design philosophy (optional reading)
templates/
  character.txt         # Character seed, build, rules, objectives
  journal.txt           # Session-by-session narrative log
  map.txt               # POIs, coordinates, vehicles, stashes
  handcuffs.txt         # Trauma mechanics and their triggers
```

The AI will create a folder for your character and populate these files as you play.

## Core Mechanics

### Handcuffs

Psychological constraints with gameplay consequences. Not punishments - texture.

| Handcuff | Effect |
|----------|--------|
| Insomnia | Can't sleep until 2-3am. Next day starts late. |
| Avoidance | Must avoid a location from yesterday. |
| Compulsion | Must return to a location already searched. |
| Numbness | Won't change bandages. Infection risk. |
| Exhaustion | Can't leave until 10-11am. No sprinting first hour. |
| Hypervigilance | Must check windows/doors. Interrupted sleep. |

### Nightly Roll

After each session, the AI calculates a trigger chance based on:
- Base rate (15%)
- Today's violence (kills/100, capped at 25%)
- Cumulative exposure (total kills/1000, capped at 15%)

High violence days risk triggering handcuffs. Zero-kill days can remove them.

### Character Rules

Each character has 2-4 rules that constrain gameplay:
- "No skill grinding without the book"
- "Must check radio frequencies daily"
- "Can't sleep without a locked door"
- "Weekly drink required"

These prevent optimization and create hard choices.

## Modes

**Ack Mode** (default): Brief acknowledgments during play. AI tracks, logs, stays out of the way.

**Convo Mode** (on request): Full discussion, narrative reflection, decision support.

Say "ack mode" or "convo mode" to switch.

## Recommended Mods

- **Pillow's Random Spawn** - Randomizes spawn locations. Forces you to adapt to wherever you wake up instead of optimizing around known spawns.

## Design Philosophy

Read `framework.md` for the full philosophy. The short version:

- Comfort is the enemy of tension
- Constraints create meaningful decisions
- The game's moodles fade in an hour. Trauma doesn't.
- Meta knowledge vs character knowledge - keep them separate

## Credits

Developed through actual playthroughs. Characters who shaped this framework:
- Rosita - Hermit Archivist (16 days, never reached Mama)
- Richard - Evidence Room Clerk (ongoing, escaping Louisville)

## License

Use it, modify it, share it. If you build something cool, let us know.
