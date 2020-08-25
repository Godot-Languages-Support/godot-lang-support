# 🗺 Godot Languages Support
> Originally forked from https://gist.github.com/ShalokShalom/7b2308e6ddc020d7ab7080b645953f1b

*A community-maintained listing of languages with bindings for making scripts in Godot Engine.*

### ⚠ Disclaimer
Core engine or module development is preferably done using C++ (which is the language in which the engine is written), for which [the official docs for contributing to the engine](https://docs.godotengine.org/en/stable/community/contributing/index.html) is a better starting point.

The languages provided here can be used for *making scripts through the GDNative interface*, which also includes C++, but support for which is different from its use in module development.

## Categories

### (TODO)
(Per-module support feature legend. Currently, Rust (IIRC) doesn't support the video encoding module.)


### By feature
- 🧬 Integrated with Godot Engine
- 🔌Needs External IDE

### By maintainer
- 💍 Official
- 👥 Community-maintained


## 🏆 Full support
1. **[GDScript](https://docs.godotengine.org/en/stable/getting_started/scripting/gdscript/index.html) 💍🧬**
1. **[VisualScript](https://docs.godotengine.org/en/stable/getting_started/scripting/visual_script/index.html) 💍🧬**

  GDScript is actively maintained and documented, and is stable. It is the primary language, has the most tutorials online and has deep in-Godot editor support.

  VisualScript can be considered as a secondary scripting language with blocks-and-nodes. It too provides rich support, although there is a community effort to make it more intuitive to use as a design tool instead of what users describe as a one-to-one mapping of code with terse programming jargon where it should be more humanised.

## 🥇 Production Ready
1. **[Rust](https://github.com/godot-rust/godot-rust) 👥🔌**
1. **[Nim](https://github.com/pragmagic/godot-nim) 👥🔌**
1. **[JavaScript](https://github.com/GodotExplorer/ECMAScript) 👥🔌**
1. **[C#](https://docs.godotengine.org/en/stable/getting_started/scripting/c_sharp/index.html) 💍🔌**


  These languages are documented and stable. Some people use it in production.

  (C# External Code Editing support is decent. What's it like for the others?)

## 🥈 Nearly There
1. **[D](https://github.com/godot-d/godot-d) 👥**

  Stable, not documented.

## 🥉 Has Potential
1. **[Python](https://github.com/touilleMan/godot-python) 👥🧬**  
1. **[Kotlin](https://github.com/utopia-rise/godot-kotlin) 👥🔌**

  Python is the only language integrated via PluginScript. It provides editor integration as GDScript does - it's still in beta.

  Kotlin bindings, while declared unready for production use and still in alpha, are being maintained fairly regularly in 2020.

## 🏅 Okay, I guess?
1. **[C++ *GDNative support*](https://github.com/godotengine/godot-cpp) 💍🔌**

  C++ is a bit of a hot potato anywhere, and it is here as well: some people like to use it, but it could use better documention in places. Some peeves such as not being able to use modern C++ features starting from C++11 dwell in this API.

## Left 4 Dead
1. **[Haskell](https://hackage.haskell.org/package/godot-haskell) 👥🔌**
1. **[Go](https://github.com/ShadowApex/godot-go) 👥🔌**

  Haskell is used by one project only and is only partly integrated and documented.
  
  Go bindings haven't been updated since 2018.

  Sadly, not documented and stable enough for production.
  If you can, please revive them.
