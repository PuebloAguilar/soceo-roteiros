# SOCEO Roteiros

Pack publico de skills de copywriting para roteiros e anuncios, extraido de um agente-base de vendas e adaptado para uso em Codex/Claude.

## Skills

- `soceo-roteiros-youtube`: roteiros de YouTube, videos longos e VSLs com angulo, promessa, prova, retencao e CTA.
- `soceo-roteiros-reels`: roteiros de Reels com plano, gancho, cenas executaveis, palavras de poder, CTA de DM e diagnostico de metricas.
- `soceo-roteiros-anuncios`: anuncios e roteiros publicitarios para Meta, TikTok, YouTube Ads, Google Ads, VSL ads, criativos, headlines e testes de hook.
- `humanizer`: revisao final para remover sinais de texto gerado por IA e deixar a copy mais natural.

## Estrutura

```text
skills/
  soceo-roteiros-youtube/
    SKILL.md
    agents/openai.yaml
    references/trechos-agente.md
  soceo-roteiros-reels/
    SKILL.md
    agents/openai.yaml
    references/trechos-agente.md
  soceo-roteiros-anuncios/
    SKILL.md
    agents/openai.yaml
    references/trechos-agente.md
  humanizer/
    SKILL.md
    LICENSE
```

Cada skill e auto-contida. Os trechos operacionais usados do agente-base foram copiados para `references/trechos-agente.md`, entao as skills nao dependem do arquivo original.

## Humanizer

As tres skills SOCEO chamam `$humanizer` como revisao final para remover sinais de texto gerado por IA, como introducoes genericas, promessas infladas, excesso de negrito, travessoes, conclusoes artificiais e ritmo robotico.

O pacote ja inclui `skills/humanizer`. A skill original usa licenca MIT, preservada em `skills/humanizer/LICENSE`.

## Instalacao local

Copie ou crie symlinks das pastas dentro de `skills/` para o diretorio de skills do seu runtime:

```bash
ln -s "$PWD/skills/soceo-roteiros-youtube" ~/.codex/skills/soceo-roteiros-youtube
ln -s "$PWD/skills/soceo-roteiros-reels" ~/.codex/skills/soceo-roteiros-reels
ln -s "$PWD/skills/soceo-roteiros-anuncios" ~/.codex/skills/soceo-roteiros-anuncios
ln -s "$PWD/skills/humanizer" ~/.codex/skills/humanizer
```

Para Claude, use `~/.claude/skills/` no destino.

## Observacoes

- Este repo nao inclui o prompt completo do agente-base.
- Foram mantidos apenas trechos de copy, estrutura, angulos, palavras de poder, oferta, diagnostico e humanizacao.
- Nao foram incluidos blocos internos de protecao, guardrails privados ou persona abusiva.
