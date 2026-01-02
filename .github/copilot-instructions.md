<!-- Arquivo gerado pelo assistente. Ajuste conforme necessário. -->
# Copilot / Agentes: Diretrizes rápidas

Objetivo: permitir que agentes de código contribuam de forma segura e produtiva neste repositório pequeno e experimental.

- **Contexto do projeto:** Este repositório é um repositório inicial/experimentação (veja [README.md](README.md)). Não existem scripts de build, testes ou dependências declaradas no repositório raiz.
- **Arquivo-chave:** a licença do projeto está em [LICENSE](LICENSE).

Regras operacionais:

1. Priorize mudanças pequenas e reversíveis. Este projeto não tem infraestrutura automatizada — evite adicionar dependências, CI/CD ou frameworks sem confirmação explícita do mantenedor.
2. Antes de criar novos arquivos que introduzam build/tooling (por exemplo `package.json`, `requirements.txt`, `Makefile`, `.github/workflows/*`), pergunte ao mantenedor se deseja esse caminho.
3. Procure por artefatos existentes antes de duplicar funcionalidade: verifique a raiz do repositório por `package.json`, `pyproject.toml`, `requirements.txt`, `Makefile` e diretórios como `src/` ou `docs/`. Se não existirem, documente a sugestão ao propor a mudança.

Padrões de contribuição (específicos para este repositório):

- Mensagens de commit: curtas e descritivas. Ex.: `docs: atualizar README` ou `chore: adicionar copilot-instructions.md`.
- Mudanças de documentação: atualize `README.md` quando fizer mudanças visíveis ao usuário final.

Exemplos práticos (o que fazer / o que evitar):

- Fazer: corrigir texto em [README.md](README.md) para melhorar clareza do propósito do repositório.
- Fazer: adicionar um arquivo README mais detalhado ou exemplos mínimos se o usuário pedir.
- Evitar: adicionar um projeto Node/Python inteiro sem instruções do usuário.

Investigações que o agente deve executar automaticamente:

- Listar arquivos na raiz e procurar por sinais de linguagem/plataforma (ex.: `package.json`, `pyproject.toml`, `setup.py`, `requirements.txt`, `Cargo.toml`). Se encontrados, preferir usar o fluxo nativo dessa linguagem.
- Se o repositório estiver vazio de infra, sugerir opções antes de implementar (ex.: "Deseja que eu adicione um `package.json` para gerenciar dependências?").

Comportamento ao propor mudanças maiores:

- Sempre abrir um PR/patch com descrição curta que explique o porquê e os riscos.
- Incluir instruções de como validar manualmente as alterações (comandos, arquivos a inspecionar).

Checklist rápido para o agente antes de criar um PR:

- [ ] Confirme que não há ferramenta de build detectada; se houver, documente e siga o fluxo.
- [ ] Mantenha mudanças mínimas e focadas (uma responsabilidade por PR).
- [ ] Atualize `README.md` se a experiência do usuário mudar.

Pergunte ao mantenedor quando em dúvida — este repositório é pequeno e as preferências do autor devem guiar decisões de arquitetura.

Fim.
