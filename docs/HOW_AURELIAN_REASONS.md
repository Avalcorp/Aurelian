# HOW AURELIAN REASONS

**Status:** hipótese de ciclo de raciocínio
**Relação:** operacionaliza as capacidades propostas em `H-AUR-MIN-01_O_QUE.md`.

## Ciclo proposto

```text
ARTEFATO
   ↓
INTERPRETAÇÃO
   ↓
RECONSTRUÇÃO
   ↓
REPRESENTAÇÃO
   ↓
CONTEXTUALIZAÇÃO
   ↓
AVALIAÇÃO
   ↓
EXPLORAÇÃO
   ↓
COMPARAÇÃO / TESTE
   ↓
RECOMENDAÇÃO
```

O fluxo é uma orientação analítica, não uma sequência rígida. O raciocínio é iterativo: nova evidência, contradição ou insuficiência pode exigir retorno a etapas anteriores.

```text
evidência insuficiente ou contraditória
             │
             ▼
INTERPRETAÇÃO → RECONSTRUÇÃO → REPRESENTAÇÃO
      ▲                              │
      └──────────────────────────────┘
```

## 1. Artefato

O ciclo começa com um insumo e sua proveniência: origem, versão, data, responsável, escopo, finalidade declarada e eventuais relações com outros materiais. Aurelian não presume que o artefato descreva a realidade completa.

## 2. Interpretação

Nesta etapa, Aurelian extrai alegações, conceitos, participantes, ações, decisões, regras e qualificadores. Também classifica o material: evidência observada, relato, norma, hipótese, recomendação ou decisão. A interpretação deve conservar trechos ou referências que permitam verificar por que uma afirmação foi extraída.

Perguntas de controle:

- O que este material efetivamente sustenta?
- O que ele apenas sugere?
- A que contexto e tempo ele se aplica?
- Há ambiguidade, omissão ou conflito interno?

## 3. Reconstrução

Aurelian reúne fragmentos interpretados em uma hipótese sobre o cenário. Reconstruir inclui identificar objeto de transformação, fluxo de trabalho, intervenientes, decisões, dependências, exceções e consequências.

Toda relação reconstruída deve distinguir observação direta de inferência. Lacunas não são preenchidas silenciosamente: tornam-se questões ou necessidades de evidência.

## 4. Representação

O cenário é tornado analisável como uma rede de elementos e relações. A representação deve conseguir responder, por exemplo:

- quem executa, decide, supervisiona e responde;
- quais atividades produzem quais resultados;
- de que capacidades, dados e sistemas dependem;
- quais regras, restrições e autoridades limitam a ação;
- quais evidências sustentam cada ligação.

## 5. Contextualização

O mesmo padrão de atividade tem significados diferentes conforme domínio, risco, objetivo, maturidade operacional, horizonte temporal e exigência de controle. Contextualizar impede que a análise reduza o cenário a uma lista de tarefas isoladas.

## 6. Avaliação

Aurelian avalia suficiência, consistência e relevância da representação antes de recomendar qualquer transformação. Avalia também as implicações de alternativas possíveis: benefício esperado, riscos, reversibilidade, impacto sobre autoridade, necessidade de supervisão e qualidade de evidência.

Uma avaliação pode concluir `INSUFICIENTE PARA RECOMENDAR`. Essa conclusão é governada e informativa.

## 7. Exploração

Explorar é gerar alternativas condicionais sem antecipar uma resposta única. Exemplos: manter execução humana, fornecer apoio inteligente, delegar subatividade a agente, usar agente sob aprovação, ou compor fluxo híbrido.

Cada alternativa deve indicar o que muda, que capacidades exige, qual autoridade preserva ou desloca e quais condições precisam ser verdadeiras para ser plausível.

## 8. Comparação e teste

As alternativas são confrontadas com evidências, restrições e critérios comuns. Testar, neste estágio, pode significar verificar coerência com o cenário representado, procurar contraexemplos, comparar impactos ou definir experimento posterior. Não significa declarar validade sem evidência.

## 9. Recomendação

A saída deve conter:

- recorte do cenário analisado;
- recomendação ou alternativas ordenadas;
- racional e evidências de suporte;
- incertezas, pressupostos e evidências contrárias;
- restrições, riscos e controles necessários;
- decisão ou validação humana requerida;
- próximos passos de verificação.

## Estados de conhecimento

Para preservar governança, os registros do ciclo devem usar categorias explícitas:

| Estado | Significado |
| --- | --- |
| Evidência | informação ancorada em artefato rastreável |
| Inferência | conclusão derivada de evidências, sujeita a revisão |
| Hipótese | explicação ou possibilidade ainda não validada |
| Lacuna | informação necessária e ainda indisponível |
| Recomendação | avaliação proposta por Aurelian |
| Decisão | deliberação humana registrada fora de Aurelian |

## Resultado esperado da experimentação

O ciclo será considerado produtivo se seus retornos revelarem onde ele precisa mudar: uma etapa ausente, uma fronteira artificial entre etapas, um critério insuficiente ou uma representação que não suporta o raciocínio necessário.
