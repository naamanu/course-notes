# MIT-inspired self-study plan — draft 2

Prepared **2026-11-08** for a beginner with **10–15 hours per week**,
interested in machine learning, systems engineering, and distributed systems.
See [the catalog reference](README.md) for official requirements and sources.

Math starting point: school algebra, logarithms, and calculus have largely
been forgotten. Start the [math foundations track](math-foundations.md)
alongside introductory Python. Calculus follows algebra and trigonometry
readiness; the initial programming course can begin immediately.

## What we are building toward

The outcome is the ability to write reliable programs, explain their
correctness and cost, understand the machine and operating system they run
on, train and evaluate basic ML models, and eventually build a replicated
service. Progress is demonstrated through problems, code, and explanations.

We will use the current MIT curriculum to choose topics and prerequisites,
and public course materials to study them. An older complete public course
can be more useful than a current course page with restricted assignments.
This is a personal learning program, not an MIT credential or a claim to
have reproduced the whole degree.

## Start with one main course

Begin with **6.100A**, using the public **6.0001 Fall 2016** materials:

- [Course home](https://ocw.mit.edu/courses/6-0001-introduction-to-computer-science-and-programming-in-python-fall-2016/)
- [Lecture videos](https://ocw.mit.edu/courses/6-0001-introduction-to-computer-science-and-programming-in-python-fall-2016/video_galleries/lecture-videos/)
- [Assignments](https://ocw.mit.edu/courses/6-0001-introduction-to-computer-science-and-programming-in-python-fall-2016/pages/assignments/)

The official syllabus targets people with little or no programming
experience. Use a maintained Python 3 release; the 2016 examples may need
small compatibility adjustments. Course setup and the first assignment
will establish whether any tools need attention.

### Weekly rhythm

| Activity | Hours |
| --- | --- |
| Math explanations and written exercises | 5–7 |
| Python lectures and programming assignments | 4–6 |
| Review mistakes and retry earlier problems | 1–2 |

Choose within these ranges to stay inside 10–15 hours. For a 12-hour week,
use 6 hours for math, 5 for Python, and 1 for review. A difficult assignment
takes priority over watching the next lecture. Attempt problems before
looking at solutions; use hints first when asking for help.

## First checkpoint: two weeks

This is an initial pacing experiment, not a promise to finish half a course.

| Week | Work | Evidence |
| --- | --- | --- |
| 1 | Set up Python; work through lecture 1 and attempt problem set 0. Check signed numbers, fractions, and order of operations; review whichever are rusty. | A runnable first program, worked arithmetic exercises, and a short error log. |
| 2 | Work through lecture 2 if ready. Continue arithmetic practice, then begin simple expressions and equations when ready. Retry problems from week 1. | Small branching/loop examples, completed practice exercises, and an explanation of how an equation stays balanced. |

At the checkpoint, use actual assignment time and understanding to set the
next four weeks. If branching or loops remain confusing, spend another week
there. Move from arithmetic to algebra only when the practice is reliable.
Keep the full calculus and discrete-math courses for later readiness gates.

## First programming sequence

The time ranges are planning estimates at your weekly budget, not official
MIT durations. We will revise them after the first checkpoint. These blocks
are sequential within the Python strand, with math studied alongside them.

| Block | Main work | Approximate weeks | Exit evidence |
| --- | --- | --- | --- |
| A — Learn to program | 6.100A / public 6.0001 | 12–18 | Complete the programming assignments; write a small program from a blank file; explain functions, loops, basic data structures, testing, and debugging. |
| B — Model with programs | 6.100B / public 6.0002 | 12–18 | Build and explain a simulation; compare its results against a prediction; distinguish a model's assumptions from its outputs. |
| C — Build larger programs | 6.1010 / older 6.009 materials | 16–24 | Complete representative multi-part labs; reason about recursion and data representation; debug unfamiliar code and explain design decisions. |

These blocks total roughly 40–60 study weeks. Add breaks and catch-up
instead of compressing the assignments to fit a fixed anniversary.

Alongside them, rebuild arithmetic as needed, then algebra, functions,
exponents, logarithms, and basic trigonometry. See the [math track](math-foundations.md)
for resources and readiness checks. MIT's 18.01SC syllabus assumes high-school
algebra and trigonometry. Begin **18.01 single-variable calculus** after that
foundation is secure. The public 6.042J mathematics syllabus formally assumes 18.01,
so the full discrete-math course follows calculus readiness. Sampling logic,
sets, and simple proofs earlier is useful preparation, not completion of
that prerequisite. Calculus may need its own main-course block if new to you.

Public starting points:

- [6.0002 — Computational Thinking and Data Science, Fall 2016](https://ocw.mit.edu/courses/6-0002-introduction-to-computational-thinking-and-data-science-fall-2016/)
- [6.1010 — Fundamentals of Programming, Fall 2026](https://py.mit.edu/fall26):
  the landing page is public but asks for login for full access. Before
  block C, select an accessible archived offering and verify that its labs
  and starter files are available; access to the current offering is not assumed.
- [18.01SC — Single Variable Calculus](https://ocw.mit.edu/courses/18-01sc-single-variable-calculus-fall-2010/)
- [6.042J — Mathematics for Computer Science, Spring 2015](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/)

## Longer path, chosen by readiness

This is a dependency map, not a commitment to study every elective.
At 10–15 hours per week, broad coverage is a multi-year project. A rough
planning envelope is **3–5+ years** for substantial foundations and selected
ML/systems depth, depending on math preparation and assignment scope.

| Stage | Subjects | What you should be able to demonstrate |
| --- | --- | --- |
| Mathematical and algorithmic foundations | Finish 18.01 readiness; 6.1200; then 6.1210. Include 18.02 multivariable calculus before courses that formally require Calculus II. | Write induction and invariant arguments; implement data structures, graph search, and dynamic programming; justify correctness and complexity. |
| Reliable software and the machine | 6.1020; 6.1903 or 6.1904; then 6.1910. | Specify and test software; reason about memory, pointers, and assembly; explain how a processor executes a program. MIT lists Physics II for 6.1910, so review that background and the chosen public offering's prerequisites before scheduling it. |
| First ML specialization | 18.06 and 18.05 or 6.3700; then 6.3900. Add 6.S191 as a short extension if desired. | Implement a basic learning algorithm, create a baseline, use separate training/validation/test data, and explain errors and limitations. |
| First systems specialization | 6.1810, with 6.1800 as valuable broader systems study. Then consider 6.5831 databases or 6.5821 networks. | Extend xv6, explain synchronization and virtual memory, and reason about recovery or networking behavior. |
| Later depth | 6.1220 or 6.1400; 6.1060 performance engineering; optionally graduate 6.5840 distributed systems. | Prove a harder algorithm, measure an optimization, or build a replicated key-value service and test failures. |

6.1020 follows 6.1010. The current catalog lists 6.1020, 6.1210, and
6.1910 as prerequisites for 6.1060. Treat the graduate distributed course
as a later choice after substantial programming and systems work.

The linear algebra + probability combination is a recommendation for your
ML goals; the 6-3 degree itself permits a single subject from its math
selection. Our plan intentionally studies more math there.

## Keep the program small enough to finish

The first usable milestone is programming competence from blocks A–C.
After the foundations, choose **one** initial depth route:

- **ML first:** linear algebra and probability → 6.3900 → a small evaluated ML project.
- **Systems first:** C and architecture → 6.1810 → an xv6 lab portfolio.

The other route remains available later. Databases, networks, performance,
and distributed systems are extensions we can prioritize after experience
with the first specialization.

For completed work, retain source code, a brief explanation of decisions,
evidence of checking correctness, and a note about what remains unclear.
At each course boundary, attempt a new problem without following a worked
solution. Video completion alone is not the exit criterion.

Review the plan every four weeks. Revise it when assignment time consistently
exceeds the budget, prerequisites prove weak, material access fails, or your
interests change. Select public resources for the next stage at that review
instead of maintaining a detailed calendar years in advance.

## Decisions for our next discussion

The immediate next actions are a short arithmetic practice session and the
first 6.0001 lecture, followed by problem set 0 when Python is set up.
We can then refine:

1. Which arithmetic topics need practice, using the first two weeks' work.
2. Whether Bilibili should remain the preferred video source for every stage.
3. Whether the first specialization should be ML or systems, after trying both
   through small introductory exercises.

The principal risks are math readiness and access to complete lab materials.
The first two weeks check readiness; the review before each new course
checks materials and sets a realistic assignment scope.
