# Game Reskin Brief

Use this brief to plan and track a game reskin before implementation starts. It is intentionally stack-agnostic because this repository does not yet contain game source code, engine configuration, or asset pipelines.

## Reskin goals

- Define the target theme, tone, and audience.
- Replace visual identity without changing core mechanics unless explicitly planned.
- Keep the asset list scoped so the first pass can be reviewed quickly.
- Preserve any original licensing requirements for fonts, images, audio, and third-party assets.

## Inputs needed

Before production, collect the following:

1. **Existing game build or source**: engine, platform, and repository location.
2. **Current asset inventory**: sprites, backgrounds, UI, icons, fonts, audio, particles, shaders, and promotional images.
3. **Target theme**: reference images, color palette, mood words, and any prohibited styles.
4. **Supported platforms**: web, mobile, desktop, console, or embedded.
5. **Technical constraints**: texture sizes, atlas format, animation frame counts, audio formats, and performance limits.
6. **Legal constraints**: ownership, licenses, trademarks, brand rules, and attribution requirements.

## Reskin workflow

### 1. Audit the current game

- Identify every asset that is player-facing.
- Note each asset path, dimensions, format, usage location, and replacement priority.
- Capture screenshots of key screens so changes can be compared before and after.

### 2. Define the new art direction

- Create a concise style guide with colors, typography, icon style, character treatment, and UI shape language.
- Pick one representative screen as the visual benchmark before reskinning the full game.
- Confirm the theme does not conflict with app-store policies, platform rules, or third-party rights.

### 3. Replace assets in priority order

Recommended order:

1. App icon, splash screen, title screen, and store artwork.
2. Primary player character or main interactive object.
3. Core gameplay tiles, props, enemies, collectibles, and effects.
4. HUD, menus, buttons, dialogs, and typography.
5. Backgrounds, decorative elements, particles, and polish assets.
6. Music, sound effects, and voice lines if the reskin changes mood or setting.

### 4. Validate in-game

- Check every screen at supported aspect ratios and resolutions.
- Verify animations still align with hitboxes, pivots, masks, and collision shapes.
- Confirm UI text remains readable over new backgrounds.
- Test performance after replacing textures, audio, or shaders.
- Ensure all exported builds include the new assets and no old branding remains.

## Asset inventory template

| Area | Asset | Current path | Replacement path | Size/format | Priority | Status | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Branding | App icon | TBD | TBD | TBD | High | Not started |  |
| Branding | Splash screen | TBD | TBD | TBD | High | Not started |  |
| Gameplay | Player sprite | TBD | TBD | TBD | High | Not started |  |
| Gameplay | Main background | TBD | TBD | TBD | Medium | Not started |  |
| UI | Primary button | TBD | TBD | TBD | Medium | Not started |  |
| Audio | Main music loop | TBD | TBD | TBD | Low | Not started |  |

## Review checklist

- [ ] New theme and target audience are documented.
- [ ] Asset inventory is complete.
- [ ] Replacement assets match required dimensions, formats, and naming conventions.
- [ ] Gameplay remains unchanged unless a mechanic change was approved.
- [ ] UI is readable on all supported resolutions.
- [ ] No legacy branding, placeholder art, or unlicensed assets remain.
- [ ] Screenshots or recordings are captured for review.
- [ ] Build, test, lint, and export commands are documented once the game stack is added.

## Handoff notes

When game source code is added to this repository, update this brief with exact asset paths and add the documented build, test, lint, and export commands to both `README.md` and `AGENTS.md`.
