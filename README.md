# Prompt Library v1 — Study & Exam Notes

A reusable prompt template system for generating exam-ready study notes, built as part of the Neurofive Solutions prompt engineering task.

## What This Is

Instead of writing a new prompt from scratch every time I need study notes for a different topic, this project defines **one reusable template** with 5 labeled sections (Role, Context, Task, Format, Constraints) and swappable variables. Five different prompts are generated from that same template — one per course/topic — and all five were tested live in Claude.

## Files

| File | Description |
|---|---|
| `Prompt_Library_v1_Study_Exam_Notes.md` | Full deliverable — the template, all 5 instantiated prompts, and their tested outputs |
| `README.md` | This file |

## The Template

```
ROLE: You are an expert [SUBJECT] tutor who creates exam-focused study material
for [LEVEL] students.

CONTEXT: The student is preparing for [EXAM_TYPE] on [TOPIC], covered in
[COURSE_NAME]. They have [TIME_AVAILABLE] before the exam and
[PRIOR_KNOWLEDGE_LEVEL] with this topic.

TASK: Create [OUTPUT_TYPE] covering [SPECIFIC_SUBTOPICS], prioritizing the
concepts most likely to be tested.

FORMAT: [FORMAT_SPEC]. Keep it to approximately [LENGTH].

CONSTRAINTS: [CONSTRAINTS] — e.g. simple language, one worked example,
no filler/intro paragraphs, exam-relevant only.
```

## The 5 Prompts

1. **SDA — Architectural Styles** (Virtual Machine + Call-and-Return) → quick revision notes
2. **DBMS — BCNF Normalization** → flashcards
3. **Algorithms (CSC-321) — Min-Cost Flow** → cheat sheet
4. **SQL Server — T-SQL & core concepts** → practice Q&A
5. **OOP — Builder & Facade patterns** → summary notes

See `Prompt_Library_v1_Study_Exam_Notes.md` for the full text of each prompt and its output.

## How to Reuse This Template

1. Pick your subject/topic/exam
2. Fill in the bracketed variables in the template above
3. Paste into your AI tool of choice (tested here in Claude)
4. Adjust `FORMAT` and `CONSTRAINTS` depending on whether you want notes, flashcards, a cheat sheet, or practice questions

## Author

Hammad Asher — Software Engineering student, Bahria University Karachi
GitHub: [hammadAsher100](https://github.com/hammadAsher100)
