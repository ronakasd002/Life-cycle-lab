# LifeCycle Lab

**Plan it. Estimate it. Test it.**

LifeCycle Lab is an integrated software engineering toolkit that brings four early stages of a software project into one application: choosing a lifecycle model, writing the requirements, estimating cost, and validating inputs through testing.

**Live demo:https://ronakasd002.github.io/Life-cycle-lab/**

## Flow of the project

Model > Specify > Estimate > Test

## Modules (4 integrated practicals)

| Practical | Module | What it does |
|---|---|---|
| EXP-1 | SDLC Model Simulator | Simulates Waterfall, Incremental, Prototyping and Agile step by step with a live phase tracker |
| EXP-3 | SRS Generator | Takes functional and non-functional requirements and produces an IEEE-format SRS document |
| EXP-5 | COCOMO Estimator | Calculates effort, development time, team size and cost using Basic COCOMO (Organic, Semi-detached, Embedded) |
| EXP-9 | Black-Box Tester | Tests input ranges using Boundary Value Analysis and Equivalence Class Partitioning with PASS/FAIL results |

## Problems it targets

- Confusion in choosing the right SDLC model
- Non-standard, messy requirement documents
- Project planning without effort and cost estimates
- Boundary bugs caused by unvalidated inputs

## Two versions

1. **Java console version** (in `src/`): a colourful, animated menu-driven program.
2. **Web version** (`index.html`): the same four modules with animations, hosted on GitHub Pages.

## How to run the Java version

Requirements: JDK 17 or newer.

```
javac -sourcepath src -d bin src/Main.java
java -cp bin Main
```

Use a terminal that supports colours (VS Code terminal or Windows Terminal).

## Project structure

```
LifeCycleLab/
├── index.html              (web version)
├── README.md
└── src/
    ├── Main.java           (main menu)
    ├── Ui.java             (colours, boxes, animations)
    ├── InputHelper.java    (input validation)
    ├── SdlcSimulator.java  (EXP-1)
    ├── SrsGenerator.java   (EXP-3)
    ├── CocomoEstimator.java(EXP-5)
    └── BlackBoxTester.java (EXP-9)
```

## COCOMO formulas used

- Effort = a x (KLOC)^b  (person-months)
- Time = c x (Effort)^d  (months)
- Cost = Effort x monthly salary per person

| Mode | a | b | c | d |
|---|---|---|---|---|
| Organic | 2.4 | 1.05 | 2.5 | 0.38 |
| Semi-detached | 3.0 | 1.12 | 2.5 | 0.35 |
| Embedded | 3.6 | 1.20 | 2.5 | 0.32 |

## Built with

Java (console version), HTML, CSS and JavaScript (web version)

## Author

Ronak, MCA, Software Engineering Lab Project
