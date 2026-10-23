# Melee Code Collection

Gecko codes for **Super Smash Bros. Melee (NTSC 1.02)**, built to work with
**Slippi Dolphin**, including rollback netplay over direct connect.

Each code is a plain `.txt` file in the [`codes`](codes) folder that you can
paste into Dolphin's Gecko Codes tab.
There's one code so far, and more will follow.

## Codes

| Code | File | What it does | Status |
|---|---|---|---|
| Turbo Mode | [`codes/TurboMode.txt`](codes/TurboMode.txt) | Land a hit, then cancel your move into a different one | Beta |

---

## Turbo Mode

A recreation of **Turbo Melee** from *The Akaneia Build*, for vanilla Melee.
Akaneia's version doesn't work on Slippi. This one is written to stay in sync
over rollback.

### How it plays

- **Land a hit to get turbo.** Your fighter blinks pink for up to half a
  second (30 frames).
- **While you're pink, cancel your current move into a different one.** On
  the ground that's attacks, specials, grab, jump, dash, roll, spot dodge or
  taunt. In the air it's aerials, specials, jump, Z-air or item throws.
- **You can't cancel into the move that landed the hit.** All jabs count as
  one move.
- **You can cancel during hitlag.** Cancelling ends the freeze right away.
- **No shield or air dodge cancels.**
- Holding the stick back after a grounded hit turns you around, and that uses
  up turbo.
- Hits on fighters count, including your projectiles and throws. Hits on
  shields don't.
- Getting hit, or using turbo, ends it. Landing a new hit gives you a fresh
  30 frames, so you can chain cancels.
- Each cancel plays a small effect and a sound.

The rules are based on how Akaneia's code actually behaves, not just its
description. That includes some of its odd edge cases.

---

## Requirements

- **Super Smash Bros. Melee, NTSC 1.02** (game ID `GALE01`, revision 2). Other
  versions and other mods aren't supported.
- **[Slippi Dolphin](https://slippi.gg)**, or a recent Dolphin build that
  supports Gecko codes.

## Installing a code

1. Open the code's `.txt` file and copy everything in it, including the first
   line that starts with `$`.
2. In Dolphin, right-click Melee in the game list and choose **Properties**.
3. Open the **Gecko Codes** tab, click **Add New Code**, and paste the code.
4. Make sure the new code is ticked, then close the window.
5. Start the game.

If you use Slippi, do this in the Dolphin used for netplay. You can open its
settings from the Slippi Launcher.

## Playing online

- **Both players need the same code enabled.** If only one player has it, or
  the versions differ, the game will desync.
- Use it in **direct connect** with a friend. Don't use it in matchmaking.
- If you have several codes enabled, keep the same set on both sides.

## Reporting problems

These codes are still being tested. If something breaks, please
[open an issue](https://github.com/LiamTrader43/Melee-Code-Collection/issues).
Include:
- which code you used;
- the characters, moves and stage involved;
- whether it was offline or online.

---

## Credits

Made by **LiamTrader**.

**Special thanks to Kneemaster12.**

Thanks also to:
- **Team Akaneia**, who created Turbo Melee for *The Akaneia Build*. This
  collection isn't affiliated with Team Akaneia. It includes none of their
  files or code; the codes were written separately for vanilla Melee.
- **Project Slippi**, for Slippi and rollback netplay.
- The **Melee decompilation project** (doldecomp/melee) and **m-ex**, for
  their documentation of the game's code.
