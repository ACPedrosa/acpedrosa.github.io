# Git e GitHub - Guia Básico para Iniciantes

## O que é Git?

O Git é um sistema de controle de versão utilizado para registrar alterações em arquivos ao longo do desenvolvimento de um projeto.

Com ele é possível:

* Salvar versões do código;
* Recuperar alterações antigas;
* Trabalhar em equipe;
* Acompanhar o histórico de modificações.

## O que é GitHub?

O GitHub é uma plataforma que hospeda repositórios Git na nuvem.

Ele permite:

* Armazenar projetos online;
* Compartilhar código;
* Trabalhar colaborativamente;
* Gerenciar versões e contribuições.

---

# Fluxo Básico de Trabalho

## Verificar alterações

Antes de enviar alterações, verifique quais arquivos foram modificados:

```bash
git status
```

---

## Adicionar arquivos para o commit

Adicionar todos os arquivos modificados:

```bash
git add .
```

Adicionar um arquivo específico:

```bash
git add index.html
```

---

## Criar um commit

Após adicionar os arquivos, registre as alterações:

```bash
git commit -m "feat: adiciona página de perfil"
```

O commit funciona como uma fotografia do estado atual do projeto.

---

## Enviar alterações para o GitHub

```bash
git push
```

Esse comando envia seus commits locais para o repositório remoto.

---

## Atualizar seu projeto local

Antes de começar a trabalhar, obtenha as alterações mais recentes:

```bash
git pull
```

Esse comando baixa e integra as alterações do repositório remoto.

---

# Comandos Mais Utilizados

## Clonar um repositório

```bash
git clone URL_DO_REPOSITORIO
```

Exemplo:

```bash
git clone https://github.com/usuario/projeto.git
```

---

## Ver histórico de commits

```bash
git log
```

Versão resumida:

```bash
git log --oneline
```

---

## Ver em qual branch você está

```bash
git branch
```

---

## Criar uma nova branch

```bash
git checkout -b feature/login
```

ou

```bash
git switch -c feature/login
```

---

## Trocar de branch

```bash
git checkout main
```

ou

```bash
git switch main
```

---

# Entendendo o git push --force

## O que ele faz?

O comando:

```bash
git push --force
```

força a atualização do repositório remoto, substituindo o histórico existente.

## Atenção

Esse comando pode apagar alterações de outras pessoas.

Utilize apenas quando:

* Receber orientação do professor;
* Estiver corrigindo um erro em commits recentes;
* Souber exatamente o que está fazendo.

Na maioria dos casos:

Use:

```bash
git push
```

Evite:

```bash
git push --force
```

---

# Padrão de Commits

Utilizamos o padrão Conventional Commits para manter o histórico organizado.

## Estrutura

```text
tipo: descrição da alteração
```

Exemplo:

```text
feat: adiciona página de perfil
```

---

## feat

Utilizado quando uma nova funcionalidade é adicionada.

Exemplos:

```text
feat: adiciona formulário de cadastro
feat: cria menu de navegação
feat: implementa modo escuro
```

---

## fix

Utilizado para correção de erros.

Exemplos:

```text
fix: corrige alinhamento do cabeçalho
fix: resolve erro de validação do formulário
fix: corrige link quebrado
```

---

## docs

Utilizado para alterações na documentação.

Exemplos:

```text
docs: atualiza README
docs: adiciona guia de instalação
docs: corrige documentação da API
```

---

## style

Utilizado para alterações visuais que não modificam funcionalidades.

Exemplos:

```text
style: ajusta espaçamento do menu
style: altera cores da interface
style: melhora responsividade
```

---

## refactor

Utilizado para reorganização ou melhoria do código sem alterar comportamento.

Exemplos:

```text
refactor: reorganiza estrutura de componentes
refactor: simplifica função de validação
```

---

## chore

Utilizado para tarefas de manutenção.

Exemplos:

```text
chore: atualiza dependências
chore: configura prettier
chore: adiciona arquivo gitignore
```

---

# Boas Práticas para Commits

## Faça

✔ Um commit para cada alteração relevante

✔ Utilize mensagens claras

✔ Faça commits frequentes

✔ Escreva mensagens objetivas

Exemplos:

```text
feat: adiciona seção de projetos
fix: corrige menu responsivo
docs: atualiza instruções de instalação
```

---

## Evite

Mensagens genéricas:

```text
update
ajustes
mudanças
teste
aaaa
```

Essas mensagens dificultam a identificação do que foi alterado.

---

# Fluxo Recomendado

```bash
git pull

git status

git add .

git commit -m "feat: adiciona página de perfil"

git push
```

Esse é o fluxo que será utilizado na maioria das atividades do curso.
