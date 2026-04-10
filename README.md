# SIMPLE.py: Algebraic expression-simplifier
Step-by-Step Simplifier
**Version:** 1.0 — Midterm Release

A desktop application that simplifies or factors algebraic expressions step by step, showing the full solution trail with color-coded output.

---

## Features

- **Simplify** — expands brackets, groups like terms, and combines coefficients step by step
- **Factor** — identifies common factors and produces the fully factored form
- **Implicit multiplication** — type `2x` instead of `2*x`
- **Color-coded solution trail** — each section (GIVEN, METHOD, STEPS, FINAL, VERIFICATION, SUMMARY) is clearly labeled
- **Input validation** — catches empty input, invalid characters, unmatched parentheses, and division by zero
- **Stopping reason** — the trail always states why the process ended

---

## Dependencies

| Package | Purpose | Version |
|---------|---------|---------|
| Python  | Runtime | 3.8 or higher |
| tkinter | GUI (built into Python) | Included |
| sympy   | Symbolic math engine | 1.12 or higher |

---

## Installation — Step by Step

### Step 1 — Install Python

1. Go to https://www.python.org/downloads/
2. Download the latest Python 3 installer for your operating system
3. Run the installer
   - **Windows:** check the box that says **"Add Python to PATH"** before clicking Install
   - **Mac/Linux:** Python may already be installed; check by opening a terminal and typing `python3 --version`
4. Verify the install by opening a terminal or command prompt and running:
   ```
   python --version
   ```
   You should see something like `Python 3.11.x`

---

### Step 2 — Install SymPy

Open a terminal or command prompt and run:

```
pip install sympy
```

To verify it installed correctly:

```
python -c "import sympy; print(sympy.__version__)"
```

You should see a version number like `1.12`.

---

### Step 3 — Download the Program

Save `simple.py` to a folder on your computer, for example:
```
C:\Users\YourName\simplifier\simple.py       (Windows)
/Users/YourName/simplifier/simple.py         (Mac/Linux)
```

---

### Step 4 — Run the Program

Open a terminal or command prompt, navigate to the folder where you saved the file, then run:

```
python simple.py
```

The application window will open.

---

## How to Use

1. Type an algebraic expression in the input box
   - You can use `*` for multiplication, or skip it: `2x` works the same as `2*x`
2. Select a **Method** from the dropdown: `Simplify` or `Factor`
3. Press **Compute** — the solution trail will appear below
4. Press **Clear** to reset the input and trail
5. Click **About / Help** (top right) for a quick reference guide

---

## Example Inputs

| Expression | Method | Result |
|------------|--------|--------|
| `3x + 2x` | Simplify | `5*x` |
| `2*(x + 3) + x` | Simplify | `3*x + 6` |
| `x**2 - 4` | Factor | `(x - 2)*(x + 2)` |
| `x**2 + 2*x + 1` | Factor | `(x + 1)**2` |
| `x + y` | Simplify | Already simplified |

---

## Troubleshooting

**`pip` not found**
Try `pip3 install sympy` instead, or `python -m pip install sympy`

**tkinter not found**
On Linux, run: `sudo apt-get install python3-tk`
On Mac, reinstall Python from python.org (the official installer includes tkinter)

**The window does not open**
Make sure you are running Python 3, not Python 2. Use `python3 simple.py` if `python simple.py` does not work.
