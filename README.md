# 🗺 An overview about the available language bindings for Godot

### ⚠ Disclaimer

If you want to help, or if you are a language maintainer, see here: https://github.com/Vivraan/godot-lang-support/issues

This list is for Godot 4. In case you are looking for Godot 3 bindings, find them [here](https://github.com/Godot-Languages-Support/godot-lang-support/blob/15fb99b3214959432aedffb91218b4bd33d3789f/README.md)

Note that some of that projects have moved on to Godot 4, so you will have to use one of their older versions.

See the README or contact the project for further information.

The engine itself, and the Godot modules are developed in C++. 
For those, please start with the official docs for [contributing to the engine](https://docs.godotengine.org/en/stable/community/contributing/index.html) and [understanding engine development](https://docs.godotengine.org/en/stable/development/cpp/index.html).

In contrast, the languages provided here are for programming the game logic. There are different methods for extending the engine, and granting additional language support:

- **Modules:** Maintainers/Developers define custom implementations of Godot's `Script`, `ScriptInstance`, and `ScriptLanguage` types in a module. Users add the module to the engine source code and compile the engine themselves (or a developer may provide precompiled binaries).

- **GDExtension:** This is the official, new way to implement plugins for Godot 4. One of the limitations here is, that it wont support the Nintendo Switch. It has the benefit, that it does not need to be compiled into the engine, and gives more control over it.

## Categories

### By editor support
- 🧬 Can be edited inside Godot Engine 
- 🔌 Has support for the Godot API in an external editor.

### By maintainer
- 💍 Official
- 👥 Community-maintained

### By method
- ⚙️ Module
- 🧩 GDExtension
- 🏄 "Surfs" on another language
- 🏰 Sandboxes the code

## 🏆🥇 Production Ready
   These languages are documented and stable.  
   *In alphabetical order*. 
   
### [C++ / Godot module](https://docs.godotengine.org/en/stable/contributing/development/core_and_modules/custom_modules_in_cpp.html)  💍 ⚙️
   
   You can code your entire project (or parts of it) in C++ and include the game logic as Godot modules.

 ### [C++ / Jenova](https://jenova-framework.github.io/)  🧬 🔌 👥 🧩
   Jenova provides not only hot reloadable C++ game scripting, editor support within Visual Studio, Visual Studio Code, and Godot itself, but also a lot of other features like support for nested GDExtension development, an inbuilt virtual machine for starting an entire OS, that can be embedded into the game, and interact with it.

   It also provides its own API for the development of extensions, although currently undocumented.

   Limited to Windows and Linux as development platform.

   A non-free edition that provides encrypted code obfuscation and more, is also available.

### [C++, Rust and Zig](https://github.com/libriscv/godot-sandbox)  👥 🏰 🧩
   This mainly focuses on Cpp and Rust support and also features Zig. It sandboxes the code and is suitable for modding support. 

### [C#](https://docs.godotengine.org/en/stable/getting_started/scripting/c_sharp/index.html)  💍 🔌 ⚙️ 🧩
   C# support is made possible by an official Godot module. If you have the dotnet version of Godot or Blazium, it comes built-in. It does not support web export via wasm as of now.
   
### [D](https://github.com/godot-dlang/godot-dlang)  👥 🔌 🧩
   New, maintained binding to GDExtension. 

### [GDScript](https://docs.godotengine.org/en/stable/getting_started/scripting/gdscript/index.html)  💍 🧬 🔌 ⚙️
   GDScript is actively maintained, documented and is stable. It is the primary language in the Godot ecosystem, has the most tutorials online, and deep Godot editor support.
   Can be extended with [Golden Nugget](https://monnef.gitlab.io/golden-gadget/features). 

### [Haxe](https://github.com/SomeRanDev/reflaxe.GDScript)  👥 🔌 🏄
   Does compile Haxe to GDScript.
   Made with the `reflaxe` framework.

### [JavaScript and Typescript](https://github.com/godotjs/GodotJS)  👥 🔌 🧩
   Javascript and Typescript extension, with multiple different backends to choose from. 

### [Kotlin, Java, and Scala.](https://github.com/utopia-rise/godot-jvm)  👥 🔌 ⚙️
   Provides proper support for Kotlin and Java. Aims to support Scala in the near future as well. Their [Discord](https://discord.gg/3NSA7fKBMD) is nice and friendly.

### [Lua](https://github.com/gilzoide/lua-gdextension)  👥 🧩
   New and exciting binding, that allows to use Lua both directly, and as well by calling into it from other languages.

### [Nim](https://github.com/godot-nim/gdext-nim)  👥 🔌 🧩
   Feature complete, hot reloadable implementation of Nim.

### [Orchestrator](https://github.com/CraterCrash/godot-orchestrator)  👥 🧬 🧩
   Orchestrator is a visual scripting language with advanced macro support to provide high-level abstractions.
Friendly and competent support.
Also usable for dialog scripting. 
It provides rich API support, is implemented in C++, and compiles to native code. 

### [Rust](https://github.com/godot-rust/gdext)  👥 🔌 🧩
   You can find the project homepage [here.](https://godot-rust.github.io/)

### [Swift](https://github.com/migueldeicaza/SwiftGodot)  👥 🔌 🧩
   Very well-supported implementation by Miguel Deicaza.

   There is also [SwiftGodotKit](https://github.com/migueldeicaza/SwiftGodotKit)

## 🤪 Curiosities 
   Stable programming languages, ... with a twist 😉 

### [Enu](https://github.com/dsrw/enu)  👥 🧬 ⚙️
   Experimental block-based language and framework. 

### [Ink](https://github.com/inkle/ink)  👥 🔌 🏄
   Scripting language for writing interactive narrative.

## 🥈 Halfway there
   In active development, and comparable to being in the beta stage.

### [Block Coding](https://github.com/endlessm/godot-block-coding)  🧬 👥 🧩
   Scratch-like visual coding in blocks.

### [Dart](https://github.com/fuzzybinary/godot_dart)  👥 🧩
   The project's README contains a detailed roadmap.

### [Go 1](https://github.com/godot-go/godot-go/)  👥 🔌 🧩
   Go bindings to GDExtension.

### [Go 2](https://github.com/grow-graphics/gd)  👥 🔌 🧩
   Go bindings to GDExtension.
   Possible to use it for shaders.

### [Lua](https://github.com/perbone/luascript)  👥 🧬 🔌 ⚙️
   This version of Lua is currently undergoing a partial rewrite and seems to be stuck in development.

### [Python](https://github.com/touilleMan/godot-python/tree/godot4-meson)  👥 🧬 🔌 🧩
   Currently in reconstruction.

### [Python 2](https://github.com/niklas2902/py4godot)  👥 🧬 🧩
   Python implementation from scratch. 

### [WASM](https://github.com/Dheatly23/godot-wasm)  👥 🏰 🏄
   Bindings for wasm. Implemented via the Rust bindings.

### [WASM 2](https://github.com/ashtonmeuser/godot-wasm)  👥 🏰 ⚙️ 🧩
   Allows to load WASM libraries from other languages. Available as both module and GDExtension.

### [Zig](https://github.com/thimenesup/GodotZigBindings)  👥 🔌 🧩
   Almost no documentation is provided, uncertain about the status of the project. 

## 🌐 Other Useful links

- See the language/scripting section on [Wikipedia.](https://en.wikipedia.org/wiki/Godot_(game_engine)#Scripting)
- Gamesfromscratch made a [video](https://youtu.be/zdqSLz9ZpqQ) about some of the supported languages.
- (You can expand this list!)

## Enjoy ^-^
