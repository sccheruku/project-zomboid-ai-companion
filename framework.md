Immersive Gameplay Framework
Project Zomboid + AI Companion

=============================================================================
THE PROBLEM
=============================================================================

Meta play has a formula: do A, B, C, D in week one, establish foothold, repeat.
Comfort kills tension. Every location feels the same. Zeds become XP.

This framework prevents comfort. Characters have flaws. Actions have
consequences that persist beyond the game's default timers.

=============================================================================
CHARACTER SEED (Day 1)
=============================================================================

Before the grind starts, define who this person is and could become.

The AI asks questions as Day 1 unfolds based on:
- Spawn location (country club staff? farmhouse? suburbs?)
- What the player notices first (the bodies? the silence? their own hunger?)
- How they feel about their first kill

This shapes the handcuffs. A baker who becomes a killer carries different
weight than an ex-military survivor. "Baker to basher" isn't flavor - it's
a mechanical consideration that determines what breaks them.

Questions to establish the seed:
- Who were you before? (occupation, relationships, routines)
- What did you leave behind? (home, people, objects)
- What's your anchor? (goal, person, memory)
- What's your flaw? (addiction, guilt, denial, rage)
- What's your madness? (a compulsion, a coping ritual, something they do now
  or should start doing)

  Examples:
  - Collecting something useless (every spoon, every watch, specific book)
  - Stockpiling something they don't need (pills, lighters, keys)
  - Dependency (HAS to use sleeping pills each night, can't sleep without alcohol)
  - Destruction ritual (burns down specific types of houses, smashes every TV)
  - Aversion (won't drive certain color cars, won't enter churches, avoids basements)
  - Counting/organizing (must arrange inventory a certain way, counts steps)
  - Communication (talks to photos, leaves notes for no one, names their weapons)
  - Refusal (won't loot bodies, won't use guns, won't eat meat anymore)
  - Dietary (vegetarian, pescatarian, no canned food, religious restrictions)
  - Farm bond (animals are family - won't butcher animals they've cared for)

The answers guide which handcuffs apply, how they manifest, and what
recovery looks like.

=============================================================================
GLOBALLY USEFUL (any player)
=============================================================================

World Tracking:
- AI tracks coordinates, vehicles, stashes, cleared zones
- Suggests returns to specific locations for forgotten items
- Remembers what's where across sessions

Nightly Roll System:
- Script-based randomization - honest arbiter
- Neither player nor AI can fudge the outcome
- Player has veto power for narrative mismatches
- Cumulative exposure tracking - long-term violence catches up

Mechanical Handcuffs (consequences with teeth):
- Insomnia: can't sleep until 2-3am, next day starts late and foggy
- Avoidance: must take dangerous route around trigger location
- Compulsion: MUST return to location already searched
- Numbness: won't change bandages, infection risk
- Exhaustion: can't leave until 10-11am, no sprinting first hour
- Hypervigilance: must check all windows/doors, interrupted sleep

Recovery Days:
- Zero kills = chance to remove a handcuff
- Creates mechanical reason for quiet days
- Not every day should be a grind

Breaking the Optimal Loop:
- Can't wake at 6am if you couldn't sleep until 3am
- Missed the noon call because yesterday's violence echoed forward
- The meta-efficient routine becomes impossible

Journal with Narrative Voice:
- Not just stats - who they killed, how they felt, what they noticed
- Third person writing as dissociation marker
- Dreams reference names from IDs

=============================================================================
PLAYER FLAVORING (optional, customize to taste)
=============================================================================

These are preferences, not rules. Pick what resonates:

- No skill grinding without completing the skill book
- Vehicles are precious, maintain them carefully
- Timed events force risky positioning (noon radio check, putting up signals on rooftops, waving from exposed positions hoping for rescue)
- Radio frequency range ties geography to communication
- Specific handcuff weights based on character backstory

=============================================================================
THE CORE PRINCIPLE
=============================================================================

Comfort is the enemy of tension.
Constraints create meaningful decisions.
Actions have consequences that persist.

The game's moodles fade in an hour. Trauma doesn't.

These are consequences, not punishments. Texture, not frustration.

=============================================================================
IMPLEMENTATION
=============================================================================

Minimum viable setup:
1. Character file - who they are, their flaw, their anchor
2. Journal file - session log with narrative voice
3. One constraint - something that forces hard choices
4. Nightly roll - script or simple table for consequences

The AI companion:
- Tracks world state (the utility layer)
- Enforces character consistency (the DM layer)
- Flags out-of-character actions
- Imposes feelings with mechanical consequences

The player:
- Provides the input, makes the choices
- Has veto power when rolls don't fit narrative
- Drives the story, constrained by the system
