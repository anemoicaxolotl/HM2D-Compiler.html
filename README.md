# HM2D Logic Compiler v1.4

**Primi-HM2D Edition** - The primitive, foundational form of the HM2D programming language

---

## 📋 About HM2D

**HM2D** (Hierarchical Modular 2-Dimensional Logic) is a custom programming language designed to bridge logical reasoning with spatial and temporal operations. This repository contains **Primi-HM2D**, the most simplified, foundational version of the language—perfect for learning the core concepts before advancing to more complex implementations.

### Founded By
**Kaileb James Hitch** - Creator and Lead Designer of the HM2D Language Specification

---

## 🎯 What is Primi-HM2D?

Primi-HM2D represents the **primitive** (simple, foundational) implementation of HM2D logic. It focuses on:

- **Simplicity**: Easy-to-learn syntax with minimal complexity
- **Core Operations**: Essential commands for logic, movement, and temporal reasoning
- **Foundation**: Serves as the base for more advanced HM2D implementations
- **Accessibility**: Designed to be approachable for beginners and educators

---

## 🏗️ Core Commands

### 1. **SAY** - Output/Communication
```hm2d
say Hello, World!
say This is a message to the console
```
**What it does:** Outputs text to the terminal. Used for logging, debugging, and communication within programs.

---

### 2. **MOVE** - Spatial Navigation
```hm2d
move north
move east
move up
move southwest
```
**What it does:** Performs movement operations in a 2D or directional space. Used for navigating logical grids, positions, or states.

**Supported directions:** north, south, east, west, up, down, left, right, and diagonal combinations

---

### 3. **TEMPORAL** - Time-Based Logic
```hm2d
temporal delay 1000ms
temporal loop 5
temporal sync
```
**What it does:** Handles time-dependent operations, loops, delays, and synchronization. Essential for controlling execution flow and managing temporal sequences.

---

## 🖥️ The Compiler Interface

This project includes a **web-based HM2D compiler** with the following features:

### Features:
- **Live Code Editor**: Write HM2D code in a dark-themed editor with syntax highlighting
- **Execution Terminal**: Real-time output and execution logs with color-coded messages
- **Keyboard Shortcuts**: Press `Ctrl+Enter` to quickly execute code
- **Command Logging**: Different colors for different command types:
  - 🔵 **SAY** commands (blue) - communication outputs
  - 🟢 **MOVE** commands (green) - navigation operations
  - 🟣 **TEMPORAL** commands (purple) - time-based logic
  - 🔴 **ERRORS** (red) - compilation and runtime errors
  - ⚫ **SYSTEM** messages (gray) - compiler status updates

### Interface Components:
1. **Header**: Compiler version, creator information, and control buttons
2. **Code Editor** (Left): Main textarea for writing HM2D source code
3. **Execution Terminal** (Right): Real-time output and logging
4. **Execute Button**: Compile and run the current code
5. **Clear Button**: Reset the terminal output

---

## 🚀 How to Use

### 1. Open the Compiler
- Clone or download this repository
- Open `index.html` in a web browser
- You'll see the HM2D compiler interface

### 2. Write Code
In the left editor panel, write HM2D code:
```hm2d
say Starting HM2D program
move north
say Moved north successfully
temporal loop 3
move east
```

### 3. Execute
- Click the **Execute** button, or
- Press **Ctrl+Enter** on your keyboard

### 4. View Output
Check the terminal on the right for execution results and any errors

---

## 📝 Example Programs

### Example 1: Simple Navigation
```hm2d
say Initializing navigation system
move north
move east
move south
say Navigation complete
```

### Example 2: Temporal Loop
```hm2d
say Starting temporal operation
temporal loop 5
say This repeats 5 times
move forward
```

### Example 3: Error Handling
```hm2d
say Valid command
unknown_command invalid
// Comments are ignored and don't execute
say Program continues despite unknown command
```

---

## 🔍 Technical Details

### Language Features
- **Whitespace-Insensitive**: Extra spaces are ignored
- **Comment Support**: Lines starting with `//` are ignored
- **Case-Insensitive**: Commands work in any case (SAY, say, Say)
- **Single-Line Execution**: Each command is processed sequentially

### Compilation Process
1. **Parsing**: Code is split into individual commands
2. **Validation**: Each command is checked for validity
3. **Execution**: Valid commands are executed and logged
4. **Reporting**: Results and errors are displayed in the terminal

---

## 🎓 Learning Path

**Beginner:**
- Start with `say` commands to understand output
- Practice basic `move` operations
- Learn comment syntax

**Intermediate:**
- Combine commands in sequences
- Explore `temporal` operations
- Handle error messages

**Advanced:**
- Create complex programs with multiple operations
- Optimize command sequences
- Prepare to transition to full HM2D

---

## 📦 Version Information

- **Current Version**: 1.4 (Primi-HM2D Logic)
- **Release Date**: 2026
- **Edition**: Primitive/Foundational
- **Status**: Stable and ready for educational use

---

## 🔮 Future Versions

Beyond Primi-HM2D, the HM2D language roadmap includes:
- **Standard-HM2D**: Variables, functions, and data structures
- **Advanced-HM2D**: Object-oriented features and modules
- **Full-HM2D**: Complete language specification with compilation to machine code

---

## 📄 License

This project is created by Kaileb James Hitch. Usage terms available upon request.

---

## 💡 Tips & Tricks

1. **Use comments liberally**: Add `// comments` to explain your code
2. **Test incrementally**: Run small code segments before creating large programs
3. **Check the terminal**: All output and errors are logged with color-coding
4. **Keyboard shortcut**: Ctrl+Enter is faster than clicking Execute
5. **Clear often**: Use the Clear button to keep your terminal readable

---

## 🤝 Contributing & Support

For questions, suggestions, or improvements regarding HM2D:
- Check the official HM2D documentation
- Contact the creator: Kaileb James Hitch
- Submit feedback through this repository

---

**Happy coding with Primi-HM2D! 🚀**
