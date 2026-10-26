# Cognalyze
### AI Hiring Committee & Campus Placement Intelligence Platform

**The world doesn't have a talent shortage. It has a talent intelligence problem.**

Cognalyze is an AI-powered talent assessment and campus placement intelligence platform designed to bridge the gap between candidate preparation and enterprise recruitment.

It combines multi-agent candidate evaluation, evidence verification, adaptive interview preparation, coding assessments, and recruiter intelligence to make talent assessment more structured, transparent, and evidence-driven.

Rather than relying solely on resume keywords or a single AI-generated score, Cognalyze aims to connect candidate claims, demonstrated competencies, and role-specific requirements.

---

## The Problem

Traditional hiring and campus placement processes face three fundamental challenges:

- **Resume-Driven Screening:** Candidates can be overlooked because their resumes do not adequately represent their actual capabilities.
- **Limited Assessment Depth:** Conventional assessments may not capture problem-solving ability, technical understanding, communication, or practical experience comprehensively.
- **Disconnected Preparation and Hiring:** Students often prepare using disconnected tools, while recruiters lack a consistent, evidence-grounded view of candidate capabilities.

Cognalyze aims to bridge these gaps through an integrated talent intelligence ecosystem.

## Our Solution

Cognalyze connects candidate preparation, assessment, and recruitment through specialized AI workflows.

The platform is designed to help students develop and demonstrate their skills while giving recruiters structured information to support candidate evaluation.

### Core Capabilities

- **Adversarial AI Hiring Committee:** Multi-agent evaluation that examines candidates from multiple assessment perspectives.
- **Evidence Verification:** Connect candidate claims to available supporting evidence from resumes, GitHub repositories, coding profiles, and interview transcripts.
- **Live AI Mock Interviews:** Conversational technical interviews with role-relevant questions and structured evaluation.
- **Coding and Problem-Solving Assessment:** Evaluate demonstrated problem-solving ability through coding tasks and related evidence.
- **Adaptive Socratic Mentor:** Guide students through conceptual questions and progressive hints rather than relying exclusively on direct answers.
- **Adaptive Skill Development:** Adjust learning difficulty and practice activities based on observed performance.
- **Recruiter Intelligence:** Support role-specific candidate discovery, evidence-grounded questions, and structured evaluation.
- **Blind Screening and Decision Auditing:** Support privacy-conscious screening workflows and traceability of human review and overrides.
- **Career and Community Features:** Connect students with opportunities, hiring posts, collaboration, and career-development activities.

Feature availability depends on the implemented modules and deployment configuration.

---

## Multi-Agent Architecture

Cognalyze is designed around seven major subsystems containing 18 specialized AI agents, with distinct responsibilities and verification contracts.

### 1. Evidence Verification and Anti-Hallucination Pipeline

**Purpose:** Connect candidate claims to supporting evidence and identify unsupported assertions.

Key agents include:

- Pipeline Orchestrator
- Deep Review and Anti-Vibe Coding Agent
- GitHub Evidence Agent
- LeetCode and Problem-Solving Agent
- Hackathon and External Achievement Agent
- Resume Claim Extraction Agent
- Interview Competency Matcher Agent
- Quote Verifier Agent

The pipeline is designed to coordinate evidence collection, map claims to source material, and check whether attributed quotations appear in the original transcript.

### 2. Adaptive Socratic Mentor and Diagnostic Engine

**Purpose:** Help students improve their understanding through guided reasoning and contextual feedback.

Key agents include:

- Intent and Semantic Understanding Agent
- Socratic Interaction Engine Agent
- Knowledge Graph and Prerequisite Agent
- Diagnostic and Evaluator Agent
- Contextual Reference and Memory Agent

The subsystem is designed to identify learning intent, provide progressive hints, track prerequisite relationships, and assess demonstrated conceptual understanding.

### 3. Adaptive Skill Engine

**Purpose:** Personalize preparation and progressively challenge students.

The Adaptive Engine Agent supports the planned workflow of learning, practice, coaching, interviewing, and retesting. It can introduce system-design failure scenarios and adjust difficulty based on performance.

### 4. Recruiter and Decision Intelligence

**Purpose:** Help recruiters evaluate candidates against role-specific requirements with greater transparency.

Key components include:

- Recruiter Intelligence Agent
- Decision and Override Audit Engine

The subsystem supports evidence-grounded candidate queries, privacy-conscious screening workflows, talent rediscovery, and auditable human decisions.

### 5. Candidate Screening and Funnel Engine

**Purpose:** Structure candidate evaluation across recruitment stages.

The Candidate Screening and Dynamic Funnel Agent organizes assessment against role-specific criteria and supports progression through stages such as application, technical assessment, system design, and offer.

### 6. Live Mock Interview and Proctoring

