# Emacs Init
## Português (Brasil)
No Emacs usamos sequências de teclas descritas por `C-` e `M-` que são para:
* `C-` - _Ctrl +_
* `M-` - _Alt +_ 
* `S-` - _Shift +_
* `s-` - _Super(Windows) +_

Então o comando `C-x C-c`, para sair do Emacs, é `Ctrl + x` e depois `Ctrl + c`.

### Aplicando configuração
Após instalar o Emacs, utilize `C-x C-f` e digite o diretório de onde foi baixado o arquivo `setconfig.org`, dentro do clone desse repositório. Procure no arquivo pelas configurações de diretórios e arquivos, caso queira modificar. Se não, apenas crie-os:
* `~/Documents/org/roam`
* `~/Documents/org/tasks.org`
* `~/.emacs.d/file.bib`
* `~/Documents/org/csl/`

Faça então:
* Copie `setconfig.org` para `~/Documents/org/roam/emacs_config.org`
* Mova `abnt.csl` para `~/Documents/org/csl/abnt.csl`
* Baixe o orderless `M-x package-vc-install RET orderless`
* Use o comando `M-x treesit-install-language-gramar RET` e escolha a linguagem para baixar o Treesit
* Baixe as fontes com os comandos `M-x nerd-icons-install-fonts RET` e `M-x all-the-icons-install-fonts`

Baixe os LSP para as linguagens que deseja [aqui](https://github.com/joaotavora/eglot?tab=readme-ov-file#connecting-to-a-server), e pronto! Após isso, utilize o comando `C-c C-v t` para aplicar as configurações ao arquivo `init.el`. Feche o Emacs, e abra novamente.

### Elcord
Caso queira o **Elcord-mode**, eu fiz uma atualização do **Elcord** para o `ts-mode` em [Elcord-ts](https://github.com/rahvax/elcord-ts)

## English (Coming Soon)
