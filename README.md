# PHP Learning Notes (Obsidian Vault)

A structured repository of personal study notes, syntax guides, code snippets, and development roadmaps for mastering **PHP (HyperText Preprocessor)** for modern back-end web development.

---

## 📖 Background & Purpose

This collection of notes is maintained within an [Obsidian](https://obsidian.md/) knowledge base to document the learning progression of server-side programming with PHP. 

The primary goals of this repository are to:
- **Build a Strong Foundation**: Master core PHP language syntax, data structures, and control flow mechanisms.
- **Understand Server-Side Execution**: Learn how local development environments (e.g., Apache/Nginx, local dev servers) execute PHP scripts and generate dynamic web content.
- **Bridge Back-End & Databases**: Progressively cover database interactions (MySQL), secure querying (prepared statements, CRUD operations), and state management (sessions, cookies).
- **Prepare for Full-Stack & API Development**: Transition from foundational scripts to building RESTful APIs, processing authentication/authorization, and communicating with frontend applications.

---

## 🗂️ Obsidian Vault Structure & Contents

```text
PHP/
├── README.md                                       # Repository overview and documentation
├── Roadmap.md                                      # Comprehensive 6-phase learning roadmap
├── PHP Fundamentals/                               # Core syntax and language basics
│   ├── Guide.md                                    # Curriculum breakdown and tutorial references
│   ├── Introduction to PHP.md                      # Language overview and local web server setup
│   ├── Variables, Data Types & Concatenation.md    # Variables, types, identifiers, and string concatenation
│   ├── Numbers & Operators.md                      # Arithmetic, precedence, shorthands, and increment/decrement
│   └── Strings.md                                  # String methods, indices, quoting rules, and length
├── PHP Logic/                                      # Flow control and decision-making
│   ├── Conditional Statements.md                   # if, if..else, if..elseif..else, and switch statements
│   └── Looping Statements.md                       # while, do..while, for, and foreach loops
└── PHP Data Handling/                              # Data structures and modular code (In Progress)
    └── Untitled.md                                 # Working notes for arrays and functions
```

---

## 📚 Detailed Topic Breakdown

### 1. [PHP Fundamentals](PHP%20Fundamentals/)
Covers foundational building blocks required to read and write PHP scripts:
- **Introduction**: Server-side execution models, dynamic page rendering, and running local development servers.
- **Variables & Data Types**: Variable declaration (`$var`), identifiers, data types, and the concatenation operator (`.`).
- **Numbers & Operators**: Type conversion, arithmetic operators, operator precedence rules, shorthand operators, and increment/decrement behavior.
- **Strings**: Single vs. double quotes, string indexing, character length inspection, and essential string manipulation functions.

### 2. [PHP Logic](PHP%20Logic/)
Focuses on control flow and algorithmic execution:
- **Conditional Statements**: Branching execution paths using `if`, `else`, `elseif`, and multi-case `switch` structures.
- **Looping Statements**: Repeating code blocks with condition-controlled loops (`while`, `do...while`), counter loops (`for`), and collection traversal (`foreach`).

### 3. [PHP Data Handling](PHP%20Data%20Handling/) *(In Progress)*
Deals with organizing and encapsulating data:
- Indexed, associative, and multidimensional arrays.
- Reusable custom functions, parameters, return types, and scope.

---

## 🗺️ Master Learning Roadmap

The learning sequence follows the 6 progressive phases outlined in `Roadmap.md`:

| Phase | Milestone | Focus Areas |
| :--- | :--- | :--- |
| **Phase 1** | **PHP Fundamentals** | Variables, data types, concatenation, basic operators, and string handling |
| **Phase 2** | **PHP Logic** | Conditionals (`if`, `else`, `switch`) and iteration (`for`, `while`, `foreach`) |
| **Phase 3** | **Data Handling** | Indexed/associative/multidimensional arrays and function design |
| **Phase 4** | **Backend Processing** | `$_GET` & `$_POST` handling, form validation, sanitize inputs, sessions & cookies |
| **Phase 5** | **MySQL Integration** | PDO/MySQLi connections, CRUD operations, prepared statements, and error handling |
| **Phase 6** | **Backend Applications** | Authentication & registration, JSON REST APIs, and frontend integration |

---

## 🛠️ How to Use with Obsidian

1. Open **Obsidian**.
2. Select **Open folder as vault** and choose this directory:
   ```text
   Obsidian Notes/Web Development/Back-End/Programming Languages/PHP
   ```
3. Use Obsidian's graph view, internal `[[WikiLinks]]`, and markdown preview for seamless navigation across notes and roadmap milestones.
