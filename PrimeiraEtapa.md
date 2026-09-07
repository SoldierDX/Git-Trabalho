# Documentação: Primeira Etapa do Projeto

Este documento detalha o planejamento, os requisitos e a execução da **Primeira Etapa** do trabalho de versionamento e colaboração em equipe utilizando Git e GitHub.

---

## 1. Objetivo da Etapa

A primeira etapa teve como foco principal estabelecer o ambiente compartilhado de desenvolvimento, configurar as permissões de acesso da equipe e exercitar o fluxo básico de contribuição colaborativa distribuída (clone, commit, push e verificação de integridade do histórico).

---

## 2. Requisitos e Procedimentos Realizados

Abaixo estão descritas as ações executadas com base nos requisitos definidos para a etapa:

### 1. Criação do Repositório e Gestão de Colaboradores
- **Ação**: O repositório central (`Git-Trabalho`) foi criado na plataforma GitHub.
- **Configuração de Acesso**: Os demais integrantes do grupo foram adicionados formalmente como colaboradores do projeto através das configurações do repositório (`Settings` $\rightarrow$ `Collaborators`), garantindo permissões de escrita para envio direto de alterações.

### 2. Clonagem do Repositório Localmente
- **Ação**: Cada membro da equipe realizou o clone do repositório remoto para sua máquina local, estabelecendo a conexão padrão com o servidor (`origin`):
  ```bash
  git clone https://github.com/SoldierDX/Git-Trabalho.git
  cd Git-Trabalho
  ```

### 3. Contribuições Individuais e Commits Claros
- **Ação**: Cada integrante realizou suas contribuições individuais diretamente no repositório, garantindo no mínimo 2 commits próprios por pessoa.
- **Padrão de Mensagens**: Os commits foram estruturados com mensagens descritivas e objetivas, documentando exatamente o que foi adicionado ou modificado em cada etapa do fluxo de trabalho.

### 4. Meta Global de Commits
- **Ação**: O repositório atingiu e superou a meta mínima estabelecida de **6 commits no total** somando a participação conjunta de todos os membros do grupo.

### 5. Documentação do Repositório (README.md)
- **Ação**: Foi incluído o arquivo base `README.md` na raiz do projeto, estruturando a apresentação do projeto, os temas de estudo abordados (Git, GitHub, controle de branches e colaboração) e a contextualização para qualquer visitante do repositório.

### 6. Sincronização com o Repositório Remoto (Push)
- **Ação**: Todas as alterações locais foram devidamente preparadas (`git add`), consolidadas (`git commit`) e enviadas ao GitHub por meio do comando:
  ```bash
  git push origin main
  ```
  Isso garantiu que todo o progresso ficasse disponível na nuvem antes do prazo final de entrega.

### 7. Auditoria e Validação do Histórico de Contribuições
- **Ação**: Foi realizada a conferência do histórico completo de commits utilizando o comando de visualização de log:
  ```bash
  git log --graph --pretty=format:"%h - %an, %ar : %s"
  ```
  Dessa forma, validou-se que as contribuições de todos os integrantes constam no histórico de versionamento com seus respectivos autores e identificadores.

---

## 3. Fluxo de Trabalho Resumido dos Comandos Utilizados

```text
[Repositório GitHub]
         │
         │  git clone
         ▼
[Repositório Local] ──▶ git add . ──▶ git commit -m "..." ──▶ git push origin
         ▲                                                           │
         └─────────────────── (Sincronizado via GitHub) ─────────────┘
```

---

## 4. Conclusão da Primeira Etapa

Com a conclusão destes 7 passos, a equipe estabeleceu a base necessária de colaboração no Git e GitHub:
- Ambiente de trabalho integrado e permissões validadas;
- Histórico de commits consistente e distribuído entre os colaboradores;
- Repositório documentado e pronto para os desdobramentos das etapas seguintes (como estratégias avançadas de ramificações e merges).
