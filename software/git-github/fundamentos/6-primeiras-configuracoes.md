# Módulo 1 – Página 6: Primeiras Configurações do Git

## Visão Geral
Agora que o Git está instalado, precisamos configurá-lo para garantir que suas alterações sejam identificadas corretamente. Aqui, vamos definir seu nome, e-mail e algumas preferências básicas.

---

## 1. Configurando Nome e E-mail
Cada commit no Git contém informações sobre o autor. Para definir seu nome e e-mail, use os seguintes comandos:

```sh
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

**Explicação:**  
- `user.name` define o nome que aparecerá nos commits.
- `user.email` define o e-mail associado aos commits.
- `--global` aplica a configuração para todos os repositórios do usuário. Para configurar apenas um repositório específico, remova `--global`.

Para verificar se a configuração foi aplicada corretamente, use:
```sh
git config --global --list
```
Isso exibirá a lista de configurações do Git.

---

## 2. Definindo o Editor Padrão
Por padrão, o Git pode abrir um editor de texto para mensagens de commit ou edição de configurações. Você pode definir um editor de sua preferência:

- **VS Code**:
  ```sh
  git config --global core.editor "code --wait"
  ```
- **Vim**:
  ```sh
  git config --global core.editor "vim"
  ```
- **Nano**:
  ```sh
  git config --global core.editor "nano"
  ```

Se não configurar um editor, o Git usará o editor padrão do sistema.

---

## 3. Configurando o Estilo de Exibição de Branches
O Git permite visualizar as branches de forma mais clara. Podemos definir um alias para isso:

```sh
git config --global alias.branches "branch --all"
```
Agora, ao executar `git branches`, você verá todas as branches do repositório.

---

## Resumo
- **Nome e e-mail**: Configurados com `git config --global user.name` e `git config --global user.email`.
- **Editor padrão**: Pode ser definido para VS Code, Vim ou Nano.
- **Alias útil**: `git branches` para listar todas as branches.
- Para visualizar todas as configurações, use `git config --global --list`.

Com essas configurações prontas, seu Git está preparado para ser usado! No próximo módulo, veremos os conceitos fundamentais do Git.
