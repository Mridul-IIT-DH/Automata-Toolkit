# Automata Toolkit

A comprehensive **C++ toolkit for Formal Languages and Automata Theory**, supporting transformations between **Regular Expressions, ε-NFA, NFA, DFA**, along with **DFA minimization, isomorphism checking**, and **automata visualization**.

🚀 **One-click runnable using GitHub Codespaces** — no manual setup required.

---

## ✨ Features

- Regular Expression → ε-NFA conversion  
- ε-NFA → NFA → DFA conversion (subset construction)
- DFA minimization (including Brzozowski’s algorithm)
- DFA isomorphism checking
- ε-closure computation
- Automatic automata visualization using **Graphviz**
- Modular and extensible C++ design

---

## 🛠️ Tech Stack

- **Language:** C++
- **Compiler:** `g++`
- **Visualization:** Graphviz (DOT)
- **Platform:** GitHub Codespaces (preconfigured)

---

## 🚀 Running the Project (GitHub Codespaces)

This repository includes a **preconfigured `.devcontainer`**.

### ✅ No installation required  
The environment automatically provides:
- C++ compiler (`g++`)
- Graphviz
- Required VS Code extensions

---

### Open in Codespaces

1. Go to the GitHub repository
2. Click **Code → Codespaces → Create codespace on main**
3. Wait for the environment to initialize

That’s it — the project is ready to run.

---

### Run the Program

Open `code/src/main.cpp` and press `Ctrl + Alt + N`.

You need to create a `.txt` file in the `inputs` folder for program to read your input, and if you want to use option `isomorphism` option then the `.txt` file should be in `outputs` folder.

Format for naf, dfa are as follows:
```txt
STATES:
0 1 2

ALPHABET:
a b

TRANSITIONS:
0 a 0
0 b 0
0 a 1
1 b 2

INITIAL_STATES:
0

FINAL_STATES:
2
```
The above is the sample input please follow it exactly you are only allowed to modify the line just after the `heading` (like heading: `STATES:` so you can modify `0 1 2`). Please follow the exact spacing in between throughout.

Format for regular expression is just a single line with your choice of regular expression, below is a sample for the input .txt file for all the regulare expression related options:

```txt
(a*)*
```
The following symboles can be used in regular expression:
- Any alphabet character `a-z`
- Union `|`
- Concatination `.`
- Star `*`
- Parathesis `(`, and `)`

Follow the on-screen prompts to:

* Minimize regular expressions
* Generate ε-NFA, NFA, and DFA
* Minimize DFA
* Check DFA isomorphism
* Generate automata visualizations

---

## 📊 Automata Visualization

* The program generates `.dot` files automatically
* Graphviz converts them into images (e.g., `.png`)
* Output files are stored in the `output/` directory

You can open generated images directly inside Codespaces.

---

## 📁 Project Structure

```
.
├── .devcontainer/
├── .vscode/
├── include/
├── src/
├── .gitignore
└── README.md
```

---

## 🎓 Academic Relevance

This project demonstrates practical implementation of core concepts from:

* Theory of Computation
* Formal Languages and Automata Theory
* Compiler Design

Algorithms implemented include:

* Subset construction
* ε-closure computation
* DFA minimization
* DFA structural isomorphism

---

## 📌 Notes

* Designed for correctness, clarity, and extensibility
* Easily extendable to PDA or Turing Machine simulations
* Ideal for coursework, demos, and academic evaluation

---
