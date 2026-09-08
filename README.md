<p align="center">
  <img src="https://github.com/Avalcorp/Aurelian/blob/main/Aurelian.png" alt="Ícone" width="120" style="vertical-align: middle;">
  <span style="font-size: 32px; font-weight: bold; margin-left: 10px;">Aurelian</span>
</p>
 

## Purpose

Aurelian is the research artifact being developed within **Artigo CNEG: AIM — Modelo de Agentificação**.

Its purpose is to evolve as an experimental and analytical instrument for the research, rather than as a frozen architecture.

The research seeks to:

> **Modelar as melhores práticas para, diante do cenário organizacional e tecnológico posto, estabelecer uma agentificação — isto é, uma alocação de IA agêntica — nos processos e departamentos de uma determinada corporação produtiva.**

Aurelian is expected to be both:

- an **object of experimentation**, exercised with the states, artifacts and evidence produced by the research; and
- an **instrument for observing and validating the evolution of the research itself**.

A guiding question is:

> **“O que este artefato, ao ser analisado por Aurelian, nos revela sobre nossa investigação de como agentificar processos e departamentos de uma corporação produtiva?”**

## Governance principle

> **Aurelian produces RECOMMENDATION; Aurelian does NOT make DECISIONS.**

Aurelian may observe, represent, compare, test, identify impacts, evidence inconsistencies and produce recommendations.

Its recommendation is a parameter/evidence for the human governance process. It never replaces the human decision.

```text
AURELIAN
   │
   ▼
RECOMMENDATION
   │
   ▼
HITL HUMAN
   │
   ▼
DECISION
```

## Relationship with the Research Schedule

The **Research Schedule (Cronograma da Pesquisa)** is the primary temporal reference.

The **Rolling Aurelian** is subordinate to it. It is not a parallel research schedule.

```text
RESEARCH SCHEDULE
       │
       │ movement
       ▼
ROLLING AURELIAN
       │
       ├── Aurelian current state
       ├── exercise
       ├── test
       ├── evidence
       ├── impact / reflection
       ├── recommendation
       ├── HITL / human decision
       └── next state
```

This makes Aurelian's evolution observable in synchronization with the evolution of the research.

## Rolling Aurelian v0.1

**Status:** APPROVED — HITL  
**Approval date:** 08/09/2026 — BRT  
**Starting point:** A01 — first approved artifact of Phase 1

The approved Rolling Aurelian begins retrospectively with **A01** and reconstructs the trajectory through **A10**, then synchronizes with the current state of the research.

```text
A01 → A02 → A03 → ... → A10
                         │
                         ▼
              Phase 1 absorption study
                         │
                         ▼
                 Aurelian state
                         │
                         ▼
              Current research state
                         │
                         ▼
                  Phase 2 onward
```

The first operational movement is the reconstruction of **A01–A10**, including relevant supporting artifacts.

## Inputs

The Rolling considers two categories of research material:

### Direct artifacts

Artifacts directly produced and approved by the research.

### Supporting artifacts

Artifacts that preserve or point to complementary information in source documents used to construct the direct artifacts.

Supporting artifacts are part of the exercise and traceability whenever they are necessary to understand, verify or complement the direct artifacts.

## Per-movement observation

For each Phase 1 artifact and, subsequently, each relevant research movement, the Rolling records:

| Element | Purpose |
|---|---|
| Research State | State reached by the research |
| Movement | What changed |
| Artifact / Input | Direct or supporting artifact entering the exercise |
| Aurelian State Before | Previous known Aurelian state |
| Exercise | How the material is confronted with Aurelian |
| Test / Question | What is being verified |
| Evidence | What was actually observed |
| Impact | Positive, negative, mixed, neutral or unknown |
| Reflection on Research | What the exercise reveals about the agentification investigation |
| Aurelian Recommendation | Evaluation/recommendation produced by Aurelian |
| HITL / Human Decision | Governance decision, when applicable |
| Aurelian State After | Resulting state |
| Next Movement | Next research movement and/or enabled exercise |

## Impact and evolution

Aurelian's evolution is evidence-driven.

Initial impact classification:

- `POSITIVE`
- `NEGATIVE`
- `POSITIVE + NEGATIVE`
- `NEUTRAL / NO IMPACT IDENTIFIED`
- `UNKNOWN`

A recommendation to absorb something into the metadata is **not itself an absorption decision**.

Only the human governance process can decide whether an element is absorbed.

## Phase 1 absorption study

After reconstructing A01–A10, the Rolling enters the **Phase 1 absorption study**.

The purpose is to establish what the complete Phase 1 research mass reveals about:

- the model Aurelian needs;
- the metadata Aurelian needs;
- structural gaps;
- semantic gaps;
- inconsistencies;
- possible evolutions;
- implications for the research itself.

This is a discovery activity. It does not assume that Aurelian is complete.

## Wrapper

After the Phase 1 absorption study, and when sufficient evidence/mass exists, the Rolling introduces the experimental construction of the **Wrapper**.

The Wrapper is intended as a complementary element of Aurelian that enables provocative interactions capable of producing new evidence and perspectives for the research.

Its architecture is **not frozen in advance**. Its characteristics and needs should emerge from exercises and tests.

## Research feedback loop

The intended permanent cycle is:

```text
RESEARCH
   ↓
MOVEMENT
   ↓
EXERCISE IN AURELIAN
   ↓
TEST
   ↓
EVIDENCE
   ↓
IMPACT / REFLECTION
   ↓
AURELIAN RECOMMENDATION
   ↓
HITL HUMAN
   ↓
DECISION
   ↓
NEW STATE
   ↓
NEW EXERCISE
   ↓
RESEARCH
```

This creates a bidirectional relationship:

> The research exercises Aurelian, while Aurelian helps make the evolution of the research observable.

## Updates and traceability

Aurelian is **not a frozen architecture**.

Its model and metadata may evolve as evidence emerges.

Research artifacts may also be updated. An update does not erase history. Previous versions, changes, evidence and the rationale for revised conclusions must remain traceable.

A later artifact or updated artifact may therefore change the interpretation of a previous conclusion, but it must not silently erase the historical trajectory.

## Repository role

The repository is a versioned research environment for preserving:

- Aurelian's evolving representation;
- governed artifacts;
- supporting material;
- evidence;
- decisions and their provenance;
- the evolution of the model and metadata;
- the relationship between Aurelian and the Research Schedule.

The repository should not be treated merely as a collection of files.

## Versioning and governance

The currently approved Rolling baseline is **v0.1**, approved through HITL on **08/09/2026 — BRT**.

Any subsequent structural version must use the immediately preceding formally approved version as its reference base.

Structural changes must be explicitly identified, traceable and governed. Silent structural evolution is not permitted.

## Core principles

1. The Research Schedule is the primary temporal reference.
2. Rolling Aurelian is subordinate to the Research Schedule.
3. The Rolling history begins with A01 and reconstructs A01–A10.
4. Direct and relevant supporting artifacts are part of the exercise mass.
5. Aurelian is both an object of experimentation and an instrument for observing and validating research evolution.
6. Aurelian produces recommendations; it does not make governance decisions.
7. Human HITL remains the decision authority.
8. Positive, negative, mixed, neutral and unknown results are valid research outcomes.
9. Metadata evolution is driven by evidence.
10. Artifact updates preserve history and traceability.
11. Aurelian's architecture is not frozen.
12. Structural evolution must not be introduced silently.
