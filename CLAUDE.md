# Masks: Adversaries Pack

Content pack containing villain NPCs from the Masks: Adversaries supplement.

## Overview

- **Module ID:** `masks-adversaries`
- **Type:** Content pack (Actor compendium)
- **Dependency:** Requires `masks-newgeneration-unofficial`
- **Content:** 77 villain NPCs

## Structure

```
masks-adversaries/
├── module.json             # Module manifest
├── packs/adversaries/      # LevelDB compendium (gitignored)
├── src/packs/adversaries/  # JSON source files (version controlled)
├── images/adversaries/     # NPC portraits
├── tools/                  # Pack conversion scripts
└── package.json
```

## Commands

```bash
npm install              # Install dependencies
npm run pullJSONtoLDB    # JSON → LevelDB (after git pull)
npm run pushLDBtoJSON    # LevelDB → JSON (for version control)
```

**Important:** Foundry must be closed when running pack conversion.

## Image Paths

Images are referenced as: `modules/masks-adversaries/images/adversaries/{filename}`

## Editing Content

1. Make changes in Foundry
2. Close Foundry (or go to welcome screen)
3. Run `npm run pushLDBtoJSON`
4. Commit the JSON changes

## JSON File Naming

Files follow the pattern: `{type}_{SafeName}_{id}.json`
- Example: `npc_Legion_15jFlciZjBHryVs7.json`
