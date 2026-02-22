# Claude Skills

A collection of custom skills for [Claude Code](https://claude.ai/code).

## Available Skills

| Skill | Description |
|-------|-------------|
| `cpp-tutor` | Interactive C++ tutor covering modern C++ (C++11-C++23), build systems, testing frameworks, third-party libraries, and code explanation. |

## Getting Started

Clone this repository:

```bash
git clone https://github.com/greggkp/claude-skills.git
```

## Installing Skills

### Option 1: Copy into your project

Copy a skill into the root of your project so it's available when you use Claude Code there:

```bash
mkdir -p /path/to/your/project/.claude/skills
cp -r claude-skills/.claude/skills/cpp-tutor /path/to/your/project/.claude/skills/
```

### Option 2: Install as personal skills

Copy a skill into your personal Claude configuration so it's available across all projects:

```bash
mkdir -p ~/.claude/skills
cp -r claude-skills/.claude/skills/cpp-tutor ~/.claude/skills/
```

### Invoking a skill

Once installed, you can invoke a skill directly in Claude Code by typing `/cpp-tutor` followed by a topic or question. Skills can also be invoked automatically by Claude when your conversation matches the skill's description.

**Learning C++ concepts:**

```
/cpp-tutor smart pointers
/cpp-tutor move semantics and rvalue references
/cpp-tutor what are concepts in C++20?
```

**Learning libraries and tooling:**

```
/cpp-tutor how do I set up googletest with CMake?
/cpp-tutor parameterized tests in Catch2
/cpp-tutor integrating nlohmann/json with FetchContent
```

**Explaining code:**

```
/cpp-tutor explain the template metaprogramming in src/traits.hpp
/cpp-tutor what does this code do?
/cpp-tutor walk me through the CRTP pattern in this file
```
