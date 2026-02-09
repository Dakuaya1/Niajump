

Executive Summary

"Lean Before You Leap" is a consolidated framework for a mobile-first, endless vertical platformer. The project's core design philosophy shifts player agency away from traditional action inputs (jumping) and toward physical commitment under uncertainty. By utilizing a tilt-only control scheme and an automatic jumping mechanic, the game forces players to manage horizontal momentum and anticipate fixed jump intervals.

The experience is built upon three integrated pillars: Perfect Timing (reward system), Momentum (skill expression), and Risk Platforms (decision layer). Success is not determined by reflexes, but by the player’s ability to rhythmically commit to a direction before the mechanical jump occurs. The document outlines a "build-ready" design that explicitly forbids feature bloat—such as power-ups, currencies, or tutorials—favoring a pure, mechanics-driven depth where difficulty scales invisibly through tightened tolerances.


--------------------------------------------------------------------------------


1. Core Identity and Gameplay Philosophy

The project is defined by a minimalist approach to mobile platforming, removing standard button inputs to focus on the physical sensation of balancing and leaning.

* Genre: Endless vertical platformer.
* Control Scheme: Phone tilt only (left/right). There are no buttons and no manual jump inputs.
* Input Philosophy: Tilt controls horizontal acceleration rather than direct position. This prevents jitter, encourages early commitment, and makes over-correction costly.
* The Central Tension: The game requires the player to commit physically (leaning the device) before the game commits mechanically (triggering the jump).

The Authoritative Core Loop

The gameplay follows a perpetual cycle that tightens as the session progresses:

1. Balance: Stabilize after landing.
2. Anticipate: Await the silent approach of the jump timer.
3. Commit Lean: Move the device to set direction.
4. Auto Jump: The system triggers a jump at a fixed interval with constant force.
5. Momentum Carry: Horizontal speed persists mid-air.
6. Decision/Outcome: The player lands, survives a "drama moment," or falls.
7. Camera Pressure: The upward-moving camera advances, forcing the next loop.


--------------------------------------------------------------------------------


2. The Three Pillars of Integration

The framework operates through three systems that interact during every jump cycle.

I. Perfect Timing (Reward System)

The primary "dopamine source" for the player is the Perfect Landing. This occurs when a player lands within a narrow timing window with controlled horizontal momentum.

* Rewards: Subtle affirmations such as a brief camera slowdown, a slightly longer hang-time on the subsequent jump, or soft audio-visual cues.
* Systemic Constraint: The game explicitly avoids score multipliers, UI pop-ups, or currencies to reward skill.

II. Momentum (Skill Expression)

Momentum is the primary method for players to express mastery without character upgrades.

* Persistence: Momentum is never reset and carries across platforms.
* Impact: It determines the width of the jump arc and the difficulty of mid-air corrections.
* Skill Curve: Beginners play safely (slowly), while experts "surf" or "ride" high momentum through risky sections.

III. Risk Platforms (Decision Layer)

The game presents a constant choice between safety and voluntary stress.

* Safe Platforms: Wide and forgiving; they maintain neutral camera pressure.
* Risk Platforms: Narrow or offset; landing on these temporarily reduces camera pressure, providing "breathing room."
* Strategic Choice: Players must decide whether to play it safe and risk being squeezed by the camera, or take a risk to relieve that pressure.


--------------------------------------------------------------------------------


3. Environmental Mechanics and Difficulty Scaling

The Camera as Invisible Enemy

The camera acts as the primary antagonist. It moves upward at a speed that increases over time and never reacts to player mistakes. Hesitation is punished by the camera "consuming" the player, while perfect timing and risk-taking provide "mercy" or "relief" from its advance.

Systemic Difficulty Scaling

Difficulty increases elegantly without introducing new mechanics or tutorials. Scaling is achieved by:

* Shortening jump intervals.
* Increasing momentum carry-over.
* Reducing the "perfect timing" window.
* Increasing the frequency of risk platforms.
* Reducing recovery tolerance.


--------------------------------------------------------------------------------


4. Session Design and User Experience

Session Flow

Designed for short-burst, "flow-state" play, the game features a streamlined session structure:

* Average Run: 30 to 90 seconds.
* Restart Flow: Single tap anywhere to restart; no menus or delays (target restart time: < 1 second).
* Failure Conditions: Run ends immediately upon falling below the camera, missing a platform, or losing control from excess momentum.

Recovery and "Drama Moments"

To prevent failure from feeling binary and to increase engagement, the design includes "drama moments" where a player should have failed but barely survived:

* Tiny wall brushes.
* Micro slides.
* One-frame edge/catch saves.

Visual and Audio Framework

Element	Philosophy	Specifications
Visuals	Minimalist/High Contrast	Clear silhouettes; player is the brightest object; no distracting parallax initially.
Audio	Rhythmic Intuition	Subtle rhythmic cue before auto-jumps; soft confirmation for perfect timing; sharp/short failure sound.


--------------------------------------------------------------------------------


5. Development Scope and Guardrails

The framework includes strict "Scope Guardrails" to protect the core design from feature creep. The document defines the game by what it is not as much as what it is.

Explicitly Forbidden Features:

* Power-ups or collectibles.
* Progression trees or stat systems.
* Skins as rewards or any form of currency.
* Multiplayer or narrative elements.
* Tutorials (the game must be learnable through play).

Build Order Priority

1. Core auto-jump loop.
2. Tilt-based momentum.
3. Camera pressure mechanics.
4. Platform generation and risk platform logic.
5. Perfect timing detection.
6. Recovery moments.
7. Final polish and tuning.


--------------------------------------------------------------------------------


6. Key Philosophical Takeaways

The documentation concludes with a definitive statement on the game's intent:

* Not about: Precision input, jumping, or reflexes.
* About: "Commitment under uncertainty."
* The Player's Question: The player does not ask "Can I make this jump?" but rather "Am I already too late?"
