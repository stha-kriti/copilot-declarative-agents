# Microsoft Copilot Declarative Agents

Three declarative agents I designed in Microsoft 365 Copilot (Agent Builder) for everyday study and work tasks.
Each spec contains the exact instructions, conversation starters, knowledge sources, test prompts and what I
changed after testing.

| Agent | Use case | Spec |
|---|---|---|
| Literature Review Assistant | Triage and critically read papers, no invented citations | [agents/01_literature_review_assistant.md](agents/01_literature_review_assistant.md) |
| Exam Study Coach | Quiz and study plan built only from uploaded lecture material | [agents/02_exam_study_coach.md](agents/02_exam_study_coach.md) |
| Meeting Action Items Agent | Turns messy meeting notes into decisions, owners and due dates | [agents/03_meeting_action_items_agent.md](agents/03_meeting_action_items_agent.md) |

`evidence/` holds screenshots of the configuration and of test conversations before and after each instruction change.

## What I learned

- Short, rule-based instructions with an explicit behaviour for missing information ("say not stated") work better than long persona text.
- Fixing the output structure makes answers easy to check and compare between test runs.
- Every agent needs a fixed test set: I re-ran the same prompts after each instruction change and kept a log of failures and fixes.
