## v1.0.0 - 2026-05-26

> Bump: MAJOR
> Compatibilidade: release inicial

### Added
- Skill `agent-social-maneger` para operacao assistida de redes sociais, conteudo, comunidade, metricas e Ads do Zeus.
- Referencias operacionais para conexao de contas, autenticacao simples, integracoes, producao de conteudo, comunidade, Ads, metricas e seguranca.
- Manifesto `skill.json`, README, LICENSE e workflow de release no padrao QuickClaw.

### Security
- Credenciais devem ser lidas de ambiente, conectores autorizados ou Chaves e Segredos do dashboard; nenhum segredo deve ser salvo no git.

### Migration Notes
- Nao aplicavel para release inicial.

### Validation
- [x] SKILL.md frontmatter validado (name, description)
- [x] skill.json.version atualizado e bate com a tag planejada
- [x] Sem scripts runtime para compilar nesta release
- [x] Sem secrets, sem `.env`, sem artefatos de runtime versionados
- [ ] CI da org passou (aguardar GitHub Actions apos tag)
- [x] README/SKILL.md sem paths absolutos do host

### Rollback
- Tag anterior estavel: nenhuma
- Procedimento: remover a skill do catalogo ou publicar PATCH corretivo
