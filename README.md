# agent-social-maneger

> Skill operacional para o Zeus gerenciar redes sociais, conteudo, comunidade, metricas e Ads com limites de seguranca.

## O que faz

- Planeja e cria posts, reels, shorts, carrosseis, roteiros, thumbnails e calendarios editoriais.
- Orienta conexao de contas sociais via OAuth, tokens em cofre, conectores autorizados ou webhooks.
- Responde e modera comentarios e DMs dentro de limites de permissao.
- Analisa metricas e gera relatorios objetivos de conteudo, comunidade e campanhas.
- Planeja, cria, pausa, otimiza e relata campanhas de Meta Ads, Google Ads, YouTube Ads e TikTok Ads quando autorizado.

## Pre-requisitos

| Requisito | Como configurar |
|-----------|-----------------|
| Contas sociais | Conectar pelo dashboard QuickClaw ou conector autorizado da plataforma. |
| Tokens/API keys opcionais | Salvar em Chaves e Segredos no dashboard; nunca commitar segredo no repo. |
| Permissao de publicacao/Ads | Definir manifesto de autonomia com contas, limites, orcamento e aprovacoes. |

A skill tambem funciona em modo rascunho sem credenciais, entregando planos, payloads e conteudos para revisao.

## Exemplos de Uso

### Exemplo 1: Calendario editorial
**Usuario:** "Zeus, cria um calendario de posts para o Instagram da semana."
**Bot:** entrega calendario em modo rascunho, respeitando marca, publico, tom e limites informados.

### Exemplo 2: Conexao de conta
**Usuario:** "Conecta minha conta do TikTok e deixa pronto para publicar."
**Bot:** inicia wizard assistido, pergunta uma coisa por vez, valida credenciais no ambiente e nao publica sem permissao explicita.

## Estrutura

```text
agent-social-maneger/
|-- SKILL.md
|-- skill.json
|-- README.md
|-- LICENSE
|-- RELEASE_NOTES.md
|-- agents/
|   `-- openai.yaml
`-- resources/
    |-- ads-management.md
    |-- autonomy-safety.md
    |-- community-management.md
    |-- connection-wizard.md
    |-- content-production.md
    |-- integrations.md
    |-- metrics-reporting.md
    `-- simple-auth.md
```

## Instalacao

Instalada automaticamente via plataforma QuickClaw apos publicacao da release.

Para instalacao manual em OpenClaw:

```bash
openclaw skills install agent-social-maneger
```

## Changelog

| Versao | Data | Mudanca |
|--------|------|---------|
| 1.0.0 | 2026-05-26 | Release inicial da skill social do Zeus. |

## Licenca

Proprietary - uso restrito ao platform QuickClaw. Ver LICENSE.
