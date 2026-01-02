<!-- Instruções concisas e específicas para agentes que trabalham neste repositório -->
# Copilot / Agentes — Instruções rápidas

Resumo: repositório pequeno e estático — sem build, sem testes automatizados. Alterações devem ser pequenas, reversíveis e aprovadas pelo mantenedor.

- **Arquivos-chave:** [README.md](README.md), [LICENSE](LICENSE), [Pasta 1/index.html](Pasta%201/index.html), [Pasta 1/teste](Pasta%201/teste)
- **Objetivo do agente:** propor e aplicar mudanças simples (docs, pequenos ajustes de HTML/markdown), evitar adicionar infra sem permissão.

Como validar localmente:
- Abra [Pasta 1/index.html](Pasta%201/index.html) no navegador para conferir alterações visuais.
- Edite e revise [Pasta 1/teste](Pasta%201/teste) como nota/markdown; valide apenas manualmente.

Regras operacionais específicas:
- Não adicione `package.json`, `requirements.txt`, `Makefile` ou workflows em `.github/workflows` sem perguntar antes.
- Evite introduzir dependências externas ou configurar CI/CD por conta própria.
- Nomes de arquivos/ pastas podem conter espaços e acentos; ao referenciar em links, use a codificação URL quando necessário (ex.: `Pasta%201/index.html`).

Commits e PRs:
- Mensagem de commit curta e com escopo: `docs:`, `fix:`, `chore:`. Ex.: `docs: corrigir texto em README.md`.
- PRs: descreva a mudança, risco, e passos manuais para validação (ex.: "Abrir Pasta 1/index.html e verificar título").

Boas práticas de mudança:
- Prefira editar texto e arquivos estáticos (HTML/MD). Para código novo, explique impacto e peça revisão humana.
- Se propuser criar infra (build/test/CI), inclua justificativa curta e alternativa sem infra.

Exemplos rápidos:
- Ajuste no README: faça commit `docs: melhorar README` e adicione instrução de validação.
- Pequena correção de HTML: `fix: ajustar título em Pasta 1/index.html` com indicação do arquivo linkado.

Pergunte se incerto: se a mudança tocar arquitetura, dependências ou automação, peça confirmação explícita ao mantenedor antes de aplicar.

Fim.
