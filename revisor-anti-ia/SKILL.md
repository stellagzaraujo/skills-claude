---
name: revisor-anti-ia
description: Revisa textos para remover características de linguagem de IA com base em um conjunto de regras de escrita. Use este skill SEMPRE que o usuário disser "revise esse texto com as regras de escrita anti IA", "tira o tom de IA", "revisa com as regras de escrita", "aplica as regras de escrita", "revisa esse texto anti IA", "audita esse texto" ou qualquer variação que indique revisão de texto contra padrões de linguagem de IA. Ative também quando o usuário trouxer um texto produzido por IA e pedir para humanizá-lo, torná-lo mais natural, ou remover o tom artificial.
---

# Revisor anti-IA

## Antes de começar

Leia `references/regras_de_escrita.md` na íntegra antes de revisar qualquer texto. Esse documento é a única fonte de verdade para as regras. Não use o que você sabe sobre boas práticas de escrita — use o que está nele.

---

## Fluxo de trabalho

Este skill funciona em duas fases. Nunca pule para a Fase 2 sem confirmação explícita do usuário.

### Fase 1: Diagnóstico

Analise o texto sistematicamente contra as regras do documento de referência.

Para cada problema encontrado, use este formato exato:

**Problema [N] — [nome curto da categoria]**
Trecho: "[trecho exato do texto original, entre aspas]"
Regra: [seção e nome da regra violada]
Correção: [como corrigir, com exemplo reescrito quando necessário]

Categorias a verificar nesta ordem:
1. Vocabulário proibido (seção 4A)
2. Estruturas de frases proibidas — verbos inflados (seção 4B)
3. Aberturas e frases mortas (seção 4C)
4. Transições mortas (seção 4D)
5. Isca de engajamento (seção 4E)
6. Linguagem de hype (seção 4F)
7. Paralelismo negativo e reframing (seção 5 completa)
8. Metáforas proibidas — estruturais, funcionais, famílias, verbos metafóricos (seção 6)
9. Padrões de IA: regra dos três, alcances falsos, variação elegante, metacomentário, falsa profundidade, ritmo de metrônomo, inflação de importância (seção 8)
10. Especificidade baixa — afirmações vagas que poderiam ser concretas (seção 7)

Se o texto não tiver problemas em uma categoria, não mencione a categoria.

Se o texto estiver limpo em todas as categorias, diga isso diretamente e não gere a Fase 2 sem que o usuário peça.

Ao final do diagnóstico, pergunte:
"Confirma as correções? Posso reescrever o texto completo."

---

### Fase 2: Reescrita

Execute somente após confirmação explícita do usuário.

Reescreva o texto completo aplicando todas as correções listadas no diagnóstico. Siga as regras de voz (seção 1), formatação (seção 3) e o guia anti-excesso de ajuste (seção 9) durante a reescrita.

Entregue apenas o texto reescrito. Sem comentários antes ou depois.

---

## Princípios de julgamento

- Aplique as regras com discernimento. O espírito acima da letra.
- Quando uma palavra proibida for a palavra exata e não houver substituto mais limpo, anote o problema mas não force uma piora no texto.
- Não transforme o diagnóstico em uma lista exaustiva de microdetalhes. Priorize os problemas que mais prejudicam a naturalidade do texto.
- Se uma violação for borderline, mencione mas marque como opcional na correção.
