# WSL-windows

Resumo de instalação WSL no windows e dependencias da trybe e github.

<details>
<summary><strong>🪟 Passo 1 - Instalação WSL</strong></summary>

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
<summary><strong>💻 Passo 2 - Configuração do Terminal</strong></summary>

1º Abra o Windows terminal, digitando na barra de pesquisa do windows - "Terminal".

2º Va nas configurações e deixe igual a imagem abaixo

- Em inicialização

<img src="./images/windows-terminal-config.png" />

</details>

<details>
<summary><strong>💚 Passo 3 - Instalação do Oh My Zsh </strong></summary>

1º Abra o terminal do Ubuntu e instale o zsh:

```zsh
sudo apt-get install zsh
```

2º Feche o terminal e abra um novo terminal e instale o Oh My Zsh:

- wget

```wget
install wget
```

```my zsh
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

</details>

<details>
<summary><strong>📇 Passo 4 - Instalação do vscode com code .</strong></summary>

1º Abra o Microsoft Store e procure por vscode:

- OBS: "A instalação tem que ser pela Microsoft Store"

2º Abra um novo terminal do Ubunto e digite o comando abaixo para abrir o vscode da pasta atual:

```code
code .
```

</details>

<details>
<summary><strong>📗 Passo 5 - Instalação do Node com NVM</strong></summary>

1º Abra o terminal do Ubunto e digite o comando abaixo para instalar o NVM:

```nvm
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.2/install.sh | bash
```

2º Abra uma nova janela do terminal para utilizar os comandos do NVM e digite o comando abaixo para instalar a versão mais atual do node;

```node atual
nvm install lts/
```

3º Em seguida para instalar a versão do node para os projetos da trybe digite o comando abaixo:

```node v16
nvm install 16
```

</details>

<details>
<summary><strong>🔑 Passo 6 - Instalação da chave ssh </strong></summary>

1º Abra o terminal do Ubunto e digite o comando abaixo para instalar uma nova chave publica:

- OBS: onde está escrito "your_email@example.com" é para digitar seu email do github.

```criando key
ssh-keygen -t ed25519 -C "your_email@example.com"
```

- ENTER;
- DIGITE UMA SENHA QUE VOCÊ LEMBRE;
- DIGITE A SENHA NOVAMENTE NOVAMENTE;

2º Agora vamos adicionar a chave criada para o github, no terminal digite o comando abaixo para copiar a chave pública SSH para sua área de transferência.

```chave pub
cat ~/.ssh/id_ed25519.pub
```

3º No canto superior direito de qualquer página do github, clique na foto do seu perfil e em Configurações.

<img src="./images/userbar-account-settings.png" width="150"/>

4º Na seção "Access" da barra lateral, clique nas SSH and GPG keys.

5º Clique em New SSH key.
<img src="./images/ssh-add-ssh-key-with-auth.png" />

6º Adicione um titulo para sua chave.

7º Cole sua chave no campo "Key".

<img src="./images/ssh-key-paste-with-type.png" />

8º Clique em Add SSH key.

<img src="./images/ssh-add-key.png" />

</details>

<details>
<summary><strong>🌎 Passo 7 - Instalação google chrome no linux</strong></summary>

1º Abra o terminal do Ubunto e digite o comando abaixo para instalar o google chrome:

```baixar chrome
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```

2º Instale o pacote do Chrome baixado anteriormente.

```
sudo dpkg -i google-chrome-stable_current_amd64.deb
```

3º Corrija os erros de instalação do Chrome.

```
sudo apt-get install -f
```

4º Digite "google-chrome" e pressione a tecla ↵ Enter para abrir o Chrome.

</details>
