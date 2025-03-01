# Instalação do Git

## Introdução

Antes de começar a usar o Git, é necessário instalá-lo no seu sistema operacional. O Git é compatível com Windows, Linux e macOS, e cada sistema possui um método específico de instalação.

## Instalando o Git no Windows

A forma mais comum de instalar o Git no Windows é utilizando o instalador oficial.

### Passo a passo:
1. Acesse o site oficial do Git: [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. Baixe o instalador compatível com sua versão do Windows.
3. Execute o instalador e siga as instruções, mantendo as opções padrão recomendadas.
4. Após a instalação, abra o `Git Bash` e verifique se a instalação foi bem-sucedida com o comando:

```sh
$ git --version
```

Se o Git foi instalado corretamente, será exibida a versão instalada.

## Instalando o Git no Linux

A maioria das distribuições Linux já possui o Git disponível nos repositórios oficiais.

### Para Ubuntu/Debian:
```sh
$ sudo apt update
$ sudo apt install git
```

### Para Fedora:
```sh
$ sudo dnf install git
```

### Para Arch Linux:
```sh
$ sudo pacman -S git
```

Após a instalação, verifique a versão com:
```sh
$ git --version
```

## Instalando o Git no macOS

No macOS, o Git pode ser instalado de várias formas, sendo as mais comuns:

### Usando Homebrew (recomendado):
```sh
$ brew install git
```

### Usando o Xcode:
Se você tiver o Xcode instalado, basta executar o comando:
```sh
$ git --version
```
Se o Git não estiver instalado, o macOS oferecerá a opção de instalar os Developer Tools.

## Configuração Inicial
Após instalar o Git, configure seu nome e e-mail para associar seus commits corretamente:
```sh
$ git config --global user.name "Seu Nome"
$ git config --global user.email "seu.email@example.com"
```

Para verificar as configurações, use:
```sh
$ git config --list
```

## Resumo
- O Git pode ser instalado no **Windows, Linux e macOS**.
- No **Windows**, utilize o instalador oficial.
- No **Linux**, instale via gerenciador de pacotes.
- No **macOS**, utilize o **Homebrew** ou o Xcode.
- Após a instalação, configure seu nome e e-mail para associar corretamente seus commits.

---

No próximo tópico, veremos as **primeiras configurações do Git**, como definir nome, e-mail e editor padrão.