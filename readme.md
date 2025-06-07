# The Library

**A Personal Codex of Concepts, Coded.**

## 📖 About This Project (Nature)

"The Library" is my personal, evolving knowledge base dedicated to housing the mathematical formulas, concepts, and algorithms I learn. The primary focus is currently on mathematics, 
Might also expand to include physics, astronomy, and other quantitative fields as my learning journey progresses. Idk just thoughts.

This project is more than just a static collection; it's an active learning tool where I translate theoretical knowledge into practical code.

## 🎯 Core Principles & Objectives

**Core Principles:**

- **Modularity:** Components are designed to be as independent as possible to promote reusability.

- **Testing:** All mathematical operations must have corresponding unit tests to ensure correctness and prevent regressions.

- **Documentation:** Public-facing classes, methods, and functions will have clear docstrings explaining their purpose, parameters, and return values.

- **Version Control:** Git is used from the start, with a convention of frequent, clear commit messages.

- **Mathematical Precision:** All implemented formulas and algorithms are checked against reliable sources to ensure accuracy.

**Primary Goals**:

*   **Deepen Understanding:** To solidify my grasp of algebric and quantitative/analytic concepts by implementing them programmatically. The act of coding a concept forces a deeper level of understanding.
*   **Language Proficiency:** To learn and improve my skills in both **Python** and **Java** by developing two separate, parallel versions of this application. This will allow me to compare implementations and understand language-specific nuances.
*   **Useful Resource:** To potentially develop this into a robust library that I can leverage for other personal projects requiring mathematical or scientific computations.
*   **Track Progress:** To serve as a tangible record of my learning and development in various STEM fields.

## 🏁 Getting Started

This project contains parallel implementations in Python and Java.

**Prerequisites:**
*   Python 3.10+
*   Java JDK 21+ (Gradle is included via the wrapper)

**To build the Java project:**
```bash
# From the project root (thelibrary/)
./gradlew build
```
**To run the Python project:**
```bash
# From the project root (thelibrary/)
cd src/python
pip install -r requirements.txt
python __main__.py
```

## 🚀 Roadmap

My development plan is structured as follows:

The Library is organized thematically, with each major area of mathematics on its own "Shelf." Development will proceed shelf by shelf, focusing on creating robust, well-tested components.

**Shelf 1: Foundations**
*   `[ ] Number Theory:` Euclidean algorithm, prime factorization.
*   `[ ] Set Theory:` Custom `Set` class with core operations. (Mostly an extention of the already existing Set class in Python & Java)
*   `[ ] Combinatorics:` Factorials, binomial coefficients.

**Shelf 2: Algebra**
*   `[ ] Linear Algebra:` `Vector`, `Matrix`, and `Determinant` classes with core operations.
*   `[ ] Polynomials:` `Polynomial` class with full arithmetic.
*   `[ ] Abstract Structures:` Interfaces/classes for `Group`, `Ring`, and `Field`.

**Shelf 3: Analysis**
*   `[ ] Sequences & Series:` `Sequence` class, convergence tests.
*   `[ ] Calculus:` Tools for symbolic differentiation and numerical integration.

**Shelf 4: Geometry**
*   `[ ] Euclidean Space:` `Vector` class with dot products, norms, and angles.

## 💻 Technologies

*   **Primary Languages:** Python, Java
*   **Potential UI (Python):** Libraries like Tkinter, PyQt, Kivy, or even a web framework like Flask/Django for a local web app. (mostly gonna go with the web app)
*   **Potential UI (Java):** Libraries like Swing, JavaFX.
*   **Plotting/Visualization (Python):** Matplotlib, Seaborn, Plotly.
*   **Plotting/Visualization (Java):** JFreeChart, or libraries that can bridge to JavaScript plotting if using JavaFX webview.

## ⚙ Structure

