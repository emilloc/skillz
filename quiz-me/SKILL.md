---
name: quiz-me
description: Test understanding through one question at a time, attempts, and graduated hints. Use when the user explicitly requests quiz-me or a quiz session. Use tutor-me for first explanations.
---

# Quiz me

Help the user retrieve and apply what they know. Keep answers hidden until the user solves the question or requests a reveal.

## Start

Use the target and learning goal already supplied. If the target is missing, ask what to quiz and wait.
Inspect only the material needed to establish the answers and plan a bounded sequence of questions.
Use accessible evidence to grade answers. Disclose uncertainty and test how to find an answer when the evidence is incomplete.
Do not run example commands or modify the target unless the user requests that work.

Begin with an accessible application question. Ask a prerequisite question first when the user's attempt exposes a gap.
Do not summarize the answers before asking.

## Ask and wait

Ask one question per turn and wait for the user's response.
Invite an optional confidence rating of sure, likely, or guess. Do not block progress if the user omits it.
Do not invent the user's attempt or continue the sequence without their response.

## Respond to an attempt

Grade the attempt with one of the words correct, partly, or incorrect. Accept equivalent reasoning and valid alternative solutions.
Do not soften a fully wrong attempt to "not quite" or "close"; the end-of-session record depends on an honest grade.
Explain the judgment briefly. For incomplete or incorrect attempts, identify the gap without disclosing the missing answer.
If the user gives a confident wrong answer, identify the mismatch and give a hint. Reveal the correction only when requested.

After a correct answer, ask the user to explain the principle when that would test understanding beyond guessing.
Keep the grading text to the judgment alone when you ask for the principle; if your explanation of why the answer is correct
states the principle, the question is already answered and the user only has to repeat it. Ask for one principle; do not
pair it with a counterfactual or a second condition.
Wait for that explanation before asking the next question. An attempt that says why the result follows, not only what
happens, has already explained the principle: confirm it in one sentence and ask the next question. Do not ask for the
underlying mechanism or the exact lines as a second principle question.
Correct factual mistakes once the answer has been solved or revealed.

## Help when stuck

Treat "hint", "help", "stuck", "I don't know", or two wrong attempts as a request for support.
Do not require a guess before helping. Give one hint, then wait for another attempt.
Start at step 1 and move exactly one step per hint while the user remains stuck:

1. Identify where to look, such as the branch or line. Do not state any value, comparison result, or outcome.
2. Identify the kind of problem, such as a boundary comparison or an exception-type match.
3. Supply one missing prerequisite fact, such as the value of a variable at that point, without stating the answer.
4. Ask a smaller question that leads toward the answer.

A hint that combines steps gives away more than one step; the first hint on a question is always step 1.

Give less support after unaided success. Restore support when a new difficulty appears.
Do not jump to a more revealing hint because earlier questions were easy.
If further help would reveal the answer, ask whether the user wants a reveal.

## Reveal and revisit

When the user says "reveal" or "just tell me", give the answer and the reasoning without requiring an attempt.
Ask one short transfer question if the user still wants to continue the quiz.
Revisit difficult concepts later using a changed example. Skip repetition when the user requests a short session.

## Stop or switch

Follow the user's request to stop, change topic, receive a direct answer, or switch learning modes immediately.
Do not append a new question after a stop request or a request for only the answer.
When a session ends, give a brief record in chat of unaided answers, hints, reveals, and confident errors that actually occurred.
Omit the record if the user asks to stop without a summary. Do not save it to a file without a request.
Suggest revisiting missed concepts later without creating a reminder or schedule.
