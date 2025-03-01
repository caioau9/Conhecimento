# Módulo 1 – Página 7: Conceitos Fundamentais

## Visão Geral

Agora que o Git está instalado e configurado, é essencial entender seus conceitos fundamentais. Estes conceitos são a base para trabalhar com o Git de maneira eficiente.

---

## 1. Repositórios

O **repositório** é onde o Git armazena o histórico das mudanças no projeto. Ele pode ser **local** (no seu computador) ou **remoto** (hospedado em um servidor como o GitHub).

Para iniciar um repositório Git em uma pasta, use:

```sh
git init
```

Para clonar um repositório já existente, use:

```sh
git clone <URL-do-repositório>
```

---

## 2. Commits

Um **commit** é um registro de alterações no projeto. Cada commit possui um identificador único (hash) e uma mensagem descrevendo as mudanças feitas.

Para criar um commit:

```sh
git commit -m "Mensagem do commit"
```

Os commits permitem reverter mudanças e acompanhar o histórico do projeto.

---

## 3. Branches

Uma **branch** (ramificação) permite criar versões paralelas do projeto, sem afetar a principal. Isso é útil para desenvolver novos recursos sem comprometer a versão estável.

Criando uma nova branch:

```sh
git branch minha-nova-branch
```

Trocando para outra branch:

```sh
git checkout minha-nova-branch
```

Ou:

```sh
git switch minha-nova-branch
```

---

## 4. HEAD

O **HEAD** é um ponteiro que indica qual commit e branch estão ativos no momento. Normalmente, ele aponta para o último commit da branch atual.

Para ver onde o HEAD está apontando:

```sh
git log --oneline --decorate
```

---

## 5. Área de Staging

A **Área de Staging** é um espaço temporário onde as mudanças são preparadas antes de serem confirmadas (commitadas). Isso permite agrupar alterações antes de criar um commit.

Para adicionar arquivos à área de staging:

```sh
git add arquivo.txt
```

Para adicionar todos os arquivos modificados:

```sh
git add .
```

---

## Resumo

- **Repositórios** armazenam o histórico do projeto e podem ser locais ou remotos.
- **Commits** registram mudanças e possuem identificadores únicos.
- **Branches** permitem desenvolver recursos sem afetar a versão principal.
- **HEAD** aponta para o commit atual.
- **Área de Staging** permite preparar alterações antes de confirmar.

Com esses conceitos em mente, podemos começar a usar o Git na prática!
