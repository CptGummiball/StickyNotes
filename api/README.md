# Sticky Notes API for mod developers

API version **1** · package `dev.cptgummiball.stickynotes.api` · mod id `stickynotes`

**Most mods need nothing from this page** if Sticky Notes uses the standard loader interfaces.

## Getting the API

`stickynotes-api-1.jar` and `stickynotes-api-1-javadoc.jar` from the [releases](../../../releases),
as a **compile-only** dependency. Do not ship the API or any Sticky Notes files in your mod. If
Sticky Notes is optional for your mod, check that the mod `stickynotes` is loaded before touching its
classes.

The license (section 5) allows compiling against the API and publishing mods that use it.
