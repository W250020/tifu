# TIFU Chatbot Stimuli

Interactive chatbot stimuli for the TIFU manuscript (Studies 1 and 2), built as
self-contained HTML pages and hosted via GitHub Pages for embedding in Qualtrics.

## Condition key

| Variable | Level | Meaning |
|---|---|---|
| **T** (Transparency) | T1 | Chatbot explicitly references what the participant said |
| | T0 | Chatbot response is generic, no back-reference |
| **I** (Interpretability) | I1 | Chatbot explains the underlying mechanism ("because...") |
| | I0 | Chatbot stays at the practical/logistical level |
| **A** (Autonomy, Study 2 only) | A1 | Chatbot validates the participant's own judgment, presents illusory choice |
| | A0 | Chatbot is directive, no choice offered |

Study 1 is a 2×2 (T × I) design. Study 2 is a 2×2×2 (T × I × A) design.

## Live links

### Study 1

| Condition | Link |
|---|---|
| T1_I1 | https://w250020.github.io/tifu/study1-T1_I1.html |
| T1_I0 | https://w250020.github.io/tifu/study1-T1_I0.html |
| T0_I1 | https://w250020.github.io/tifu/study1-T0_I1.html |
| T0_I0 | https://w250020.github.io/tifu/study1-T0_I0.html |

### Study 2

| Condition | Link |
|---|---|
| T1_I1_A0 | https://w250020.github.io/tifu/study2-T1_I1_A0.html |
| T1_I0_A0 | https://w250020.github.io/tifu/study2-T1_I0_A0.html |
| T0_I1_A0 | https://w250020.github.io/tifu/study2-T0_I1_A0.html |
| T0_I0_A0 | https://w250020.github.io/tifu/study2-T0_I0_A0.html |
| T1_I1_A1 | https://w250020.github.io/tifu/study2-T1_I1_A1.html |
| T1_I0_A1 | https://w250020.github.io/tifu/study2-T1_I0_A1.html |
| T0_I1_A1 | https://w250020.github.io/tifu/study2-T0_I1_A1.html |
| T0_I0_A1 | https://w250020.github.io/tifu/study2-T0_I0_A1.html |

## Embedding in Qualtrics

Insert via a Text/Graphic question, switch to the HTML view of the rich content
editor, and drop in an iframe pointing at the relevant URL:

```html
<iframe src="https://w250020.github.io/tifu/study1-T1_I1.html"
        width="100%" height="750" style="border:none;"></iframe>
```

Swap the `src` per condition/block. Height of 700–750px gives room for the
scenario card plus a few visible messages without the participant needing to
scroll the outer survey page.

## Notes

- Study 2's `_A1` files include a 3-option choice widget at three points in the
  conversation (illusory choice per SDT: the participant's selection changes
  the displayed message, not the chatbot's subsequent response).
- All bubble text is sourced directly from `TIFU_Manuscript_Stimuli_22_June.xlsx`
  (22 June update tab), with two approved wording overrides in Study 2 Turn 6/7
  to remove activity-specific language that presupposed the Turn 4 choice.
