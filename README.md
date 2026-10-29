# Portugal Business Skills

Agent Skills em português para quem empreende, trabalha por conta própria ou abre negócio em Portugal — com foco em brasileiros e outros estrangeiros já residentes.

## Porque existe

Quase todas as skills públicas são em inglês e escritas para o mercado americano. Quem procura "abrir atividade nas Finanças", "recibos verdes para brasileiro" ou "que anexo do IRS" não encontra nada. Este repositório preenche esse vazio, com números ancorados nas fontes oficiais e a data da última verificação.

## Skills disponíveis

| Skill | Para quê |
|---|---|
| [`nif-niss-numero-utente`](skills/nif-niss-numero-utente/SKILL.md) | Obter NIF, NISS e número de utente do SNS sendo estrangeiro — documentos, onde pedir, atalho dos 12 Espaços Cidadão |
| [`abrir-atividade-financas`](skills/abrir-atividade-financas/SKILL.md) | Abrir atividade como trabalhador independente: CIRS vs CAE, ato isolado, IVA art. 53.º, obrigações do primeiro ano |
| [`seguranca-social-direta`](skills/seguranca-social-direta/SKILL.md) | Senha do portal, declaração trimestral, contribuições, carreira contributiva, subsídios e baixas |
| [`irs-primeira-declaracao`](skills/irs-primeira-declaracao/SKILL.md) | Residência fiscal, prazos, qual anexo, deduções, reembolso, rendimentos no Brasil e dupla tributação |
| [`arrendamento-senhorio-recibos`](skills/arrendamento-senhorio-recibos/SKILL.md) | Senhorio: registar contrato (Modelo 2), recibo de renda eletrónico, atualização anual, IRS categoria F, incumprimento |

## Ordem natural de uso

Quem chega a Portugal passa por estas skills nesta sequência:

```
nif-niss-numero-utente  →  abrir-atividade-financas  →  seguranca-social-direta
                                    ↓
                          irs-primeira-declaracao
```

## Como instalar

**Claude Code** — copia as pastas para `~/.claude/skills/`:

```bash
git clone https://github.com/rubensbmelo/portugal-business-skills.git
cp -r portugal-business-skills/skills/* ~/.claude/skills/
```

**Qualquer agente compatível com Agent Skills** (VS Code, Cursor, ChatGPT, outros) — aponta a pasta `skills/` como diretório de skills. O formato é o padrão aberto doado à Agentic AI Foundation (Linux Foundation).

## Formato

Cada skill é uma pasta com `SKILL.md`: frontmatter YAML (`name`, `description`) e corpo em Markdown. O `description` é o que o agente lê para decidir se ativa a skill — por isso está em português, com os termos que as pessoas realmente escrevem.

## Princípios deste repositório

- **Números ancorados na fonte**, com link e data de consulta. Sem estimativas apresentadas como factos.
- **Dizer o que não se sabe.** Quando um valor não pôde ser confirmado, a skill diz "confirmar antes de usar" em vez de inventar um número.
- **Aviso legal explícito** em tudo o que é fiscal: informação operacional, não aconselhamento.
- **Erros comuns no fim**, porque é aí que está o dinheiro que se perde.

## Contribuir

Correções de valores, links quebrados e atualizações legislativas são bem-vindos. Abre uma issue ou um pull request com a fonte oficial.

## Licença

MIT.
