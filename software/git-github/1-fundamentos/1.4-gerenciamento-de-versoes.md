# Como o Git Gerencia Versões

## Introdução

O Git é um sistema de controle de versão distribuído que gerencia mudanças nos arquivos de um projeto. Diferente de outros sistemas de controle de versão centralizados, o Git armazena cada versão como um conjunto de snapshots, garantindo eficiência e integridade dos dados.

## Conceitos Fundamentais
O Git utiliza uma estrutura baseada em três componentes principais:

### 1. **Blobs (Binary Large Objects)**
Blobs representam o conteúdo dos arquivos armazenados no repositório. Cada versão de um arquivo recebe um identificador único baseado no seu conteúdo, utilizando a criptografia SHA-1.

### 2. **Trees (Árvores)**
As trees organizam os blobs em uma estrutura hierárquica, semelhante a diretórios e subdiretórios. Cada tree contém referências a blobs e outras trees, permitindo que o Git reconstrua a estrutura do projeto em qualquer ponto do tempo.

### 3. **Commits**
Os commits representam um estado do repositório em determinado momento. Cada commit contém:
- Uma referência à tree correspondente àquele momento.
- Um ponteiro para o commit anterior (ou commits, no caso de merges).
- Informações do autor e data do commit.
- Uma mensagem descritiva.

## Estrutura Interna do Git
Internamente, o Git armazena os dados no diretório `.git/` do repositório, utilizando os seguintes componentes:

- **HEAD**: Aponta para o commit atual.
- **Refs**: Contêm referências para branches, tags e outros objetos.
- **Objects**: Diretório onde blobs, trees e commits são armazenados.

## Como o Git Rastreia Alterações
Quando um desenvolvedor edita um arquivo e executa comandos do Git, o fluxo ocorre da seguinte forma:

1. **Edição de Arquivos**: O usuário modifica os arquivos no diretório de trabalho.
2. **Staging (Área de Preparação)**: O comando `git add` adiciona as alterações à área de staging.
3. **Commit**: O comando `git commit` salva as alterações de forma permanente no histórico do repositório.

Cada commit cria um snapshot do estado dos arquivos naquele momento, permitindo que o histórico do projeto seja reconstruído ou revertido quando necessário.

## Exemplo Prático
Suponha que criamos um arquivo `arquivo.txt`, adicionamos conteúdo e o commitamos:

```sh
$ echo "Primeira versão" > arquivo.txt
$ git add arquivo.txt
$ git commit -m "Adiciona primeira versão do arquivo"
```

Agora, ao inspecionar o histórico de commits, podemos ver a referência ao commit criado:

```sh
$ git log --oneline
```

Saída esperada:
```
ab12c34 Adiciona primeira versão do arquivo
```
Isso mostra que o Git armazenou o commit e pode recuperar essa versão quando necessário.

## Resumo
- O Git armazena versões como **snapshots**, não como diferenças entre arquivos.
- Utiliza **blobs, trees e commits** para organizar os dados.
- O diretório `.git/` contém toda a estrutura necessária para rastrear o histórico.
- O processo de versionamento envolve **edição, staging e commit**.

---

No próximo tópico, veremos como instalar o Git em diferentes sistemas operacionais.