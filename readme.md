# Comentários
Eu usei o Emacs, por aproximadamente dois anos, utilizando algumas configurações personalizadas - e outras copiadas dos repositórios oficiais, ou de meu amigo [G. Rosa](https://github.com/gabehellz) que é um usuário mais experiente que eu. Porém, eu decidi refatorar o Emacs com uma configuração própria, onde eu devo entender o que minha configuração faz e o motivo das coisas estarem aqui.

Essa configuração foi feita por mim, com foco e carinho em usar o Emacs como meu ambiente de trabalho e lazer. É aqui que eu trabalho, estudo e até organizo minha rotina. Então talvez a configuração não atenda você como um usuário, mas certamente ela foi construída pensando em usuários iniciantes como eu.

# Emacs - Configuração Pessoal
Minha configuração personalizada do editor GNU/Emacs, feita de uma forma que iniciantes possam usar ela.
## Observações Importantes
No Emacs usamos sequências de teclas descritas por `C-` e `M-` que são para:
* `C-` - _Ctrl +_
* `M-` - _Alt +_ 
* `S-` - _Shift +_
* `s-` - _Super(Windows) +_
* `RET` - é o ato de dar "enter"

Então o comando `C-x C-c`, para sair do Emacs, é `Ctrl + x` e depois `Ctrl + c`.

## Como Instalar
Minha configuração é dividida em dois núcleos: Core e Extensão. Isso é importante, pois qualquer pessoa que queira pegar apenas o Core e retirar as extensões vai possuir um editor de texto básico e funcional - sem grandes funções complexas ou pesadas que podem ser substituídas facilmente.

### 1. Aplicando a configuração
Ao instalar o editor Emacs na sua máquina, ele vai vir totalmente branco e bem esquisito comparado aos editores modernos. A primeira coisa que vai fazer é usar abrir um arquivo com `C-x C-f` e digitar o PATH até o arquivo `setconfig.org` desse repositório.

Este é o arquivo Org de configuração do Emacs. Você pode alterar as configurações dentro dos blocos de `emacs-lisp`, onde somente eles serão exportados ignorando os comentários e anexos em Org. Muito útil para documentação e anotação. Agora você deve exportar essa configuração pela primeira vez, mas antes disso vá até a categoria *Melpa* e descomente `(package-refresh-contents)`.

### 2. Criando configurações ambiente
Abra um arquivo em `~/.emacs.d/ambiente.el` e configure as seguintes variáveis:
```elisp
;;; init.el --- Configurações do meu Emacs -*- lexical-binding: t; -*-
(setq ambiente/irc-ip "IP_IRC")
(setq ambiente/irc-porta 6669)
(setq ambiente/emacs-welcome "Seja bem-vindo, Rahvax!")
(setq ambiente/emacs-config "~/Documents/Forgejo/emacs/setconfig.org")
(setq ambiente/emacs-banner "~/Documents/Forgejo/emacs/banner.txt")
(setq ambiente/org-workflow "~/Documents/org/")
(setq ambiente/org-workflow-tasks "~/Documents/org/tasks.org")
(setq ambiente/org-workflow-roam "~/Documents/org/roam")
```
Mude para as configurações desejadas em sua máquina, e crie os diretórios solicitados, assim como os arquivos. Isso evita o Emacs reclamar com avisos sobre isso (ainda não aprendi a automatizar isso, mas irei). Após crir os arquivos e configurar o ambiente, use `C-c C-v t` dentro do `setconfig.org` para exportar a configuração e `M-x restart-emacs`. Aguarde a instalação, pode demorar.

Observação: caso trave a tela, aperte várias vezes `C-g` ou `ESC` para cancelar ações, o Emacs possuí apenas um thread e isso pode congelar. Após isso irá exibir os erros, ou use `emacs --debug-init` para inicializar o Emacs com depuração.
## Pós-Instalão
(WIP)

## Conclusão
(WIP)