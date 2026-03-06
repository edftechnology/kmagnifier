# Como instalar o `kmagnifier` no `Linux Ubuntu`

## Resumo

Este documento apresenta os passos necessários para instalar o software de dinâmica molecular `kmagnifier` no `Linux Ubuntu`.

## _Abstract_

_This document shows the steps required to install the `kmagnifier` molecular dynamics software on `Linux Ubuntu`._

## Descrição

### `kmagnifier`

O `kmagnifier` é uma ferramenta de lupa de tela do ambiente `KDE`. Ela amplia uma região do monitor em tempo real, sendo útil para acessibilidade ou inspeção de detalhes na interface gráfica.

## 1. Configurar/Instalar/Usar o `LAMMPS` no `Linux Ubuntu`

Para instalar o `LAMMPS`, siga os passos abaixo:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando:

    ```bash
    Ctrl + Alt + T
    ```


2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando:
    ```bash
    sudo apt clean
    ```

    2.2 Remover pacotes `.deb` antigos ou duplicados do `cache` local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando:
    ```bash
    sudo apt autoclean
    ```

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando:
    ```bash
    sudo apt autoremove -y
    ```

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt update
    ```

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes:
    ```bash
    sudo apt --fix-broken install
    ```

    2.6 Limpar o `cache` do gerenciador de pacotes `apt` novamente:
    ```bash
    sudo apt clean
    ```

    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt list --upgradable
    ```

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt full-upgrade -y
    ```

3. Use o gerenciador de pacotes para instalar o programa:

    ```bash
    sudo apt install kmag -y
    ```

### 1.1 Código completo para configurar/instalar/usar

Para configurar/instalar/usar o `kmagnifier` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abrir o `Terminal Emulator`. Você pode fazer isso pressionando:

    ```bash
    Ctrl + Alt + T
    ```

2. Digite o seguinte comando e pressione `Enter`:

    ```bash
    sudo apt clean
    sudo apt autoclean
    sudo apt autoremove -y
    sudo apt update
    sudo apt --fix-broken install
    sudo apt clean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install kmag -y
    ```


## 3. Referências

[1] OPENAI. ***Instalar o `kmanifier` no `linux ubuntu` pelo `terminal emulator`***. Disponível em: <https://chatgpt.com/g/g-p-6980caf949648191ad6acfcdbe590f9e-instalar/c/69aad967-da48-8328-b703-6347e534c235>. ChatGPT. Acessado em: 18/09/2025 10:58.
