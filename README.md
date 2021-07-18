# 🗺 Godot Languages Support

*A community-maintained list of Language Support Projects for Godot Engine.*

### ⚠ Disclaimer

The engine and modules are developed in C++. For those topics, please start with the official docs for [contributing to the engine](https://docs.godotengine.org/en/stable/community/contributing/index.html) and [understanding engine development](https://docs.godotengine.org/en/stable/development/cpp/index.html).

In contrast, the languages provided here are for *making scripts* in Godot projects. Godot has many methods for granting language support:

- **Modules:** Maintainers/Developers define custom implementations of Godot's `Script`, `ScriptInstance`, and `ScriptLanguage` types in a module. Users add the module to the engine source code and compile the engine themselves (or a developer may provide precompiled binaries). Now you have a new built-in language.
- **PluginScript:** Maintainers/Developers write an EditorPlugin addon which teaches the Editor how to understand the target language as a `ScriptLanguage`. Users should only need to download the addon. Powered by Godot's *[GDNative](https://docs.godotengine.org/en/latest/tutorials/plugins/gdnative/what_is_gdnative.html) C interface* module.
- **NativeScript:** Maintainers write tools to generate and build "bindings" in the target language. Developers use the tools to create bindings, write scripts, and compile them into a native library for an addon. Users download the addon and use the native scripts in their projects. To write custom functionality, most people are both Developers and Users. Powered by Godot's *[GDNative](https://docs.godotengine.org/en/latest/tutorials/plugins/gdnative/what_is_gdnative.html) C interface* module.
    - Note: The Developer role's complexity is dependent on the quality of the Maintainer's tools. As such, it is language-dependent. Usually, they are difficult. Your mileage may vary!

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

1. ### [GDScript](https://docs.godotengine.org/en/stable/getting_started/scripting/gdscript/index.html) 💍 🧬 🔌 ⚙️
   GDScript is actively maintained and documented and is stable. It is the primary language, has the most tutorials online, and has deep in-Godot editor support.

1. ### [VisualScript](https://docs.godotengine.org/en/stable/getting_started/scripting/visual_script/index.html) 💍  🧬 ⚙️
   VisualScript can be considered as a secondary scripting language with blocks-and-nodes. It too provides rich support, although there is a community effort to make it more intuitive to use as a design tool instead of what users describe as a one-to-one mapping of code with terse programming jargon where it should be more humanized.

## 🥇 Production Ready
   These languages are documented and stable. Some people use these in production.

1. ### [C#](https://docs.godotengine.org/en/stable/getting_started/scripting/c_sharp/index.html) 💍 🔌 ⚙️
   C# support is an official module. If you have a Mono-version of Godot Engine, it comes built into the engine.
   Most people are using the [VSCode](https://github.com/godotengine/godot-csharp-vscode) extension.

1. ### [JavaScript](https://github.com/GodotExplorer/ECMAScript) 👥 🔌 ⚙️
   JavaScript support is a 3rd-party module. Modules add built-in support (like GDScript) but require [compiling it into the engine](https://docs.godotengine.org/en/stable/development/cpp/custom_modules_in_cpp.html).
   With JavaScript, you also get support for languages that transpile to JavaScript, like [TypeScript](https://www.typescriptlang.org/) or [CoffeeScript](https://coffeescript.org/) and [F# Fable](https://fable.io/).

1. ### [Lua](https://github.com/perbone/luascript) 👥 🧬 🔌 ⚙️
   Lua is currently undergoing a rewrite of its parser.

1. ### [Nim](https://github.com/pragmagic/godot-nim) 👥 🔌 🔧
   Nim has standard NativeScript features for the moment, but wishes to go beyond that by [improving its user experience](https://github.com/pragmagic/godot-nim/issues/66) to automate repetitive boilerplate tasks.

1. ### [Rust](https://github.com/godot-rust/godot-rust) 👥 🔌 🔧
   You can find the project homepage [here.](https://godot-rust.github.io/)

## 🥈 Nearly There
   Stable and not documented yet.

1. ### [Clojure](https://github.com/arcadia-unity/ArcadiaGodot) 👥 🔌 🏄
   Based on Mono. No API documentation. Usable and community supported. 

1. ### [D](https://github.com/godot-d/godot-d) 👥 🔌 🔧
   Maintained by Sheep. Available in the official Discord channel. 
   It is feature complete, performant and pretty much without any documentation.

1. ### [Haskell](https://hackage.haskell.org/package/godot-haskell) 👥 🔌 🔧
   Maintained by the SimulaVR folks. Feature complete and undocumented. 

## 🥉 Has Potential
   In active development, comparable to being in beta stage.

1. ### [F#](https://github.com/willnationsdev/godot-fsharp-tools) 👥 🔌 🏄 
   With C#, you also get support for integrating other Mono-supported languages, e.g. F# or VisualBasic. But, Godot currently hardcodes C# usage. Any class attached to a Node or Resource must be a C# script.
   For tools to automate the use of F# with Godot's C# scripts, see [Godot F# Tools](https://github.com/willnationsdev/godot-fsharp-tools).

1. ### [Go (godot-go)](https://github.com/godot-go/godot-go/) 👥 🔌 🔧
   Go bindings from godot-go are a recent project in alpha. There is decent documentation of the build workflow and example scripts. It is actively being developed.

1. ### [Kotlin JVM](https://github.com/utopia-rise/godot-jvm) 👥 🔌 ⚙️
   Currently in [Alpha](https://github.com/utopia-rise/godot-jvm/blob/master/docs/src/doc/pre-alpha.md). More or less feature complete with a few missing targets and some limitations, but with documentation and good performance characteristics. Their [Discord](https://discord.gg/3NSA7fKBMD) is nice and friendly.

1. ### [Python](https://github.com/touilleMan/godot-python) 👥 🧬 🔌 📜
   Python is the language for which PluginScript, the API that provides Godot-editor support, got designed for. It provides editor integration as GDScript does - it's still in beta. Currently, the bottleneck to its stability is its flawed [export system](https://github.com/touilleMan/godot-python/issues/146).
   PyCharm is another way of doing Python for Godot, and this one supports [visual debugging](https://medium.com/@prokopst/debugging-godot-python-with-pycharm-b5f9dd2cf769)

1. ### [Swift](https://github.com/kelvin13/godot-swift) 👥 🔌 🔧
   Provides bindings and a Swift Package Manager-powered build system for creating Godot native libraries from Swift frameworks. GDScript APIs are written in terms of Swift protocols and generics, allowing for seamless Swift-to-Godot interoperability. Automates nearly all of the process of registering types and members with the Godot runtime, and ships with an expressive, SIMD-accelerated math library. Has comprehensive [API documentation](https://kelvin13.github.io/godot-swift/) and [tutorials](https://github.com/kelvin13/godot-swift/tree/master/examples).

## 🏅 Okay, I guess?
Potential [skub](https://knowyourmeme.com/memes/skub).

1. ### [C++ *GDNative support*](https://github.com/godotengine/godot-cpp) 💍 🔌 🔧
   C++ is a bit of a hot potato anywhere, and it is here as well: some people like to use it, but it could use better documentation in places. Some peeves such as not being able to use modern C++ features starting from C++11 dwell in this API.

## 🐣 Up and coming
Comparable to being in alpha stage.

1. ### [Ada](https://github.com/MichaelAllenHardeman/gdnative_ada) 👥 🔌 🔧
   This isn't documented or (probably) stable, but it is still very new.

1. ### [Dart](https://github.com/mahdisml/DartGodot) 👥 🔌 🏄
   Uses Godot's C# API to make calls to Dart script code. Has code for generating scripts.

1. ### [Smalltalk](https://gitlab.com/chandler.justin.s/godot-talk-VM) 👥 🔌 🏄
   Used in production, still certain core features missing. Uses a custom C# VM to interpret arbitrary
   bytecode from a Pharo Smalltalk library. Cuis Smalltalk support planned.
   [Discord server available.](https://discord.gg/xkZEQrb3Xn)

## ⚰️ Left 4 Dead

1. ### [AngelScript](https://github.com/Geequlim/AngelScript)👥 🔌 🔧
   AngelScript was @Geequlim's first forray into GDNative, before making the ECMAScript bindings.

1. ### [Crystal](https://github.com/kalinon/godot-crystal) 👥 🔌 ⚙️
   Mentions nothing about its usability, unmaintained since over 2 years.

1. ### [Go (ShadowApex)](https://github.com/ShadowApex/godot-go) 👥 🔌 🔧
   Go bindings from ShadowApex haven't been updated since 2018. Not documented or stable enough for production.

1. ### [Haxe](https://github.com/mrcdk/godot-haxe) 👥 🔌 🔧

1. ### [Kotlin Native](https://github.com/utopia-rise/godot-kotlin) 👥 🔌 🔧
   Kotlin Native bindings are declared unready for production use and deprecated due to performance problems. Although, it was feature complete at the time of the drop.
   Here is the old [documentation](https://godot-kotl.in/en/latest/) of it.

1. ### [Object Pascal](https://github.com/BenediktMagnus/godot-object-pascal) 👥 🔌 🔧

1. ### [Ruby](https://github.com/onyxblade/godot-ruby) 👥 🔌 🔧
   Ruby bindings haven't been updated since 2018.
   It's an attempted PluginScript system, but it's designed poorly with ~15x performance loss vs. GDScript.
   Not documented or stable enough for use.

1. ### [Zig](https://github.com/outrera/godot-zig) 👥 🔌 🔧

## 🌐 Other Useful links

- Gamesfromscratch made a [video](https://youtu.be/VqcMlS-IJl4) about some of the supported languages.
- (You can expand this list!)

## Enjoy ^-^
