# Blender Differential Growth (fork) — notes for Claude

Read this first.

## Owner and rules
- New to coding and wants to learn. Explain in plain words and give time estimates.
- Be concise. Show only the lines you changed.
- Plan work in phases and get the plan approved before building.
- **Never push, merge or publish without explicit OK.** Use a branch and a pull request. This repo is public.
- Show a preview (renders or screenshots) for visual changes before building them.
- Take the least-token path, but never at the expense of quality.
- Say when a chat is getting long, and offer a handoff summary.
- Write a learning guide only when the owner asks.

## What it is
The owner's fork of inca/blender-differential-growth, a Blender add-on that grows lichen-, algae- and coral-like meshes. Forked to improve it in Blender. It's also the reference look for the browser `differential-growth-sim`.

## Files
| File | What's in it |
|---|---|
| `__init__.py` | Add-on registration and info |
| `op_grow.py` | The growth operator: repulsion + noise, edge splitting, inner-growth die-off |
| `settings.py` | Growth settings, whose names and defaults the browser sim may copy |
| `panel.py` | Blender UI panel |
| `symlink.sh` | Links the repo into Blender's add-ons folder for development |

## Rules of the project
- Growth changes the mesh in place, and some settings can explode the mesh and hang Blender. Warn the owner to save first.
- Keep the original credits and the Blender (GPL) license.
- Testing needs Blender on the owner's computer. Say what to check, and how, after each change.

## Current state
Forked and unchanged so far. Improvements aren't planned yet.
