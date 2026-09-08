# Anotações de Git e GitHub

## 1. O que é Git?

Git é um sistema de controle de versão usado para registrar alterações em arquivos de um projeto ao longo do tempo. Ele permite acompanhar versões, voltar atrás em caso de erro e trabalhar em equipe de forma organizada.

## 2. O que é GitHub?

GitHub é uma plataforma online que hospeda repositórios Git. Ele permite compartilhar projetos, colaborar com outras pessoas, revisar código, abrir issues e usar ferramentas de integração.

## 3. Instalação

- Baixe o Git em: https://git-scm.com/
- Verifique se foi instalado corretamente:
  ```bash
  git --version
  ```

## 4. Configuração inicial

Configure seu nome e e-mail para que cada commit seja identificado corretamente:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@email.com"
```

## 5. Criando um repositório local

Dentro da pasta do projeto:

```bash
git init
```

Isso inicia um repositório Git na pasta atual.

## 6. Verificando o status

Para ver quais arquivos foram modificados, adicionados ou estão prontos para commit:

```bash
git status
```

## 7. Adicionando arquivos ao staging

O staging é a área onde você prepara as alterações para salvar no histórico:

```bash
git add nome-do-arquivo
```

Para adicionar todos os arquivos:

```bash
git add .
```

## 8. Fazendo um commit

Um commit salva uma versão do projeto com uma mensagem explicando o que foi feito:

```bash
git commit -m "Mensagem do commit"
```

## 9. Ver o histórico de commits

```bash
git log
```

Para uma visão mais resumida:

```bash
git log --oneline
```

## 10. Criando uma branch

Branches permitem desenvolver novas funcionalidades sem mexer no código principal.

```bash
git branch nome-da-branch
```

Para trocar para a branch:

```bash
git checkout nome-da-branch
```

Ou em versões mais novas:

```bash
git switch nome-da-branch
```

## 11. Criando e alternando para uma nova branch

```bash
git switch -c nome-da-branch
```

## 12. Mesclando branches

Depois de finalizar o trabalho em uma branch, você pode juntar com a branch principal:

```bash
git checkout main
git merge nome-da-branch
```

## 13. GitHub: criando um repositório remoto

No GitHub, clique em "New repository" e siga as instruções. Depois, conecte o repositório local ao remoto:

```bash
git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
```

## 14. Enviando alterações para o GitHub

```bash
git push -u origin main
```

Se a branch for `master`, use:

```bash
git push -u origin master
```

## 15. Clonando um repositório

Para baixar um projeto do GitHub para sua máquina:

```bash
git clone https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
```

## 16. Atualizando o projeto local

Se o repositório remoto foi atualizado por outra pessoa:

```bash
git pull
```

## 17. Conflitos

Conflitos acontecem quando duas pessoas alteram a mesma parte do código. O Git marca essas partes para você resolver manualmente.

Depois de editar o arquivo para corrigir o conflito:

```bash
git add nome-do-arquivo
git commit -m "Resolve conflito"
```

## 18. Desfazendo alterações

Para desfazer alterações antes de commit:

```bash
git restore nome-do-arquivo
```

Para desfazer um commit local (mantendo as alterações):

```bash
git reset --soft HEAD~1
```

Para descartar o último commit completamente:

```bash
git reset --hard HEAD~1
```

## 19. Ignorando arquivos

Crie um arquivo chamado `.gitignore` para evitar que arquivos temporários, pastas de ambiente e dados sensíveis entrem no Git.

Exemplo:

```gitignore
node_modules/
.env
__pycache__/
```

## 20. Pull request (PR)

Quando você quer enviar suas alterações para o projeto principal, normalmente:

1. Cria uma branch;
2. Faz as alterações;
3. Faz commit;
4. Envia para o GitHub com `git push`;
5. Abre um Pull Request no GitHub.

## 21. GitHub: issues e projetos

O GitHub também permite:

- abrir issues para relatar bugs ou pedir melhorias;
- comentar em pull requests;
- acompanhar tarefas com projetos e boards;
- revisar mudanças antes de integrar ao código principal.

## 22. Fluxo básico de trabalho

Um fluxo simples pode ser:

```bash
git status
git add .
git commit -m "Adiciona funcionalidade X"
git push
```

## 23. Dicas importantes

- Faça commits pequenos e frequentes;
- Escreva mensagens de commit claras;
- Sempre revise antes de dar push;
- Use branches para cada tarefa;
- Mantenha o repositório organizado;
- Faça backups e use pull regularmente.

## 24. Comandos úteis

```bash
git init
git status
git add .
git commit -m "Mensagem"
git log --oneline
git branch
git checkout nome-da-branch
git switch -c nome-da-branch
git merge nome-da-branch
git remote add origin URL
git push -u origin main
git pull
git clone URL
```

## 25. Resumo

Git serve para controlar versões de arquivos e acompanhar o desenvolvimento de um projeto. GitHub serve para compartilhar e colaborar em repositórios online. Juntos, eles são fundamentais para trabalho em equipe, organização e versionamento de software.

## 26. Exemplo prático de workflow

```bash
git init
git add README.md
git commit -m "Cria README inicial"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/MEU-REPOSITORIO.git
git push -u origin main
```

## 27. Observações finais

Estudar Git e GitHub é essencial para qualquer pessoa que trabalhe com desenvolvimento, programação, documentação de projetos ou colaboração em equipe. Com o tempo, esses comandos se tornam cada vez mais naturais e ajudam muito no dia a dia.
