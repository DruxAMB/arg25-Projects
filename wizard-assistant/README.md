# ARG25 Project Submission Template

Welcome to Invisible Garden- ARG25.

Each participant or team will maintain this README throughout the program.  
You’ll update your progress weekly **in the same PR**, so mentors and reviewers can track your journey end-to-end.



##  Project Title
Wizard IDE Gemini Assistant

## Team
- Team/Individual Name: Muhammad Amoo
- GitHub Handles: [@druxamb](https://github.com/druxamb)
- Devfolio Handles: @druxamb

## Project Description
Extend the Wizard Stylus IDE with an embedded Google Gemini assistant that helps developers navigate the editor, troubleshoot local compilation flows, and quickly access official Stylus documentation. The goal is to keep the assistant privacy-focused (no server-side chat storage) while providing contextual guidance sourced from a curated `llm.tx` playbook.

## Tech Stack
- React + TypeScript (Wizard frontend)
- Vite, Tailwind CSS, Radix UI
- Google Generative AI SDK (`@google/generative-ai`)
- Supabase (auth + persistence already used by Wizard)
- Node.js toolchain (npm scripts, ESLint)

## Objectives
- Deliver an overlay assistant in `EditorPage` with a responsive UI and typing indicator.
- Load IDE guidance from `public/llm.tx` and enforce Stylus question redirects to official docs.
- Ensure conversations remain in-memory only (no backend logging or storage).
- Document the feature so reviewers can validate behavior quickly.

## Weekly Progress

### Week 1 (ends Oct 31)
**Goals:** Research Wizard codebase, confirm Gemini SDK compatibility, draft `llm.tx` guidance.  
**Progress Summary:** Mapped EditorPage layout, identified injection points for an overlay, produced first version of `llm.tx` with IDE navigation notes.

### Week 2 (ends Nov 7)
**Goals:** Build the assistant component, fetch guidance at runtime, integrate Stylus-doc redirection logic.  
**Progress Summary:** Created `EditorAssistant` sheet, wired it into `EditorPage`, and added keyword detection that links Stylus questions to https://docs.arbitrum.io/stylus.

### 🗓️ Week 3 (ends Nov 14)
**Goals:** Polish UX (typing indicator, copy tweaks), prep PR messaging, and run lint/tests ahead of submission.  
**Progress Summary:** Added bouncing-dot “thinking” state, refined copy, documented dependencies, and compiled PR summary. Lint run exposed unrelated legacy warnings that still need follow-up.

## Final Wrap-Up
- **Main Repository Link:** [Wizard Assistant](https://github.com/DruxAMB/wizard.git)
- **Demo / Deployment Link (if any):** _Not yet hosted; feature runs locally via `npm run dev`._  
- **Slides / Presentation (if any):** _N/A_

## 🧾 Learnings
- Integrating Gemini safely requires carefully scoped prompts and clear UX disclaimers.  
- Maintaining a local-only conversation history keeps compliance risk low but adds state-management considerations.  
- Stylus-specific support is best handled by deferring to canonical docs rather than attempting to synthesize answers.

## Next Steps
- Resolve lint warnings surfaced during `npm run lint` (legacy `any` usage and unused imports).  
- Capture short demo footage of the assistant in action.  
- Explore optional session persistence once privacy implications are clarified.

_This template is part of the [ARG25 Projects Repository](https://github.com/invisible-garden/arg25-projects)._  
_Update this file weekly by committing and pushing to your fork, then raising a PR at the end of each week._
