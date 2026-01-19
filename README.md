# full-stack

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQxBV8Vm4NfkAC2Y2KNFx05Imzdq_HtkwBQiw&s">



Tutorial de Comandos Básicos do Git

1. Configuração Inicial
Antes de tudo, identifique-se para o Git. Isso é importante porque cada "commit" (registro) leva o seu nome.

Bash

git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"

2. Iniciando um Repositório
Você pode começar um projeto do zero ou baixar um que já existe.

Para começar na sua pasta local:

Bash

git init
Para copiar um projeto do GitHub:

Bash

git clone https://github.com/usuario/repositorio.git
3. O Ciclo de Trabalho (O "Feijão com Arroz")
O fluxo básico consiste em: Alterar arquivos → Preparar → Salvar.

Verificar o status: Veja quais arquivos foram modificados.

Bash

git status
Adicionar arquivos (Staging): Prepare o arquivo para ser salvo.

Bash

git add nome-do-arquivo.js  # Adiciona um arquivo específico
git add .                   # Adiciona todas as mudanças
Salvar a versão (Commit): Grava suas alterações com uma mensagem explicativa.

Bash

git commit -m "Explique o que você fez aqui"
4. Sincronizando com o GitHub
Depois de salvar localmente, você precisa enviar para o servidor (GitHub).

Conectar ao repositório remoto: (Só precisa fazer uma vez por projeto)

Bash

git remote add origin https://github.com/usuario/repositorio.git
Enviar para o GitHub (Push):

Bash

git push -u origin main
Baixar novidades do GitHub (Pull): Use se alguém da sua equipe alterou o código.

Bash

git pull origin main
💡 Dicas de Ouro
git log: Mostra o histórico de todos os commits realizados.

.gitignore: Crie um arquivo com esse nome e coloque dentro dele o nome de pastas ou arquivos que você não quer que o Git rastreie (como senhas ou pastas node_modules).