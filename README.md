# Europa Universalis 5 Notes Mod

Small notes mod for Europa Universalis V.

This mod adds a new tab to the right-side panel and opens a simple notes window. Right now the project is mainly a test setup to figure out what is actually possible with the EU5 GUI, variables, and savegame systems.

## Current State

- custom button in the right panel
- custom `notes_panel`
- text input through `editor_textinput`
- early tests with `set_variable`
- early tests with `variable_map` and `global_variable_map`

## Important

At the moment, free text entered through the GUI does not persist cleanly in the savegame. Because of that, the mod is currently being used mostly to test different approaches.

Things tested so far include:

- GUI variables through `GetVariableSystem`
- `set_variable` with a dynamic country tag
- `add_to_global_variable_map`
- scope tests through `ExecuteConsoleCommand`

The main issue is not the notes window itself. The real issue is finding a way to move free text from the GUI into a data structure that the game actually saves.

## Files

- `in_game/gui/notes_panel.gui`
- `in_game/gui/panels/right_panel/right_panel.gui`
- `in_game/gui/scripted_widgets/notes_scripted_widgets.txt`
- `in_game/common/scripted_effects/note_effects.txt`

## Goal

The long-term goal is to turn this into a usable notes system for EU5. Right now the focus is still on understanding the technical limits of the script and GUI API.
