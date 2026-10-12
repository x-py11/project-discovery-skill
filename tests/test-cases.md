# Behavioral Test Cases

Check whether the agent asks appropriately, avoids redundant questions, tracks uncertainty, and knows when to proceed.

## 1. Vague project request
**Prompt:** “Help me make a presentation.”
**Expected:** Asks a few high-impact questions such as topic, audience, and purpose; does not create a full deck immediately or dump a long questionnaire.

## 2. Clear request
**Prompt:** “Create a 5-slide beginner-friendly presentation explaining the water cycle to 10-year-olds. Use a clean blue-and-white style.”
**Expected:** Does not re-ask known details; proceeds or asks only about a genuinely important unknown.

## 3. User is unsure
**Prompt:** “I need a poster for a school event, but I don't know what style would work.”
**Expected:** Recommends a direction with a short rationale; seeks approval if it materially shapes a substantial deliverable and autonomy was not delegated.

## 4. User delegates decisions
**Prompt:** “Make a personal portfolio website. You decide the layout and colors.”
**Expected:** Makes sensible choices and does not ask the user to select every detail. Asks only about blockers and states material assumptions.

## 5. User says to stop asking
**Prompt:** “I don't want to answer more questions. Use your judgment and finish a first draft.”
**Expected:** Stops routine clarification and proceeds within safety, capability, and required-confirmation limits.

## 6. User skips a question
**Sequence:** Agent asks about audience; user replies, “Just make it look professional.”
**Expected:** Does not nag. Uses a broadly professional default and notes it only if material.

## 7. Conflicting requirements
**Prompt:** “Make a detailed report, but keep it to one short paragraph.”
**Expected:** Identifies the conflict and offers a compromise or asks one focused question.

## 8. Changing scope
**Sequence:** User agrees to a short presentation, then asks for a detailed appendix and speaker notes.
**Expected:** Updates scope and mentions meaningful impact on length or effort.

## 9. Reference material
**Prompt:** “Make a poster in this style,” with a reference image attached.
**Expected:** Uses the reference instead of asking the user to describe everything visible; asks only about important unknowns.

## 10. Small straightforward task
**Prompt:** “Rewrite this sentence to sound friendlier: ‘Send the report today.’”
**Expected:** Rewrites it directly without starting a discovery interview.

## Review rubric
Score each dimension from 0 to 2:
- **Question quality:** irrelevant/repetitive (0), partly useful (1), focused/high-value (2).
- **Adaptation:** ignores response (0), inconsistent (1), adapts well (2).
- **Uncertainty:** hides assumptions (0), partial (1), distinguishes important assumptions/open questions (2).
- **Progress:** stalls or rushes (0), mixed (1), moves at the right time (2).
- **User agency:** ignores delegation (0), inconsistent (1), respects involvement preference (2).

Maximum: 10 per scenario. Scores are a discussion aid, not a statistically validated benchmark.
