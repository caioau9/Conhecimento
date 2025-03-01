# Módulo 1 – Página 5: Instalação do Git (Windows, Linux, macOS)

## Visão Geral
Agora que entendemos como o Git funciona, vamos instalá-lo no seu computador para começar a usá-lo.

---

## 1. Instalando o Git no Windows

1. Acesse o site oficial: [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. Baixe o instalador para Windows.
3. Execute o arquivo baixado e siga as instruções.
4. Durante a instalação, mantenha as opções padrão para evitar problemas.
5. Para verificar se a instalação foi bem-sucedida, abra o **Prompt de Comando** e digite:

   ```sh
   git --version
   ```

   Se aparecer um número de versão, significa que o Git foi instalado corretamente!

---

## 2. Instalando o Git no Linux

No Linux, a instalação varia de acordo com a distribuição. Use o comando correspondente ao seu sistema:

- **Ubuntu/Debian:**
  ```sh
  sudo apt update && sudo apt install git
  ```
- **Fedora:**
  ```sh
  sudo dnf install git
  ```
- **Arch Linux:**
  ```sh
  sudo pacman -S git
  ```

Para verificar a instalação, digite:

```sh
git --version
```

Se aparecer um número de versão, o Git foi instalado corretamente.

---

## 3. Instalando o Git no macOS

Se você usa macOS, a forma mais fácil de instalar o Git é através do Homebrew:

```sh
brew install git
```

Caso não tenha o Homebrew instalado, primeiro instale-o seguindo as instruções em [https://brew.sh](https://brew.sh), e depois instale o Git com o comando acima.

Para confirmar a instalação, use:

```sh
git --version
```

---

## Resumo

- O Git pode ser instalado no **Windows**, **Linux** e **macOS**.
- No **Windows**, basta baixar e executar o instalador.
- No **Linux**, o Git pode ser instalado pelo gerenciador de pacotes da sua distribuição.
- No **macOS**, o Git pode ser instalado com o Homebrew.
- Após a instalação, use `git --version` para verificar se tudo está funcionando.

Agora que o Git está instalado, vamos configurar as primeiras opções para usá-lo no próximo tópico!
