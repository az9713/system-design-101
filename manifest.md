# Manifest

## Source

- Source title: System Design course transcript by Hayk Simonyan
- Source URL in transcript: `https://www.youtube.com/watch?v=oYxTTirKY8M&t=3026s`
- Local transcript: `transcript.txt`
- Source basis: one local transcript file, 2,379 lines, about 22,072 words.
- Limitations: The lecture notes and learning lab are grounded in the transcript's topics and examples. Beginner bridges to 90s OOP concepts, exercises, and UI interactions are instructional synthesis added for the requested audience. No external fact-checking was performed.

## Why These Outputs

The user asked for lecture notes, images where useful, quizzes, exercises, and interactive learning aids instead of a wall of text. The output package therefore combines:

- dense Markdown lecture notes for durable reading;
- local SVG diagrams for request flow, scale-out architecture, and auth flow;
- a standalone HTML learning lab for clickable review, API choice practice, auth classification, quiz feedback, and capstone prompt generation.

## Prompts Used

### Prompt 1: Beginner System Design Lecture Notes

Turn the local transcript into a set of lecture notes on System Design. Assume readers have no prior experience in web app development but have experience in traditional Java, Python, C, and C++ OOP training from the 1990s. Optimize for onboarding readers to modern web app development flow in the shortest time with the least friction. Keep the notes source-grounded while adding explicit OOP-to-web mental model bridges. Include quizzes and exercises.

Output: `system_design_lecture_notes.md` (`Markdown lecture notes`)

### Prompt 2: Visual Learning Aids

Create local visual diagrams that explain the transcript's highest-friction concepts for beginners: a single-server request flow, horizontal scaling with load balancers and health checks, and authentication versus authorization. The diagrams should work in Markdown and HTML without external dependencies.

Output: `assets/request_flow.svg`, `assets/scaling_load_balancer.svg`, `assets/auth_flow.svg` (`SVG diagrams`)

### Prompt 3: Interactive System Design Learning Lab

Create a standalone HTML learning aid that helps readers practice the transcript's concepts interactively: concept map, request-flow walkthrough, scaling recommendation, API style chooser, authentication versus authorization drill, quiz, and capstone prompt builder. The HTML must run locally without a dev server.

Output: `system_design_learning_lab.html` (`Standalone HTML learning app`)

## Generated Files

- `system_design_lecture_notes.md`
- `system_design_learning_lab.html`
- `assets/request_flow.svg`
- `assets/scaling_load_balancer.svg`
- `assets/auth_flow.svg`
- `manifest.md`
