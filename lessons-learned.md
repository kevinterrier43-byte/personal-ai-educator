# Lessons Learned

Things I changed after using the educator for my own study.

## What worked

- **Giving it data instead of asking it to guess.** Rather than asking the AI what my learning style is, I gave it evidence to build from: results from two learning assessments, my own study notes, and my finished cheat sheets. The instructions treat the assessments as starting hypotheses, not facts.
- **Comparing models before changing the design.** I ran design questions through Perplexity Model Council and a local copy of Andrej Karpathy's [LLM Council](https://github.com/karpathy/llm-council), where several models answer, review each other, and a chairman model combines the results. I still made the final call.
- **A topic as the only prompt.** Removing the setup step made it much easier to actually start studying.
- **A fixed lesson format.** Once every lesson followed the same six steps, my notes became consistent too, and building the final cheat sheet got easier.
- **Real samples over descriptions.** Giving the educator my actual handwritten notes and finished cheat sheets worked better than describing the style I wanted.
- **Using AI to edit the instructions.** I ran my draft instructions through ChatGPT to remove repetition and reorganize them into clear sections, then decided which changes to keep.

## What didn't work at first

- **Ignoring my learning profile.** Early lessons didn't reflect my preferences, so I condensed my assessment results into a short summary and pointed the instructions directly at it.
- **Lessons that were too short.** Optimizing for concise output sometimes meant thin lessons. The instructions now separate the two: lessons should be thorough, and only the cheat sheet should be compressed.
- **Carrying over context between topics.** Lessons could trim material based on unrelated past courses, so memory is now scoped to the current topic (see design decision 7).
- **Inconsistent two-page sheets.** On a front-and-back cheat sheet, the second page sometimes came out in a different style from the first. I now review both pages together and ask for them to match.
- **PDF-only output.** I needed an editable version on my Mac to make small fixes, so I ask for that alongside the PDF.

## Keeping it fun

I added two small rules on purpose: three topic images at the start of every lesson, and emojis where they fit. Studying on my own works better when it doesn't feel like a chore.

## What I haven't measured yet

I don't have numbers on retention or time saved. Adding a simple progress tracker, and later spaced review, is the next step.
