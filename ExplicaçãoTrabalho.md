# Relatório de Estudo: Git, GitHub e Estratégia de Branches

## 1. Visão Geral do Projeto

Este projeto foi desenvolvido como um trabalho prático de estudo e capacitação sobre o sistema de controle de versão **Git** e a plataforma colaborativa **GitHub**. 

O objetivo central foi vivenciar na prática os fluxos de trabalho reais utilizados no desenvolvimento de software moderno, compreendendo como gerenciar alterações, colaborar em equipe de forma segura e organizar o ciclo de vida do código por meio de **branches** (ramificações).

Como parte prática e entregável desse estudo, elaboramos também um material completo em formato Markdown (`.md`), detalhando um guia prático passo a passo de como utilizar o Git e o GitHub no dia a dia.

---

## 2. Objetivos do Trabalho

- **Compreender a diferença entre Git e GitHub**: Entender o papel do Git como ferramenta local de versionamento distribuído e do GitHub como plataforma de hospedagem remota e colaboração.
- **Dominar o ciclo de vida dos arquivos no Git**: Praticar a transição entre *Working Directory*, *Staging Area* (Index) e *Repository* (Local e Remoto).
- **Praticar a criação e o gerenciamento de Branches**:
  - Criar e alternar entre branches para desenvolver tarefas de forma isolada.
  - Proteger a branch principal (`main`) de alterações instáveis ou incompletas.
  - Praticar o envio de branches para o repositório remoto e estratégias de mesclagem (*merge*).
- **Produzir documentação técnica clara**: Consolidar os aprendizados em um arquivo de referência acessível para consulta contínua de comandos e conceitos.

---

## 3. O que foi Desenvolvido na Prática

Durante o desenvolvimento deste trabalho, realizamos as seguintes etapas:

1. **Inicialização e Configuração do Repositório**:
   - Configuração de identidade dos autores (`user.name` e `user.email`).
   - Configuração da branch padrão `main` e conexão com o repositório remoto no GitHub.

2. **Trabalho com Múltiplas Branches**:
   - Criação de ramificações independentes (como a branch `joaovitor`) para simular o trabalho em paralelo de membros da equipe sem impactar a estabilidade da linha principal.
   - Realização de commits incrementais e descritivos em branches dedicadas.
   - Sincronização das branches locais com o servidor remoto (`git push -u origin <nome-da-branch>`).

3. **Elaboração do Guia Completo de Git e GitHub (`.md`)**:
   - Criamos um arquivo de documentação técnica estruturado em Markdown contendo todo o manual de utilização das ferramentas, facilitando o aprendizado e servindo de consulta rápida.

---

## 4. Conteúdo Abordado no Guia de Estudo

O guia elaborado em Markdown detalha os seguintes tópicos essenciais:

| Módulo | Conteúdo Principal |
| :--- | :--- |
| **Conceitos Fundamentais** | O que é Git, o que é GitHub e como funciona a arquitetura distribuída |
| **Instalação e Configuração** | Instalação no sistema operacional e configuração global de usuário |
| **Ciclo Básico de Versionamento** | Comandos `git init`, `git status`, `git add`, `git commit` e histórico via `git log` |
| **Trabalho Remoto** | Conectar repositórios locais ao GitHub (`git remote`), enviar alterações (`git push`) e baixar novidades (`git pull` / `git fetch`) |
| **Gerenciamento de Branches** | Criação (`git branch`), troca (`git checkout` ou `git switch`), junção de código (`git merge`) e exclusão de ramificações |
| **Resolução de Conflitos** | Como identificar, analisar e resolver conflitos de mesclagem |
| **Boas Práticas** | Convenções de mensagens de commit, uso de `.gitignore` e fluxo com Pull Requests |

---

## 5. Estrutura dos Arquivos do Projeto

```text
Git-Trabalho/
├── ExplicaçãoTrabalho.md    # Este relatório: contextualização do estudo, objetivos e branches
├── joao vitor.md             # Guia prático e didático sobre como utilizar o Git e o GitHub
└── readme.md                 # Arquivo de apresentação do repositório
```

---

## 6. Conclusão e Aprendizados

A execução deste trabalho permitiu consolidar a importância do controle de versões no fluxo de trabalho profissional de tecnologia. O uso de **branches** provou ser um recurso indispensável para permitir que múltiplos desenvolvedores colaborem simultaneamente sem gerar sobreposição indevida de arquivos ou quebra de funcionalidades em produção.

A produção conjunta do guia em Markdown assegurou a fixação dos comandos essenciais e servirá como material de consulta permanente para futuros projetos e integrantes do time.
