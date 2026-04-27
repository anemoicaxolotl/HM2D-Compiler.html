# HM2D Logic Compiler v1.4

**Primi-HM2D Edition** - The primitive, foundational form of the HM2D programming language

---

## 📋 About HM2D

**HM2D** (Hierarchical Modular 2-Dimensional Logic) is a custom programming language designed to bridge logical reasoning with spatial operations and keyboard integration. This repository contains **Primi-HM2D**, the most simplified, foundational version of the language—perfect for learning the core concepts before advancing to more complex implementations.

### Founded By
**Kaileb James Hitch** - Creator and Lead Designer of the HM2D Language Specification

---

## 🎯 What is Primi-HM2D?

Primi-HM2D represents the **primitive** (simple, foundational) implementation of HM2D logic. It focuses on:

- **Simplicity**: Easy-to-learn syntax with minimal complexity
- **Core Operations**: Essential commands for output and keyboard integration
- **Foundation**: Serves as the base for more advanced HM2D implementations
- **Full Keyboard Bridge**: Direct integration with hardware input (QWERTY keyboard)

---

## 🏗️ Core Protocols

### 1. **SAY Protocol** - Output/Communication
```hm2d
say (: Hello, World! :)
say (: This is a message to the terminal :)
```
**What it does:** Outputs text to the terminal. Used for logging, debugging, and communication within programs. Text must be wrapped in `(: :)` parentheses.

**Syntax:** `say (: YOUR MESSAGE HERE :)`

---

### 2. **Hardware Bridge** - Keyboard Input Integration
```hm2d
on #Q# key === , say (: Q Pressed :) ,
on #Space# key === , say (: Space was pressed :) ,
on #Enter# key === , say (: Enter key triggered :) ,
```
**What it does:** Maps keyboard keys to HM2D actions. When a physical key is pressed, the associated logic executes automatically. The Hardware Bridge is **always active** - just press any key!

**Syntax:** `on #KEY# key === , ACTION ,`

**Supported Keys:** All QWERTY letters (A-Z), Space, Enter, Shift, Escape

---

### 3. **Identity Gates** - Logic Organization
```hm2d
* LoginCheck * : say (: User authenticated :)
* StartSequence * : say (: Initialization started :)
```
**What it does:** Creates named logic gates that organize code and improve readability. Identity gates can be invoked manually or through the Hardware Bridge.

**Syntax:** `* GATE_NAME * : ACTION`

---

## 🖥️ The Compiler Interface

This project includes a **web-based HM2D compiler** with the following features:

### Features:
- **Live Code Editor**: Write HM2D code in a dark-themed editor
- **Execution Terminal**: Real-time output with timestamped messages
- **Hardware Bridge Keyboard**: Visual QWERTY keyboard for testing
- **Active State Monitor**: See all active logic gates in real-time
- **Keyboard Shortcuts**: Full physical keyboard integration

### Interface Components:
1. **Header**: Compiler version, creator info, and control buttons
2. **Code Editor** (Left): Main textarea for writing HM2D source code
3. **Hardware Bridge** (Top Right): Visual keyboard buttons
4. **Active State Identities** (Bottom Right): Monitor running logic gates
5. **Execution Terminal** (Bottom): Real-time output and logs

---

## 🚀 How to Use

### 1. Open the Compiler
- Clone or download this repository
- Open `index.html` in a web browser
- You'll see the HM2D compiler interface with starter code

### 2. Write Code
In the left editor panel, write HM2D code:
```hm2d
say (: Starting HM2D program :)
* MyGate * : say (: Gate activated :)
on #A# key === , say (: A key pressed :) ,
```

### 3. Execute
- Click the **EXECUTE SCRIPT** button, or
- Press any keyboard key to trigger Hardware Bridge actions

### 4. View Output
Check the terminal at the bottom for execution results, timestamps, and any errors

---

## 📝 Example Programs

### Example 1: Hello World
```hm2d
say (: Hello, World! :)
say (: Welcome to HM2D :)
```

