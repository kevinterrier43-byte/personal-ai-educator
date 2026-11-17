# Design Decisions

Short notes on why the educator is built the way it is.

## 1. A configured assistant instead of a custom app

A ChatGPT Project gave me what I needed without building anything: persistent instructions, project sources synced from Google Drive, and image and PDF generation for the cheat sheets. That let me focus on the teaching design rather than infrastructure.

**Tradeoff:** the logic lives in natural-language instructions, so it's less predictable and less testable than code. Generated cheat sheets in particular vary from run to run. A coded version of that step is in [AI Cheat Sheet Generator](https://github.com/kevinterrier43-byte/ai-cheat-sheet-generator).

## 2. One fixed lesson format

Early lessons varied a lot in depth and structure depending on the topic. A fixed six-step format (foundations → concepts → application → knowledge check → feedback → study notes) makes every course feel the same, which makes note-taking easier and gives every lesson a built-in practice step.

## 3. Knowledge checks before answers

The educator asks a question and waits for my answer before revealing it, then grades my reasoning, not just the final choice. Having to commit to an answer first shows me what I actually understood, instead of what just sounded familiar.

## 4. Assessment results as a starting point, not a rule

The project includes my results from two learning assessments (a learning-preference questionnaire and a motivation and learning-strategies questionnaire). The instructions say these "aren't necessarily completely accurate, but they're a good base." In practice they're condensed into a one-line learning profile: foundations-first, concept-driven and hands-on. The educator uses that summary rather than re-reading the full reports each time.

## 5. Separate instructions, reference data and operational data

- **Instructions** (how to teach) change rarely and only when I revise them.
- **Reference data** (how I learn, sample notes and cheat sheets, study list) changes as I add material.
- **Operational data** (course progress, knowledge gaps) changes every session.

Keeping these apart means I can add a new set of study notes without touching the teaching rules.

## 6. Handwritten notes, printed cheat sheet

The writing happens during the lessons: I take notes by hand as I go, because that's how I retain the material. The cheat sheet is the reference I keep afterward, so it's limited to one printed A4 sheet. The constraint forces real prioritization: if something doesn't fit, it wasn't essential.

## 7. Scoped memory

Within a topic, the educator builds on what I've already shown I understand. Across topics, it starts fresh. Without that rule, a new course could cut detail based on something I'd studied in an unrelated one.
