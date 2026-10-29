# Portugal Business Skills

Agent Skills em português para quem empreende, trabalha por conta própria ou abre negócio em Portugal — com foco em brasileiros e outros estrangeiros já residentes.

## Porque existe

Quase todas as skills públicas são em inglês e para o mercado americano. Quem procura "abrir actividade nas Finanças" ou "recibos verdes para brasileiro" não encontra nada. Este repositório preenche esse vazio, com números ancorados nas fontes oficiais e a data da última verificação.

## Skills disponíveis

| Skill | Para quê |
|---|---|
| [`abrir-atividade-financas`](skills/abrir-atividade-financas/SKILL.md) | Abrir atividade como trabalhador independente nas Finanças, escolher CIRS/CAE, IVA, Segurança Social, obrigações do primeiro ano |

## Como instalar

**Claude Code** — copia a pasta da skill para `~/.claude/skills/`:

```bash
git clone https://github.com/SEU-UTILIZADOR/portugal-business-skills.git
cp -r portugal-business-skills/skills/* ~/.claude/skills/
```

**Qualquer agente compatível com Agent Skills** (VS Code, Cursor, ChatGPT, outros) — aponta a pasta `skills/` como diretório de skills. O formato é o padrão aberto doado à Agentic AI Foundation.

## Formato

Cada skill é uma pasta com `SKILL.md`: frontmatter YAML (`name`, `description`) e corpo em Markdown. O `description` é o que o agente lê para decidir se ativa a skill — por isso está em português e com os termos que as pessoas realmente escrevem.

## Princípios deste repositório

- **Números ancorados na fonte**, com link e data de consulta. Sem estimativas apresentadas como factos.
- **Dizer o que não se sabe.** Quando um valor não pôde ser confirmado, a skill diz "confirmar antes de usar" em vez de inventar.
- **Aviso legal explícito** em tudo o que é fiscal: informação operacional, não aconselhamento.

## Contribuir

Correções de valores, links quebrados e atualizações legislativas são bem-vindos. Abre uma issue ou um pull request com a fonte oficial.

## Licença

MIT.