**Purpose:** Provide interactive interview practice and structured assessment.

Key components include:

- Alex — Staff Engineer Interview Persona
- Interview Real-Time Scoring Agent
- AI Text Detection Agent
- Visual Proctoring and Body Language Agent

The interview workflow is designed to generate targeted questions and assess dimensions such as problem-solving, technical depth, communication, system design, edge-case handling, code quality, and behavioral responses.

Automated scoring, AI-generated-text detection, and visual proctoring have limitations and should not be treated as definitive proof of a candidate's ability, integrity, or intent.

### 7. Multi-Provider LLM Router

**Purpose:** Abstract model-provider selection and support fallback behavior.

The architecture includes integrations or configured pathways for:

- Local inference through Ollama
- Llama models served through Groq
- Google Gemini
- OpenAI models

The router is designed to support provider selection and failover when a configured provider is unavailable or rate-limited. Actual model availability and fallback behavior depend on the deployment configuration.

---

## Open-Source AI Approach

Cognalyze uses a multi-agent architecture in which specialized software workflows coordinate AI-assisted tasks.

The broader architecture is designed to support different model providers, including locally hosted and externally served models. This enables flexibility in deployment, cost management, and model selection.

For reproducibility, a deployment should document:

- The exact model and version used by each relevant workflow.
- The applicable model license or provider terms.
- Which tasks rely on open-weight models versus proprietary hosted APIs.
- The verification procedures used to evaluate model outputs.
- The configuration required to reproduce the demonstrated functionality.

**Note:** A multi-agent architecture does not automatically make a project open-source. Open-source status depends on the project's licensing, while model eligibility depends on the specific model and its applicable terms.

---

## Evidence-Driven Assessment

Cognalyze aims to distinguish between a candidate's claims and the evidence available to support them.

For example, a candidate may claim experience building a distributed caching system. An evidence-oriented workflow can examine available repository history, technical explanations, interview responses, and other relevant sources.

The goal is to produce assessments that are easier to inspect and challenge rather than relying on unsupported AI-generated conclusions.

Evidence availability does not guarantee that a claim is true, and missing evidence does not prove that a candidate lacks a skill.

---

## Human Oversight and Responsible AI

Cognalyze is designed to support human decision-making, not replace it.

Key principles include:

- Traceability between assessment claims and source evidence.
- Transparent explanations of evaluation outcomes.
- Human review of consequential hiring decisions.
- Appropriate handling of candidate information.
- Awareness of model uncertainty and potential bias.
- Clear limitations for automated scoring and proctoring.

Recruitment decisions should not rely solely on automated scores, AI-generated-text detectors, or visual behavior analysis.

---

## Technology and Integrations

The architecture includes or is designed to integrate with:

- **Application:** Next.js and React
- **AI Orchestration:** Specialized agents and multi-provider model routing
- **Model Providers:** Ollama, Groq-hosted Llama models, Google Gemini, and OpenAI
- **Evidence Sources:** GitHub, coding profiles, resumes, and interview transcripts

Specific model versions, dependency versions, and configuration details should be documented for the deployment being demonstrated.

---

## Getting Started

Cognalyze is an existing application with multiple subsystems and external integrations.

Setup requirements may vary depending on the modules being used, environment configuration, model providers, and required credentials.

Before running the project, consult the repository's actual dependency manifests, environment configuration, and application entry points.

**Configuration and run commands should be documented after they have been verified against the current source code.**

Never commit API keys, access tokens, private credentials, or real candidate information.

---

## Current Scope and Limitations

Cognalyze contains a broad set of intended capabilities across student preparation, candidate assessment, and recruiter intelligence. Individual features may have different implementation and deployment requirements.

AI-generated assessments can be inaccurate, model providers can fail, and external evidence sources may be incomplete or unavailable. All consequential conclusions require appropriate human review.

---

## Contributing

Contributions to the project can focus on:

- Improving evidence verification and traceability.
- Strengthening agent evaluation and reliability.
- Improving reproducibility across model providers.
- Adding tests for unsupported claims and fabricated quotations.
- Improving accessibility, documentation, and responsible AI safeguards.

Contributions should include relevant tests and documentation.

Do not publish real candidate transcripts, credentials, or personally identifiable information in issues, pull requests, or test fixtures.

---

## License

The applicable license must be specified in the repository's `LICENSE` file and must reflect the permissions held by the project owner or rights holders.

Third-party dependencies and AI models may be subject to separate licenses or terms.

---

## Vision

Cognalyze aims to connect the entire talent intelligence journey:

**Preparation → Assessment → Evidence → Hiring**

By bringing these workflows together, the platform seeks to help students demonstrate their capabilities and help recruiters make more informed, evidence-grounded decisions.