<details>
<summary>Click to view the full directory structure</summary>
    
    TheLibrary/
    ├── .gitattributes
    ├── .gitignore
    ├── build.gradle.kts
    ├── settings.gradle.kts
    ├── gradlew
    ├── gradlew.bat
    ├── gradle/
    │
    ├── LICENSE                                                     # MIT probably ?
    ├── README.md
    ├── IDEAS.md                                                    # Brainstorming Log for future concepts.
    │
    ├── docs/                                                       # Project dashboard and documentation site.
    │   ├── index.html                                              # The main project index.
    │   ├── style.css                                               # Styles for the index.
    │   └── script.js                                               # Scripts for interactivity (filtering tags, etc.).
    │
    └── src/
        ├── java/
        │   └── src/
        │       ├── main/
        │       │   ├── java/
        │       │   │   └── com/socrateingenieour/thelibrary/
        │       │   │       ├── Main.java
        │       │   │       │
        │       │   │       ├── mathematics/                        # Section: Mathematics
        │       │   │       │   ├── package-info.java
        │       │   │       │   │
        │       │   │       │   ├── foundations/                    # Shelf 1: Foundations
        │       │   │       │   │   ├── package-info.java
        │       │   │       │   │   ├── SetTheory.java
        │       │   │       │   │   ├── Combinatorics.java
        │       │   │       │   │   └── NumberTheory.java
        │       │   │       │   │
        │       │   │       │   ├── algebra/                        # Shelf 2: Algebra
        │       │   │       │   │   ├── package-info.java
        │       │   │       │   │   ├── abstract_structures/
        │       │   │       │   │   │   ├── Group.java
        │       │   │       │   │   │   └── Ring.java
        │       │   │       │   │   ├── Polynomial.java
        │       │   │       │   │   └── linear_algebra/
        │       │   │       │   │       ├── package-info.java
        │       │   │       │   │       ├── Vector.java
        │       │   │       │   │       ├── Matrix.java
        │       │   │       │   │       └── Determinant.java
        │       │   │       │   │
        │       │   │       │   ├── analysis/                       # Shelf 3: Analysis
        │       │   │       │   │   ├── package-info.java
        │       │   │       │   │   ├── Sequence.java
        │       │   │       │   │   ├── Calculus.java
        │       │   │       │   │   └── DifferentialEquation.java
        │       │   │       │   │
        │       │   │       │   └── geometry/                       # Shelf 4: Geometry
        │       │   │       │       ├── package-info.java
        │       │   │       │       └── EuclideanSpace.java
        │       │   │       │
        │       │   │       └── physics/
        │       │   │           └── package-info.java
        │       │   │
        │       │   └── resources/
        │       │
        │       └── test/
        │           ├── java/
        │           │   └── com/socrateingenieour/thelibrary/
        │           │       └── mathematics/
        │           │           └── algebra/
        │           │               └── linear_algebra/
        │           │                   ├── VectorTest.java
        │           │                   └── MatrixTest.java
        │           └── resources/
        │
        └── python/
            ├── __main__.py
            ├── requirements.txt
            │
            ├── lib/
            │   ├── __init__.py
            │   │
            │   ├── mathematics/                                    # Section: Mathematics
            │   │   ├── __init__.py
            │   │   │
            │   │   ├── foundations/                                # Shelf 1: Foundations
            │   │   │   ├── __init__.py
            │   │   │   ├── set_theory.py
            │   │   │   ├── combinatorics.py
            │   │   │   └── number_theory.py
            │   │   │
            │   │   ├── algebra/                                    # Shelf 2: Algebra
            │   │   │   ├── __init__.py
            │   │   │   ├── abstract_structures.py
            │   │   │   ├── polynomials.py
            │   │   │   └── linear_algebra/
            │   │   │       ├── __init__.py
            │   │   │       ├── vector.py
            │   │   │       ├── matrix.py
            │   │   │       └── determinant.py
            │   │   │
            │   │   ├── analysis/                                   # Shelf 3: Analysis
            │   │   │   ├── __init__.py
            │   │   │   ├── sequences_and_series.py
            │   │   │   ├── calculus.py
            │   │   │   └── differential_equations.py
            │   │   │
            │   │   └── geometry/                                   # Shelf 4: Geometry
            │   │       ├── __init__.py
            │   │       └── euclidean_space.py
            │   │
            │   └── physics/
            │       └── __init__.py
            │
            └── tests/
                ├── __init__.py
                └── mathematics/
                    ├── __init__.py
                    ├── foundations/
                    │   └── test_number_theory.py
                    └── algebra/
                        ├── test_polynomial.py
                        └── linear_algebra/
                            ├── test_vector.py
                            └── test_matrix.py
    
</details>



## 📝 My Notes & Suggestions for Myself

*   **Sets in Python:** Python has excellent built-in `set` objects with highly optimized operations.
    *   **Why implement my own custom`Set` then?**
        1.  **Convinience:** I need to work with classes in my project, so I'll just extend the already existing set class for now.
        2.  **Specific Needs:** I might want to add custom behaviors, logging, or internal representations not available in the standard `set`.
        3.  **Learning Exercise:** The primary goal is to learn by coding. Implementing set logic from scratch (e.g., how unions or intersections work algorithmically) is a valuable exercise. 
        4.  **Java Parallel:** Since Java's standard library `Set` interface is different, building my own in Python helps keep the conceptual design parallel if I aim for similar custom features in both versions.
    *   **Recommendation:** I should definitely use Python's built-in `set` for general use in other parts of the Python version (due to its efficiency), but the custom `Set` will be a specific module for learning and deeper understanding.

*   **Version Control:** Use Git from the very beginning! Commit often with clear messages.
*   **Modularity:** Design modules and classes to be as independent as possible, especially if this is to become a reusable library.
*   **Testing:** Write unit tests for functions and methods, especially for mathematical operations, to ensure correctness. This is crucial for a "calculator" or library. Python's `unittest` or `pytest` and Java's JUnit are good starting points.
*   **Documentation:** Write clear docstrings for all classes, methods, and functions. This will be invaluable later.
*   **Start Simple:** Don't try to build everything at once. Focus on one concept or feature, get it working, then move to the next.
*   **Mathematical Rigor:** When implementing formulas, double-check them against reliable sources to ensure accuracy.

## 🛠️ Current Status

*   [x] Initial project setup (folders, basic file structure for Python/Java versions).
*   [ ] Begun defining blueprints for [mention first concept, e.g., Matrices] in [Python/Java].

*(This README is a living document and will be updated as the project progresses.)*