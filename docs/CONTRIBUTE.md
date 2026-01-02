# Guia de Contribuição (para mim)

## Git Workflow

### Commits
Formato: `tipo: descrição curta`

Tipos:
- `feat:` Nova funcionalidade
- `fix:` correção de bug
- `docs:`Documentação
- `refactor:`Refatoração do código
- `test:` Adicionar testes
- `chore:` Manutenção/config

Exemplos:
- `feat: add user registration endpoint`
- `fix: resolve login validation bug`
- `docs: update README with setup instuctions`

### Branches (para features grandes)
- `main`- código estável
- `dev`- desenvolvimento ativo
- `feature/nome-da_feature`- feature específica

## Code Style (definir conforme stack)

### Nomes
- Ficheiros: `kebab-case.js`
- Variaveis: `camelCase`
- Constantes: `UPPER_SNAKE_CASE`

### Comentários
- Comentar código complexo
- Não comentar o óbvio
- Ingles para código, português para docs do projeto

## Testing Checklist

Antes de fazer commit:
- [ ] Código funciona sem erros
- [ ] Testei Manualmente
- [ ] Comentei partes complexas
- [ ] Atualizei documentação se necessário

## Issue Management

- Fechar issue quando completamente terminada
- Usar closing keywords nos commits: `closes #X`, `fixes #X`
- Atualizar status no project board
