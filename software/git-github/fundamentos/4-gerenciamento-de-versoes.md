# Módulo 1 – Página 4: Como o Git gerencia versões (De que forma ele salva os arquivos?)

## Visão Geral

Esta página explica como o Git armazena e gerencia diferentes versões dos arquivos de um projeto. Entender como o Git organiza os dados é essencial para aproveitar todo o poder dessa ferramenta.

---

## Como o Git Guarda os Arquivos

O Git funciona como um grande álbum de fotos do seu projeto. Cada vez que você faz uma alteração e a salva, o Git tira uma foto do estado atual dos arquivos e os organiza para que você possa acessá-los depois.

**Componentes importantes do Git para gerenciar versões:**

- **Versão (Commit):** Cada foto salva do seu projeto. Você pode voltar a qualquer uma delas sempre que precisar.
- **Pastas Organizadoras (Tree):** O Git guarda os arquivos dentro de uma estrutura de pastas, para manter tudo organizado.
- **Arquivo Armazenado (Blob):** O conteúdo de cada arquivo salvo, sem informações extras.
- **Última Versão (HEAD):** O Git sempre aponta para a última versão salva do projeto, facilitando seu trabalho.

---

## Como o Git Lembra das Versões Antigas?

- Cada vez que você salva uma nova versão do projeto, o Git mantém um histórico das mudanças.
- Ao invés de salvar só as diferenças, ele guarda uma cópia completa do projeto.
- Isso permite que você volte para qualquer versão anterior com segurança.

**Exemplo:** Imagine que você esteja escrevendo um livro e quer salvar rascunhos diferentes sem perder os antigos. O Git faz isso automaticamente!

---

## Como o Git Garante que Nada se Perca?

- O Git usa uma espécie de “impressão digital” para identificar cada versão do projeto.
- Sempre que um arquivo é salvo, ele recebe um código único.
- Se o conteúdo mudar, o código muda também, garantindo que tudo esteja seguro e organizado.

---

## Resumo

- O Git funciona como um álbum de fotos do seu projeto, onde cada versão salva pode ser acessada depois.
- Ele mantém um histórico completo, garantindo que nada seja perdido.
- Cada arquivo salvo recebe um código único, tornando o processo seguro e confiável.

No próximo tópico, vamos aprender como **instalar o Git no seu computador**!