### Example 2: Keyboard Integration
```hm2d
on #Q# key === , say (: Q pressed - Starting sequence :) ,
on #W# key === , say (: W pressed - Processing data :) ,
on #E# key === , say (: E pressed - Complete :) ,
```

### Example 3: Logic Gates
```hm2d
* Initialize * : say (: System initialized :)
* Process * : say (: Processing input :)
* Terminate * : say (: System shutdown :)
on #Space# key === , * Initialize * : say (: Space triggered init :) ,
```

### Example 4: Comments
```hm2d
// This is a comment and will be ignored
say (: This will execute :)
// Only lines starting with // are ignored
```

---

## 🔍 Technical Details

### Language Features
- **Whitespace-Flexible**: Extra spaces are generally ignored
- **Comment Support**: Lines starting with `//` are ignored
- **Case-Sensitive**: Commands must be lowercase
- **Sequential Execution**: Commands execute in order from top to bottom
- **Hardware Aware**: Keyboard events trigger bridge actions immediately

### Compilation Process
1. **Parsing**: Code is split into individual commands
2. **Capsule Registration**: Hardware bridge capsules are registered first
3. **Validation**: Each command is checked for syntax validity
4. **Execution**: Valid commands are executed and logged
5. **Hardware Sync**: Keyboard input automatically triggers mapped actions

### Error Handling
- **Unknown Protocol**: Syntax errors are logged to terminal in red
- **Graceful Degradation**: Invalid lines are skipped; valid code continues
- **Terminal Logging**: All errors include timestamps for debugging

---

## 🎓 Learning Path

**Beginner:**
- Start with `say (: :)` commands to understand output
- Learn to use the Hardware Bridge with one key
- Practice syntax with comments

**Intermediate:**
- Create multiple Hardware Bridge mappings
- Use Identity Gates for organization
- Combine commands in sequences
- Test with the visual keyboard

**Advanced:**
- Create complex multi-key sequences
- Organize code with multiple Identity Gates
- Build interactive keyboard-driven programs
- Debug using terminal timestamps

---

## 📦 Version Information

- **Current Version**: 1.4 (Primi-HM2D Logic)
- **Release Date**: 2026
- **Edition**: Primitive/Foundational
- **Status**: Stable and ready for use
- **Language Composition**: 100% HTML/CSS/JavaScript

---

## 🔮 Future Versions

Beyond Primi-HM2D, the HM2D language roadmap includes:
- **Standard-HM2D**: Variables, functions, and data structures
- **Advanced-HM2D**: Object-oriented features and modules
- **Full-HM2D**: Complete language specification with external compilation

---

## 📄 License

This project is created by Kaileb James Hitch. Usage and distribution terms available upon request.

---

## 💡 Tips & Tricks

1. **Test incrementally**: Build one Hardware Bridge mapping at a time
2. **Use comments liberally**: Add `// comments` to explain your logic
3. **Check the terminal**: All output is timestamped for debugging
4. **Visual keyboard**: Use the buttons to test Hardware Bridge actions
5. **Active states**: Monitor the right panel to see your Identity Gates in action
6. **Keyboard shortcuts**: Press physical keys to trigger Hardware Bridge actions
7. **Clear often**: Use the Clear Terminal button to keep output readable

---

## 🤝 Contributing & Support

For questions, suggestions, or improvements regarding HM2D:
- Check the HM2D documentation in this repository
- Contact the creator: Kaileb James Hitch
- Test and provide feedback through GitHub issues

---

## 🎮 Quick Start Templates

**Template 1: Simple Message**
```hm2d
say (: Welcome to my HM2D program! :)
```

**Template 2: Keyboard Controller**
```hm2d
on #A# key === , say (: Action A triggered :) ,
on #B# key === , say (: Action B triggered :) ,
on #C# key === , say (: Action C triggered :) ,
```

**Template 3: Organized Gates**
```hm2d
* Welcome * : say (: Welcome to HM2D :)
* Ready * : say (: System ready for input :)
on #Space# key === , * Welcome * : say (: Starting... :) ,
```

---

**Happy coding with Primi-HM2D! 🚀**

**Built with ❤️ by Kaileb James Hitch**
