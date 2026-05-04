---
name: school-business-brief
description: Generates a structured business brief for school initiatives, programs, or proposals. Includes executive summary, stakeholder impact, resource requirements, implementation plan, and success metrics tailored to educational contexts. Use when drafting proposals for school boards, requesting budget approval for educational programs, or documenting initiatives for administrators.
---

# School Business Brief Generator

This skill generates comprehensive business briefs for educational initiatives, programs, or proposals. It produces structured documentation suitable for school boards, administrators, funding committees, and other decision-makers in K-12 or higher education settings.

## When this skill triggers

- "I need to pitch our after-school STEM program to the school board"
- "Help me write a proposal for a new reading intervention program"
- "I'm presenting our makerspace initiative to the superintendent next week"
- "Can you draft a budget justification for our mental health counseling expansion?"

## Inputs

- **initiative_name** — The name of the program, project, or initiative the brief covers.
- **purpose** — The problem being solved or opportunity being pursued.
- **target_audience** — Who will read this brief (e.g., school board, principal, funding committee).
- **scope** — Optional details about scale, timeline, affected populations, or specific requirements.

## Outputs

- **business_brief** — A formatted markdown document with sections for executive summary, background, objectives, stakeholder impact, resources, timeline, metrics, and risks.
- **executive_summary** — A standalone 1-paragraph summary of the initiative and its key points.

## How to perform this task

1. **Gather context** — Review all provided inputs. If critical details are missing (budget range, student population affected, timeline constraints), prompt the user for them. If they cannot provide specifics, acknowledge assumptions you'll make (e.g., "Assuming a one-year pilot program with existing staff").

2. **Ask the user to clarify whether this is K-12 or higher education** — Determine the educational context (public or private) and adjust tone accordingly. K-12 briefs emphasize student outcomes and parent communication; higher ed may focus on retention, research, or accreditation.

3. **Structure the brief** — Use this template as a foundation:
   - **Executive Summary** (3-5 sentences): Initiative name, purpose, who benefits, resource ask, expected outcome.
   - **Background & Need**: Explain the problem or opportunity with relevant data (test scores, enrollment trends, community feedback).
   - **Objectives**: 3-5 SMART goals specific to the initiative.
   - **Stakeholder Impact**: Address students, teachers/faculty, parents/families, administrators, and community separately.
   - **Resource Requirements**: Budget, staffing (FTE or hours), facilities, technology, materials.
   - **Implementation Plan**: Timeline with phases, key milestones, responsible parties.
   - **Success Metrics**: Quantitative (enrollment, scores, attendance) and qualitative (surveys, observations) measures.
   - **Risk Analysis**: 3-5 risks with mitigation strategies (e.g., low adoption → teacher training plan).

4. **Write the Executive Summary first** — This forces clarity. If you can't summarize in one paragraph, the initiative needs refinement. Include the "ask" (funding amount, board approval, policy change).

5. **Make objectives educational** — Avoid generic business language. Good: "Increase 3rd grade reading proficiency by 15% as measured by district assessments." Bad: "Improve literacy outcomes." Align with district goals, state standards, or institutional mission where possible.

6. **Detail stakeholder impact with specificity** — For students: what changes in their daily experience? For teachers: new prep time, training required, curriculum adjustments? For parents: communication plan, volunteer opportunities? For admin: reporting obligations, policy implications?

7. **Ground resource requirements in school realities** — Be realistic about budgets. If proposing a new program, reference per-pupil costs or benchmark against similar initiatives. For staffing, specify whether existing roles can absorb the work or new hires are needed. Mention grant opportunities if applicable.

8. **Build an implementation timeline with school calendar awareness** — Phase plans around academic terms, testing windows, professional development days. Include time for procurement, training, pilot testing, and scaling. Typical K-12 initiatives need 6-12 months for planning before launch.

9. **Choose metrics that matter to educators** — Academic growth, attendance rates, discipline referrals, parent engagement percentages, student/teacher surveys, course completion rates, college acceptance rates. Avoid vanity metrics. Specify measurement frequency and who analyzes data.

10. **Address risks honestly** — Common school risks: budget cuts mid-year, staff turnover, low student/parent buy-in, technology failures, competing initiatives. For each risk, propose a concrete mitigation (e.g., "If funding is reduced 20%, we'll prioritize grades 3-5 and delay K-2 rollout").

11. **When adapting tone, consider that school boards typically prefer concise, policy-focused language with fiscal responsibility emphasized** — Principals want operational detail. Funding committees need ROI framed as student outcomes per dollar. Parent advisory groups want accessibility and transparency. If you're responsible for tone selection, adjust accordingly.

12. **Format for readability** — Use markdown headings, bullet points, and tables (especially for budgets and timelines). Keep the full brief to 3-6 pages. Provide the executive summary as a separate output so it can be used standalone in emails or slides.

13. **Review the brief to ensure it addresses how the initiative serves diverse learners** — Check that it covers English language learners, students with disabilities, and socioeconomically disadvantaged populations. This is often a board requirement and a moral imperative.

14. **Offer next steps** — End with a clear call to action: "Seeking board approval at the March meeting" or "Request $X allocation in next fiscal year budget" or "Pilot launch August 2024, full rollout January 2025."

## Failure modes

- Initiative description is too vague to construct meaningful objectives
- Target audience is unclear, making tone and detail level ambiguous
- Missing critical data like budget estimates or affected student count
- Context mismatch between K-12 and higher education expectations

When encountering these failure modes, pause to ask clarifying questions before generating the brief. If the user cannot provide details, state your assumptions explicitly in the document (e.g., "This brief assumes a $50,000 budget based on similar district initiatives").