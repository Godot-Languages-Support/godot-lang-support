# 🗺 Godot Languages Support

*A community-maintained listing of languages with bindings for making scripts in Godot Engine.*

### ⚠ Disclaimer

Core engine or module development is preferably done using C++ (which is the language in which the engine is written), for which [the official docs for contributing to the engine](https://docs.godotengine.org/en/stable/community/contributing/index.html) is a better starting point.
The languages provided here can be used for *making scripts through the GDNative interface*, which also includes C++, but support for which is different from its use in module development.


## Categories

### By editor support
- 🧬 Godot Engine Integrated Editors (usually possible via PluginScript)
- 🔌 External IDE or Editor (NativeScript default)

### By maintainer
- 💍 Official
- 👥 Community-maintained


## 🏆 Full support
1. **[GDScript](https://docs.godotengine.org/en/stable/getting_started/scripting/gdscript/index.html) 💍🧬🔌**
1. **[VisualScript](https://docs.godotengine.org/en/stable/getting_started/scripting/visual_script/index.html) 💍🧬**

  GDScript is actively maintained and documented, and is stable. It is the primary language, has the most tutorials online and has deep in-Godot editor support.

  VisualScript can be considered as a secondary scripting language with blocks-and-nodes. It too provides rich support, although there is a community effort to make it more intuitive to use as a design tool instead of what users describe as a one-to-one mapping of code with terse programming jargon where it should be more humanised.

## 🥇 Production Ready
1. **[Rust](https://github.com/godot-rust/godot-rust) 👥🔌**
1. **[Nim](https://github.com/pragmagic/godot-nim) 👥🔌**
1. **[JavaScript](https://github.com/GodotExplorer/ECMAScript) 👥🔌**
1. **[C#](https://docs.godotengine.org/en/stable/getting_started/scripting/c_sharp/index.html) 💍🔌**
1. **[Lua](https://github.com/perbone/luascript) 👥🧬🔌**

  These languages are documented and stable. Some people use it in production.

  JavaScript support is a 3rd-party module. Modules add built-in support (like GDScript), but require [compiling it into the engine](https://docs.godotengine.org/en/stable/development/cpp/custom_modules_in_cpp.html).
  With JavaScript, you also get support for languages that transpile to JavaScript, e.g. TypeScript or CoffeeScript.

  C# support is an official module. If you have a Mono-version of Godot Engine, it comes built into the engine.
  With C#, you also get support for integrating other Mono-supported languages, e.g. F# or VisualBasic. But, Godot currently hardcodes C# usage. Any classes attached to a Node or Resource must be a C# script.
  For tools to facilitate the use of F# with Godot's C# scripts, see [Godot F# Tools](https://github.com/willnationsdev/godot-fsharp-tools).

  (C# External Code Editing support is decent. What's it like for the others?)

## 🥈 Nearly There
1. **[D](https://github.com/godot-d/godot-d) 👥🔌**
2. **[Haskell](https://hackage.haskell.org/package/godot-haskell) 👥🔌**

  Stable, not documented.

## 🥉 Has Potential
1. **[Python](https://github.com/touilleMan/godot-python) 👥🧬🔌**  
1. **[Kotlin](https://github.com/utopia-rise/godot-kotlin) 👥🔌**

  Python is the only language integrated via PluginScript. It provides editor integration as GDScript does - it's still in beta.

  Kotlin bindings, while declared unready for production use and still in alpha, are being maintained fairly regularly in 2020.

## 🏅 Okay, I guess?
1. **[C++ *GDNative support*](https://github.com/godotengine/godot-cpp) 💍🔌**

  C++ is a bit of a hot potato anywhere, and it is here as well: some people like to use it, but it could use better documention in places. Some peeves such as not being able to use modern C++ features starting from C++11 dwell in this API.

## Left 4 Dead
1. **[Go](https://github.com/ShadowApex/godot-go) 👥🔌**
1. **[Ruby](https://github.com/onyxblade/godot-ruby) 👥🧬🔌**
  
  Go bindings haven't been updated since 2018.
  Sadly, not documented and stable enough for production.
  
  Ruby bindings haven't been updated since 2018.
  It's an attempted PluginScript system, but it's designed poorly with ~15x performance loss vs. GDScript.
  Not documented or stable enough for use.

## Other Useful links

- Gamesfromscratch made a [video](https://youtu.be/VqcMlS-IJl4) about some of the supported languages.
- (You can expand this list!)

## Enjoy ^-^
