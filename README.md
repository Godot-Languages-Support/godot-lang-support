# 🗺 An overview of the available language bindings for Godot & Co

This repository aims to provide a faithful overview of the available language bindings,  
and other related projects that target the Godot Engine, or one of its many forks.

For each language support project, look for the individual `LICENSE` file on the public repository that is linked.  
This document itself is licensed under the [CC-BY-4.0](/LICENSE). We do welcome [help](/#help) to keep it as up-to-date as possible!

## Categories

### By maintainer
- 💍 Official
- 👥 Community-maintained

### By method
- ⚙️ Module
- 🧩 GDExtension
- 🏄 "Surfs" on another language
- 🏰 Sandboxes the code

### By editor support
- 🧬 Can be edited inside the Godot Engine (and its forks)
- 🔌 Has support for the Godot API being edited in an external editor.

### By target platform 
- 🌍 Web
- ⚡ On JIT restricted platforms (Consoles, iOS)^

^Consoles support is not available by default; an SDK and implementation are also needed.

## 🏆🥇 Production ready
   These languages are documented and stable.  
   *In alphabetical order*. 
   
### [C++ / Godot module](https://docs.godotengine.org/en/stable/contributing/development/core_and_modules/custom_modules_in_cpp.html)  💍 ⚙️ 🌍 ⚡
   
   You can code your entire project (or parts of it) in C++ and include the game logic as Godot modules.

 ### [C++ / Jenova](https://jenova-framework.github.io/docs/pages/Getting-Started)  👥 🧩 🧬 🔌
   
   Jenova provides hot-reloadable C++  scripting and support for Visual Studio, VS Code, and the Godot editor.
   
   There is also support for nested GDExtension development and a built-in virtual machine for running an entire OS that can be embedded into the game and interacted with.

   It is one of the most advanced and best-maintained community extensions.

   The performance is factually on the same level as native C++, with a 0.005ms impact for calling functions from Godot.

   Jenova also provides its API for the development of extensions, although that is currently undocumented.

   It is only available for Windows, Linux, and macOS, for both development and export.

   You can use Jenova during the development stage and then switch to one of the other C++ integrations, or GDExtension itself, to ship the game to more platforms.

   In that case, you should be aware of potentially missing features with these extensions.
   As an example, users should not use functions stored in JenovaSDK unless they build it statically and link against it.

### [C++, Rust and Zig](https://github.com/libriscv/godot-sandbox)  👥 🧩 🏰 🌍 ⚡
   
   This mainly focuses on C++ and Rust support, and also features Zig. It sandboxes the code, making it suitable for modding support.

### [C#](https://docs.godotengine.org/en/stable/getting_started/scripting/c_sharp/index.html)  💍 ⚙️ 🔌 
   
   C# support is made possible by an official Godot module. If you have the .NET version of Godot or Blazium, it comes built-in. 

### [GDScript](https://docs.godotengine.org/en/stable/getting_started/scripting/gdscript/index.html)  💍 ⚙️ 🧬 🔌 🌍
   
   GDScript is actively maintained, documented, and stable. It is the primary language in the Godot ecosystem, has the most tutorials online, and deep Godot editor support.
   
### [Go](https://github.com/grow-graphics/gd)  👥 🧩 ⚡ 🌍
   
   Go bindings to GDExtension.
   Possible to use it for shaders.

### [Haxe](https://github.com/SomeRanDev/reflaxe.GDScript)  👥 🔌 🏄 🌍
   
   Compiles Haxe to GDScript.
   Made with the [reflaxe](https://github.com/SomeRanDev/reflaxe) framework.

### [JavaScript and Typescript](https://github.com/godotjs/GodotJS)  👥 🧩 🔌 🌍
   
   JavaScript and TypeScript extension, with multiple different backends to choose from. 

### [Kotlin, Java, and Scala.](https://github.com/utopia-rise/godot-jvm)  👥 ⚙️ 🔌 🌍 ⚡
   
   Provides proper support for Kotlin and Java. Aims to support Scala in the near future as well. 
   
   GraalVM with [Native Image](https://www.graalvm.org/latest/reference-manual/native-image/) is also supported.
   
   Their [Discord](https://discord.gg/3NSA7fKBMD) is nice and friendly.

### [Lua](https://github.com/gilzoide/lua-gdextension)  👥 🧩 ⚡
   
   New and exciting binding that allows Lua to be used both directly and by calling into it from other languages.

### [Nim](https://github.com/godot-nim/gdext-nim)  👥 🧩 🔌 🌍 ⚡ 
   
   Feature-complete, hot-reloadable implementation of Nim.

### [Orchestrator](https://github.com/CraterCrash/godot-orchestrator)  👥 🧩 🧬 ⚡
  
   Orchestrator is a visual scripting language with advanced macro support for high-level abstractions.  
   
   Friendly and competent support. Also usable for dialog scripting.  

   It provides rich API support, is implemented in C++, and compiles to native code. 

### [Rust](https://github.com/godot-rust/gdext)  👥 🔌 🧩 🌍 ⚡
  
   You can find the project homepage [here.](https://godot-rust.github.io/)

   Very well-supported, good documentation, and an active community.

### [Swift](https://github.com/migueldeicaza/SwiftGodot)  👥 🔌 🧩 🌍 ⚡
   
   Very well-supported implementation by Miguel Deicaza.

   There is also [SwiftGodotKit](https://github.com/migueldeicaza/SwiftGodotKit)

## 🤪 Curiosities 
   Stable programming languages... with a twist 😉 

### [Enu](https://github.com/dsrw/enu)  👥 🧬 ⚙️
   Logo-like framework in a block-based 3D world. Based on Nim.

### [Ink](https://github.com/inkle/ink)  👥 🔌 🏄
   Scripting language for writing interactive narrative.

## 🥈 Halfway there
   In active development, and comparable to being in the beta stage.

*The emojis here might be incomplete.*

### [Block Coding](https://github.com/endlessm/godot-block-coding)  🧬 👥 🧩
   Scratch-like visual coding in blocks.

### [BlockFlow](https://github.com/anidemdex/blockflow)  🧬 👥 🧩
   Eventsheet-based coding.  
A visual scripting designed to help in those scenarios where you need visual control of things that may happen sequentially in-game.

### [D](https://github.com/godot-dlang/godot-dlang)  👥 🧩 🔌
   New, maintained binding to GDExtension, ported from the previous GDNative extension.

### [Dart](https://github.com/fuzzybinary/godot_dart)  👥 🧩
   The project's README contains a detailed roadmap.

### [FlowKit](https://github.com/LexianDEV/FlowKit) 👥 🧬 
   Intuitive visual event-based language.

### [Go 2](https://github.com/godot-go/godot-go/)  👥 🔌 🧩
   Go bindings to GDExtension.

### [Lua](https://github.com/perbone/luascript)  👥 🧬 🔌 ⚙️
   This version of Lua is currently undergoing a partial rewrite and seems to be stuck in development.

### [Python](https://github.com/touilleMan/godot-python/tree/godot4-meson)  👥 🧬 🔌 🧩
   Currently in reconstruction.

### [Python 2](https://github.com/niklas2902/py4godot)  👥 🧬 🧩
   Python implementation from scratch. 

### [V](https://github.com/rosshadden/gdext-v)  👥 🔌 🧩
   Bindings for [the V programming language](https://vlang.io/).

### [WASM](https://github.com/Dheatly23/godot-wasm)  👥 🏰 🏄 🌍
   Bindings for wasm. Implemented via the Rust bindings.

### [WASM 2](https://github.com/ashtonmeuser/godot-wasm)  👥 🏰 ⚙️ 🧩 🌍
   Allows loading WASM libraries from other languages. Available as both a module and a GDExtension.

### [Zig](https://github.com/Doubleword-Labs/godot-zig) 👥 🔌 🧩 

   Makes good progress, still in beta.

### [Zig 2](https://github.com/thimenesup/GodotZigBindings)  👥 🔌 🧩 
   Almost no documentation is provided. This project's status is uncertain. 

## Help

As a small **volunteer** team with only two active maintainers (@ShalokShalom and @Vivraan), tracking community favourites versus cool upcoming demos of the GDExtension technology is challenging, given our busy schedules and attention spans 🫠

We welcome active contributors! If you are a language binding maintainer or wish to update us about new, existing, or discontinued projects, please submit a pull request with the relevant edits to this README.

We also accept issue submissions, but we will always prioritise PRs:
- PRs allow us to gather attention from various community members, including project maintainers, when describing the project.
- PRs take the pressure off, giving us time for detailed reviews and comments, and may even help us merge changes faster.

### GitHub Copilot/LLM/GenAI Statement

We aren't a code repository, but we will be ironsighted about requests that we suspect have used GenAI or the GitHub Copilot service. We consider that using a grammar engine to modify existing typed text differs from completely generating content through an LLM, and we will verify suspected claims introduced in diffs.

### What about Godot 3?

This list is for Godot 4. In case you are looking for Godot 3 bindings, find them at [this commit](https://github.com/Godot-Languages-Support/godot-lang-support/blob/15fb99b3214959432aedffb91218b4bd33d3789f/README.md)

Note that some of the projects mentioned there have transitioned from Godot 3 to Godot 4, so you will have to use one of their older versions for compatibility. Contact project maintainers for more information and let us know ASAP!

Godot Engine and its modules are developed in C++.
For info on those, please start with the official docs for [contributing to the engine](https://docs.godotengine.org/en/stable/community/contributing/index.html) and [understanding engine development](https://docs.godotengine.org/en/stable/development/cpp/index.html).

In contrast, the languages provided here are for programming the game logic (often called scripting).  
There are different methods for extending the engine and granting additional language support:

- **Modules:** maintainers/Developers define custom implementations of Godot's `Script`, `ScriptInstance`, and `ScriptLanguage` types in a module. Users add the module to the engine source code and compile the engine themselves (or a developer may provide precompiled binaries).

- **GDExtension:** This is the official, new way to implement plugins for Godot 4. One of the limitations here is that it won't support the Nintendo Switch. It has the benefit that it does not need to be compiled into the engine, and gives more control over it.

## Licensing note

The Godot Engine and its individual forks are licensed by their respective maintainers. 
Relevant licensing information is available on their website or on public source code mirrors.

## 🌐 Other Useful links

- See the language/scripting section on [Wikipedia](https://en.wikipedia.org/wiki/Godot_(game_engine)#Scripting).
- Gamesfromscratch made a [video](https://youtu.be/zdqSLz9ZpqQ) about some of the supported languages.
- Jeff Ward gave a [talk](https://www.youtube.com/watch?v=opHWwaogQvw) at GodotConf 2025 about adding new Script Languages to Godot.
- (You can expand this list!)

# Enjoy ^-^
