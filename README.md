# 🗺 Godot Languages Support

*A community-maintained list of languages with bindings for making scripts in Godot Engine.*

### ⚠ Disclaimer

Engine and module development use C++. For those topics, please start with the official docs for [contributing to the engine](https://docs.godotengine.org/en/stable/community/contributing/index.html) and [understanding engine development](https://docs.godotengine.org/en/stable/development/cpp/index.html).

In contrast, the languages provided here are for *making scripts* in Godot projects. Godot has many methods for granting language support:

- **Modules:** Maintainers/Developers define custom implementations of Godot's `Script`, `ScriptInstance`, and `ScriptLanguage` types in a module. Users add the module to the engine source code and compile the engine themselves (or a developer may provide precompiled binaries). Now you have a new built-in language.
- **PluginScript:** Maintainers/Developers write an EditorPlugin addon which teaches the Editor how to understand the target language as a `ScriptLanguage`. Users should only need to download the addon. Powered by Godot's *GDNative C interface* module.
- **NativeScript:** Maintainers write tools to generate and build "bindings" in the target language. Developers use the tools to create bindings, write scripts, and compile them into a native library for an addon. Users download the addon and use the native scripts in their projects. To write custom functionality, most people are both Developers and Users. Powered by Godot's *GDNative C interface* module.
    - Note: The Developer role's complexity is dependent on the quality of the Maintainer's tools. As such, it is language-dependent. Usually, they are difficult. Your mileage may vary.

## Categories

### By editor support
- 🧬 Can be edited inside Godot Engine (includes language bindings which use `PluginScript` and the `Script API`).
- 🔌 Can be edited in an External Editor (includes languages bindings which use `NativeScript`).

### By maintainer
- 💍 Official
- 👥 Community-maintained

### By method
- ⚙️ Module
- 📜 PluginScript
- 🔧 NativeScript
- 🏄 "Surfs" on an existing language's functionality to work with Godot.

## 🏆 Full support
1. ### [GDScript](https://docs.godotengine.org/en/stable/getting_started/scripting/gdscript/index.html) 💍🧬🔌⚙️
    GDScript is actively maintained and documented and is stable. It is the primary language, has the most tutorials online, and has deep in-Godot editor support.

1. ### [VisualScript](https://docs.godotengine.org/en/stable/getting_started/scripting/visual_script/index.html) 💍🧬⚙️
    VisualScript can be considered as a secondary scripting language with blocks-and-nodes. It too provides rich support, although there is a community effort to make it more intuitive to use as a design tool instead of what users describe as a one-to-one mapping of code with terse programming jargon where it should be more humanized.

## 🥇 Production Ready
  These languages are documented and stable. Some people use it in production.

1. ### [Rust](https://github.com/godot-rust/godot-rust) 👥🔌🔧

1. ### [Nim](https://github.com/pragmagic/godot-nim) 👥🔌🔧
    Nim has standard NativeScript features for the moment, but wishes to go beyond that by [improving its user experience](https://github.com/pragmagic/godot-nim/issues/66) to automate repetitive boilerplate tasks.

1. ### [JavaScript](https://github.com/GodotExplorer/ECMAScript) 👥🔌⚙️
    JavaScript support is a 3rd-party module. Modules add built-in support (like GDScript) but require [compiling it into the engine](https://docs.godotengine.org/en/stable/development/cpp/custom_modules_in_cpp.html).
    With JavaScript, you also get support for languages that transpile to JavaScript, e.g. TypeScript or CoffeeScript.

1. ### [C#](https://docs.godotengine.org/en/stable/getting_started/scripting/c_sharp/index.html) 💍🔌⚙️
    C# support is an official module. If you have a Mono-version of Godot Engine, it comes built into the engine.
  With C#, you also get support for integrating other Mono-supported languages, e.g. F# or VisualBasic. But, Godot currently hardcodes C# usage. Any classes attached to a Node or Resource must be a C# script.
  For tools to facilitate the use of F# with Godot's C# scripts, see [Godot F# Tools](https://github.com/willnationsdev/godot-fsharp-tools).

  (C# External Code Editing support is decent. What's it like for the others?)

## 🥈 Nearly There
  Stable, not documented.
1. ### [D](https://github.com/godot-d/godot-d) 👥🔌🔧
1. ### [Haskell](https://hackage.haskell.org/package/godot-haskell) 👥🔌🔧
1. ### [Lua](https://github.com/perbone/luascript) 👥🧬🔌🔧
    Lua is currently undergoing a rewrite of its parser. 

## 🥉 Has Potential
1. ### [Python](https://github.com/touilleMan/godot-python) 👥🧬🔌📜
    Python is the language for which PluginScript, the API that provides Godot-editor support, got designed for. It provides editor integration as GDScript does - it's still in beta. Currently, the bottleneck to its stability is its flawed [export system](https://github.com/touilleMan/godot-python/issues/146).

1. ### [Kotlin](https://github.com/utopia-rise/godot-kotlin) 👥🔌🔧
    Kotlin bindings, while declared unready for production use and still in alpha, are being maintained fairly regularly in 2020.
1. ### [Go (godot-go)](https://github.com/godot-go/godot-go/) 👥🔌🔧
    Go bindings from godot-go are a recent project in alpha. There is decent documentation of the build workflow and example scripts. It is actively being developed.

## 🏅 Okay, I guess?
1. ### [C++ *GDNative support*](https://github.com/godotengine/godot-cpp) 💍🔌🔧
    C++ is a bit of a hot potato anywhere, and it is here as well: some people like to use it, but it could use better documentation in places. Some peeves such as not being able to use modern C++ features starting from C++11 dwell in this API.

## 🐣 Up and coming
1. ### [Ada](https://github.com/MichaelAllenHardeman/gdnative_ada) 👥🔌🔧
    Ada was type-safe before Rust was even born.
    This isn't documented or (probably) stable, but it is still very new.

1. ### [Dart](https://github.com/mahdisml/DartGodot) 👥🔌🏄
    Uses Godot's C# API to make calls to Dart script code. Has code for generating scripts.

## Left 4 Dead
1. ### [Go (ShadowApex)](https://github.com/ShadowApex/godot-go) 👥🔌🔧
    Go bindings from ShadowApex haven't been updated since 2018. Not documented or stable enough for production.

1. ### [Ruby](https://github.com/onyxblade/godot-ruby) 👥🔌🔧 
    Ruby bindings haven't been updated since 2018.
    It's an attempted PluginScript system, but it's designed poorly with ~15x performance loss vs. GDScript.
    Not documented or stable enough for use.

1. ### [Haxe](https://github.com/mrcdk/godot-haxe) 👥🔌🔧

1. ### [AngelScript](https://github.com/Geequlim/AngelScript)👥🔌🔧
    AngelScript was @Geequlim's first forray into GDNative, before making the ECMAScript bindings.

1. ### [Zig](https://github.com/outrera/godot-zig)👥🔌🔧

1. ### [Object Pascal](https://github.com/BenediktMagnus/godot-object-pascal)👥🔌🔧

## Other Useful links

- Gamesfromscratch made a [video](https://youtu.be/VqcMlS-IJl4) about some of the supported languages.
- (You can expand this list!)

## Enjoy ^-^
