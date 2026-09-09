# H-AUR-MIN-02 — O QUE E COMO

**Status:** hipótese funcional, operacional e arquitetural inicial
**Base:** evolui H-AUR-MIN-01 sem substituir ou declarar definitiva sua hipótese.
**Finalidade:** oferecer uma arquitetura suficientemente explícita para ser testada, refutada e refinada na Fase 2.

## Formulação de segundo patamar

> Aurelian recebe artefatos heterogêneos, interpreta seu conteúdo e status epistemológico, reconstrói o objeto de transformação e seu cenário, constrói e refina progressivamente uma representação contextual, avalia sua suficiência e consistência, explora e compara alternativas de agentificação, testa sua plausibilidade diante das evidências e restrições disponíveis e produz uma recomendação rastreável para decisão humana. Essas operações são iterativas: evidências, contradições ou lacunas podem levar à revisão de interpretações, reconstruções e representações anteriores.

H-AUR-MIN-02 não afirma que Aurelian já possui tais componentes nem que eles devem ser implementados exatamente como desenhados. Ela propõe uma hipótese arquitetural inicial para experimentação.

## Hipótese de arquitetura inicial

```text
                         AURELIAN
                            │
             ┌──────────────┴──────────────┐
             │                             │
             ▼                             ▼
      INPUT / ARTIFACT              REASONING / CONTROL
             │                             │
             ▼                             │
      INTERPRETATION                       │
             │                             │
             ▼                             │
      SCENARIO RECONSTRUCTION              │
             │                             │
             ▼                             │
      SEMANTIC REPRESENTATION ◄────────────┤
             │                             │
             ▼                             │
      CONTEXT / EVIDENCE                   │
             │                             │
             └──────────────┬──────────────┘
                            ▼
                  SCENARIO REASONER
                            │
             ┌──────────────┼──────────────┐
             ▼              ▼              ▼
         EVALUATOR      EXPLORER       COMPARATOR
             │              │              │
             └──────────────┼──────────────┘
                            ▼
                  AGENTIFICATION
                    RECOMMENDATION
                            │
                            ▼
                       HUMAN / HITL
                            │
                            ▼
                         DECISION
```

## Papéis hipotéticos

| Papel | Responsabilidade proposta | Não deve fazer sozinho |
| --- | --- | --- |
| Input / Artifact | receber, identificar e preservar proveniência | declarar o conteúdo como verdade |
| Interpretation | extrair alegações, conceitos e status epistemológico | decidir a transformação |
| Scenario Reconstruction | compor hipótese de cenário a partir dos fragmentos | ocultar lacunas ou conflitos |
| Semantic Representation | manter elementos, relações, evidências e incertezas | congelar uma ontologia definitiva |
| Context / Evidence | relacionar afirmações a fontes, tempo e condições | substituir análise crítica |
| Reasoning / Control | coordenar o ciclo, retornos e critérios de suficiência | assumir autoridade de governança |
| Scenario Reasoner | analisar o cenário e possibilidades de transformação | escolher uma alternativa sem evidência |
| Evaluator | avaliar coerência, suficiência, risco e adequação | transformar avaliação em decisão |
| Explorer | gerar alternativas condicionais | tratar alternativas como recomendações finais |
| Comparator | comparar alternativas por critérios explícitos | apagar alternativas inconvenientes |
| Recommendation | tornar a avaliação rastreável e acionável para HITL | implantar ou aprovar a mudança |

Os papéis podem se revelar capacidades de um mesmo componente, componentes separados ou uma modelagem inadequada. Essa indefinição é intencional nesta etapa.

## Núcleo de controle e rastreabilidade

O núcleo de raciocínio e controle deve preservar, para cada conclusão relevante:

- artefatos e versões usados;
- interpretações e inferências realizadas;
- evidências que sustentam e que contradizem a conclusão;
- representação do cenário adotada no momento da análise;
- critérios e alternativas avaliados;
- incertezas, lacunas e condições de validade;
- recomendação emitida e decisão humana posterior, se houver.

Esse registro permite que uma atualização posterior reveja uma conclusão sem apagar a trajetória que a produziu.

## Contrato de saída para HITL

A recomendação entregue ao decisor humano deve conter, no mínimo:

1. a pergunta e o recorte do cenário;
2. a representação relevante do cenário e suas limitações;
3. alternativas consideradas;
4. recomendação e nível de confiança justificado;
5. evidências, pressupostos e objeções relevantes;
6. riscos, restrições, controles e limites de autoridade;
7. validações ou experimentos ainda necessários;
8. decisão humana requerida.

## Hipóteses que a Fase 2 deve testar

- interpretação, reconstrução e representação são capacidades separáveis?
- autoridade deve ser modelada como restrição contextual ou como elemento nuclear?
- o avaliador, explorador e comparador são papéis necessários e distintos?
- a representação precisa ser temporal, causal ou orientada a eventos?
- a qualidade da recomendação exige simulação, experimentação ou novas classes de evidência?
- quais limites de automação e supervisão emergem de cenários reais?

## Regra de evolução

Qualquer evolução desta arquitetura deve ser registrada como hipótese, evidência, recomendação e decisão humana quando aplicável. A arquitetura não pode ser alterada silenciosamente para fazer parecer que uma conclusão já era conhecida.
