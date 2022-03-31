# Ultron-Ubuntu

REQUERIMENTOS (Windows):
Instalar GIT: https://git-scm.com/download/win
Instalar Node (LTS): https://nodejs.org/en/
Instalar Google Chrome: https://www.google.com/intl/pt-BR/chrome/

REQUERIMENTOS (Linux):

Deixar o sistema operacional atualizado:
sudo apt update
sudo apt upgrade

Instalar Git:
sudo add-apt-repository ppa:git-core/ppa && sudo apt update
sudo apt install git

Instalar Node (LTS):
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
. ~/.bashrc
nvm list-remote

Selecione a última versão estável (LTS):
nvm install v16.14.2 

Instalar Google Chrome:
wget -q -O - https://dl.google.com/linux/linux_signing_key.pub | sudo apt-key add - 
sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'
sudo apt install google-chrome-stable

Instalar última versão do npm:
npm install -g npm@latest

Isso tudo é necessário para o bot funcionar corretamente.

1 - Clone este projeto OU faça download da ultima release :
Para clonar, digite os comandos abaixo no Terminal do seu sistema:

git clone https://github.com/thiagopivatto/Ultron-Ubuntu.git
cd Ultron-Ubuntu


2 - Instale as dependências :
Antes de executar o comando abaixo, tenha certeza que você está no diretório do projeto que você clonou!

npm i


3 - Uso :
Dentro da pasta do projeto após ter realizado todos os passos anteriores, execute este comando.

npm start

Se for a sua primeira vez executando escaneie o QR Code com o seu celular (No modo BETA que não exige conexão com o celular) e digite no terminal SEU número de telefone COM CÓDIGO DO PAÍS no terminal. Ele irá encerrar o bot e você deverá inicia-lo novamente.


4 - Funcionamento :
Após todos os passos anteriores feitos, seu bot já deve estar iniciando normalmente, use os comandos abaixo para visualizar os comandos disponíveis.

!menu - Dá acesso ao MENU PRINCIPAL.
!admin - Dá acesso ao MENU de ADMINISTRADOR/DONO DO BOT.

Todos os comandos agora tem um guia ao digitar !comando guia

Pronto! Seu bot já está funcionando!!
Obs: Se você deseja utilizar os comandos !noticias (noticias atuais), !qualmusica(reconhecimento de músicas) e o recurso de anti-pornografia vá para o passo 5.

Sugestão: Caso você esteja rodando o BOT em uma VM, execute os seguintes comandos para que o BOT siga em execução mesmo com o terminal fechado:

Instalar tmux:
sudo apt install tmux

Criar uma sessão no tmux:
tmux new -s nome_da_sessao

Sair da sessão:
Ctrl B + D

Voltar a sessão:
tmux attach-session -t nome_da_sessao


5 - Obtenha as Chaves de APIs:

Primeiramente crie as chaves API. Para informações detalhadas sobre como obter as chaves do NewsAPI(Notícias), ACRCloud(Reconhecimento de Músicas) e DeepAI(Detector de Nudez e Pornografia) abra o arquivo "CHAVESAPI.md" na raiz do projeto com um editor de textos de sua preferência e siga o passo a passo corretamente.


6 - Configuração do arquivo .env:

Após a criação das chaves de API, abra o arquivo .env na raiz do projeto e edite manualmente :
    #############  DADOS DO BOT ############# 

    NOME_ADMINISTRADOR= Digite seu nome
    NOME_BOT= Digite o nome que o bot vai ter
    NOME_AUTOR_FIGURINHAS = Digite o nome que vai aparecer como autor das figurinhas

    ############ CONFIGURAÇÕES DO BOT ############# 

    # LEMBRE-SE SEU NÚMERO DE WHATSAPP E NÃO O DO BOT.
    NÚMERO_DONO = SEU número com o código do país incluido. ex: 55119xxxxxxxx
    # NEWSAPI - NOTICIAS 
    API_NEWS_ORG = recebe a chave da conta que voce criar no site newsapi.org 
    # ACRCLOUD - RECONHECIMENTO DE MÚSICAS
    acr_host= recebe seu endereço de host obtido no https://acrcloud.com/
    acr_access_key= recebe seu access_key obtido no https://acrcloud.com/
    acr_access_secret= recebe seu access_secret obtido no https://acrcloud.com/
    # DEEPAI - DETECTOR DE NUDEZ/PORNOGRAFIA
    API_DEEPAI= recebe a chave da conta que voce criar no site deepai.org 
Obs: Se o seu sistema for MAC, habilite a exibição de arquivos ocultos para exibir o .env na raiz do projeto.


7 - Recursos Principais:
Figurinhas
Criador de Sticker
✅	Foto para Sticker
✅	Sticker para foto
✅	Texto para Sticker
✅	Texto para Sticker Animado
✅	Video/GIF para Sticker
✅	Foto para Sticker (Sem fundo)
Downloads
Downloads
✅	Download de aúdio/videos (Youtube)
✅	Download de imagens/videos (Instagram)
✅	Download de imagens/videos (Twitter)
✅	Download de videos (Facebook)
✅	Download de videos (Tiktok)
✅	Pesquisa/Download de Imagens
Utilidades Gerais
Utilitários
✅	Efeitos de Aúdio
✅	Texto para voz
✅	Letra de Música
✅	Reconhecimento de músicas
✅	Detector de DDD
✅	Consulta de Clima/Previsão do Tempo
✅	Conversão de Moedas
✅	Calculadora básica
✅	Pesquisa Web
✅	Detector Anime
✅	Lançamentos recentes - Animes
✅	Rastreamento Correios
✅	Noticias Atuais
✅	Tradutor
Administração de Grupo
Apenas Grupo
✅	Promover usuário
✅	Rebaixar usuário
✅	Remover usuário
✅	Adicionar usuário
✅	Marcar todos
✅	Obter link do grupo
✅	Redefinir link do grupo
✅	Obter lista de administradores
✅	Obter dono do grupo
✅	Lista Negra
✅	Mutar Grupo
✅	Bem Vindo
✅	Auto Sticker
✅	Anti Trava
✅	Anti Pornô
✅	Anti Fake
✅	Anti Link
✅	Anti Flood
✅	Contagem de mensagens
✅	Marcar inativos
✅	Banir inativos
✅	Bloquear/Desbloquear Comandos
✅	Votação de Ban
✅	Enquete
✅	Banir Todos
✅	Apagar mensagens do bot
Administração de Dono
Apenas Dono do Bot
✅	Entrar em um grupo
✅	Sair de todos os grupos
✅	Limpar todos os chats
✅	Broadcast - Anuncio Geral
✅	Bloquear/Desbloquear usuário
✅	Sistema de Tipos de Usuários
✅	Limitador comandos diários (por usuário)
✅	Limitador de comandos por minuto (por usuário)
✅	Limitador de mensagens privadas (Anti-flood)
✅	Auto Sticker Privado
✅	Anti Trava Privado
✅	Sair do grupo
✅	Limpar somente chat de contatos
✅	Obter lista de usuários bloqueados
✅	Modificar status atual do bot