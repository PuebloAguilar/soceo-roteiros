---
name: soceo-roteiros-anuncios
description: Use quando o usuario pedir anuncios, ads, copy de trafego pago, Meta Ads, Facebook Ads, Instagram Ads, TikTok Ads, YouTube Ads, Google Ads, criativos, headlines, primary text, VSL ads, roteiro publicitario, testes de hook, oferta, objecoes ou CTA.
---

# SOCEO Roteiros Anuncios

## Objetivo

Criar anúncios e roteiros publicitários com hipótese clara de teste, ângulo, promessa, prova, objeção e CTA. A skill deve funcionar sem consultar o agente original; os trechos usados estão copiados em `references/trechos-agente.md`.

## Sub-skill obrigatória

Usar `$humanizer` como revisão final de toda copy, roteiro de vídeo, headline, descrição e CTA. Primeiro criar variações com a matriz SOCEO, depois aplicar a passada de humanização para remover sinais de IA: promessas infladas, frases corporativas vazias, excesso de negrito, conclusões genéricas, travessões, ritmo artificial e linguagem publicitária sem prova.

O resultado final deve continuar direto e vendedor, mas com cara de anúncio escrito por operador, não por chatbot.

## Fluxo

1. Identificar plataforma e formato: Meta, TikTok, YouTube Ads, Google, criativo em vídeo, criativo estático, VSL ad ou copy textual.
2. Se faltarem dados, perguntar:
   - público;
   - oferta;
   - prova disponível;
   - estágio de consciência;
   - plataforma;
   - objetivo da campanha.
3. Ler `references/trechos-agente.md`.
4. Criar variações por hipótese, não só "opções bonitas".
5. Separar cada anúncio por: hook, ângulo, promessa, prova, objeção atacada e métrica principal.
6. Revisar com `$humanizer` antes da versão final.

## Saída Padrão

Para cada variação:

- Hipótese do teste.
- Público/estágio de consciência.
- Ângulo.
- Sentimento dominante.
- Hook.
- Primary text ou roteiro de vídeo.
- Headline.
- Descrição curta.
- CTA.
- Prova usada.
- Objeção atacada.
- Métrica principal.

Gerar 3 a 5 variações quando o usuário não definir quantidade.

## Regras

- Não inventar prova, depoimento, número, garantia, escassez ou urgência.
- Não vender promessa agressiva se a entrega não sustenta.
- Para tráfego frio, priorizar problema, mecanismo e prova antes da oferta.
- Para remarketing, priorizar objeção, prova social, urgência real e CTA.
- Para YouTube Ads/VSL Ads, entregar roteiro em blocos com primeiros 5 segundos fortes.
- Não usar travessões no texto final; substituir por ponto, vírgula, dois-pontos ou frase nova.

## Diagnóstico

Se o usuário trouxer métricas, diagnosticar por gargalo:

- CTR baixo: hook/criativo/ângulo.
- Cliques bons e conversão ruim: página, oferta ou prova.
- Leads baratos e vendas baixas: qualidade do público ou qualificação.
- CPM alto: público, criativo saturado ou plataforma.
- Comentários/DMs fortes e vendas baixas: abordagem de fechamento.
