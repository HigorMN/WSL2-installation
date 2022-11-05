# WSL-windows

Resumo de instalação WSL no windows e dependencias da trybe e github.

<details>
<summary><strong>💻 Passo 1 - Instalação WSL</strong></summary>

1º Abra o Windows PowerShell como ADM e execute o comando:

```wsl
wsl --install
```

2º Enquanto instala o WSL abra o Microsoft Store e procure pelo aplicativo:

```terminal
Windows terminal
```

  <details>
    <summary>Imagem do aplicativo - Windows terminal</summary>
    <img src="./images/windows-terminal.png" />
  </details>

- Em seguida instale o aplicativo Windows terminal

3º Quando o WSL for instalado reinicie o computador!

4º Após reiniciar vai aparecer um terminal pedindo para criar um usuario linux, você digita o nome do usuario e a senha para criar, e pronto você já esta com o linux instalado via WSL.

</details>

<details>
<summary><strong>💻 Passo 2 - Configurar o Windows terminal</strong></summary>

1º Abra o Windows terminal digitando na barra de pesquisa "Terminal".

2º Va nas configurações e deixe igual a imagem abaixo

- Em inicialização

<img src="./images/windows-terminal-config.png" />

</details>

<details>
<summary><strong>💻 Passo 3 - Instalação do Oh My Zsh </strong></summary>

1º Abra o terminal do Ubuntu e instale o zsh:

```zsh
sudo apt-get install zsh
```

2º Instale o Oh My Zsh:

- wget

```
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

</details>

<!-- <details>
<summary><strong>💻 Passo 4 - Instalação do "nvm - Node.js"</strong></summary> -->

1º Abra o terminal do Ubuntu e instale o zsh:

<!-- </details> -->
