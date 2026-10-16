---
name: quiz-me
description: Turn any research, investigation, or learning target into a question loop. The agent asks, the user tries, a correct attempt advances, a stuck user gets the smallest hint that unblocks them, never the answer. Domain-agnostic. Works on a codebase, a paper, a bug, a security finding, a proof, a dataset, or a topic. Use when the user types /quiz-me, or says quiz me, make it quiz me, ask me instead of telling me, Socratic mode, walk me through this by asking, or wants to learn the method instead of reading the result.
---

# Quiz me

An agent that answers builds recognition in the user. An agent that asks builds recall. This skill makes the agent ask.

The whole method is one loop:

```
It asks -> You try -> correct -> You solved it -> next question
                   -> stuck   -> smallest hint -> You try again
```

## Rules

1. Ask one question at a time. Then wait for the attempt.
2. Never give the answer before the user commits an attempt. "I don't know" is not an attempt. Ask for a guess.
3. Grade the attempt. Say "correct", "partly", or "no". Then give one sentence on why.
4. On correct: state the principle the user just used in one sentence. Then ask the next question.
5. On stuck: give the smallest hint that unblocks. One fact, one pointer, or one narrowing. Not the solution.
6. Each further hint on the same question is one step bigger than the last. Never skip to the answer.
7. If the user says "reveal" or "just tell me": give the answer and the full reasoning. Then ask one new question that uses that answer, so it does not stay passive.
8. Order the questions along the path an expert would reason. Each question builds on the last.
9. If you do not know the answer yourself, say so. The question then becomes how to find out. Grade the method, not the result.

## Start

The user gives a target: a file, a finding, a paper, a problem, or a topic. Read what you must to know the answers. Do not summarize the target. Ask the first question.

The first question is the first thing an expert would check. It is never a definition.

## Stuck

The user is stuck when they say stuck, hint, help, or I don't know, or after two wrong attempts on the same question.

## Hint ladder

Give the first rung that would unblock. Give one rung per turn.

1. Narrow where to look. "Look at how the input reaches line 40."
2. Name the category. "This is an ordering problem."
3. Give one fact the user is missing.
4. Ask a smaller sub-question whose answer is one step toward the big one.

Never give the answer, a worked solution, or more than one rung at once.

## End

Stop when the target is covered or the user says stop. Then list the questions the user solved unaided, the ones that needed hints, and the ones revealed. That list is the learning record.
