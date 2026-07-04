---
name: soceo-roteiros-youtube
description: Use quando o usuario pedir roteiro de YouTube, video longo, video horizontal, VSL, abertura, retencao, capitulo, narracao, titulo, descricao, CTA ou estrutura de conteudo longo com copy, angulo, palavras de poder, promessa, prova e oferta.
---

# SOCEO Roteiros YouTube

## Objetivo

Criar roteiros de YouTube com lógica de retenção, autoridade e venda. A skill deve funcionar sem consultar o agente original: os trechos necessários do agente-base estão em `references/trechos-agente.md`.

## Sub-skill obrigatória

Usar `$humanizer` como revisão final de todo roteiro, título, descrição e CTA. Primeiro criar a peça com a matriz SOCEO, depois aplicar a passada de humanização para remover sinais de IA: introduções genéricas, conclusões artificiais, excesso de negrito, ritmo teatral repetitivo, travessões, frases infladas e fórmulas vazias.

O resultado final deve continuar persuasivo, mas soar como um criador real falando. Preservar tensão, promessa, prova e CTA.

## Fluxo

1. Identificar o objetivo do vídeo: autoridade, venda, leads, VSL, lançamento, educação, prova, história ou tráfego para oferta.
2. Se faltarem dados, perguntar em bloco curto:
   - público;
   - produto/serviço;
   - promessa do vídeo;
   - prova disponível;
   - CTA;
   - duração desejada.
3. Ler `references/trechos-agente.md`.
4. Escolher um ângulo e um sentimento dominante.
5. Montar o roteiro em blocos de retenção, não em texto corrido sem função.
6. Revisar com `$humanizer` antes de entregar.

## Saída Padrão

Entregar:

- 3 opções de título.
- Promessa central do vídeo.
- Ângulo escolhido.
- Sentimento dominante.
- Estrutura por blocos com tempo estimado.
- Roteiro completo de narração.
- Indicações visuais simples e executáveis.
- CTA final.
- Métricas para revisar depois: retenção média, queda nos primeiros 30s, CTR, comentários, cliques, leads e vendas.

## Estrutura Recomendada

1. Hook forte: tese, erro, promessa ou prova.
2. Sintoma: o que o público sente ou percebe.
3. Causa: o mecanismo invisível por trás do problema.
4. Risco: custo de continuar igual.
5. Autoridade: por que ouvir agora.
6. Processo: método, passos ou framework.
7. Prova: caso, demonstração, dado, print ou raciocínio verificável.
8. Objeções: quebrar as 2-3 principais.
9. Oferta/ponte: por que o próximo passo é lógico.
10. CTA: ação clara, canal claro e motivo para agir agora.

## Regras

- Não inventar números, provas, resultados, escassez ou autoridade.
- Usar tom direto e executivo; atacar o problema, não humilhar a pessoa.
- Quando o usuário pedir YouTube Shorts, confirmar se ele quer roteiro vertical curto; se for curto, usar preferencialmente `$soceo-roteiros-reels`.
- Para VSL, reforçar promessa, prova, mecanismo, objeção, oferta e CTA.
- Para vídeo educativo, manter a tensão de venda sem transformar tudo em propaganda.
- Não usar travessões no texto final; substituir por ponto, vírgula, dois-pontos ou frase nova.

## Erros Comuns

- Começar com introdução genérica.
- Entregar tópicos em vez de roteiro narrado.
- Colocar CTA antes de provar a tese.
- Misturar vários ângulos e perder retenção.
- Fazer roteiro de YouTube com ritmo de Reels.
