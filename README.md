# Ultron-Ubuntu

Guia de instalação do BOT para Whatsapp com diversas funcionalidades!<br><br>

REQUERIMENTOS (Windows):<br>
Instalar GIT: https://git-scm.com/download/win<br>
Instalar Node (LTS): https://nodejs.org/en/<br>
Instalar Google Chrome: https://www.google.com/intl/pt-BR/chrome/<br><br>

REQUERIMENTOS (Linux): <br>
Deixar o sistema operacional atualizado: <br>
`sudo apt update` <br>
`sudo apt upgrade` <br><br>

Instalar Git: <br>
`sudo add-apt-repository ppa:git-core/ppa && sudo apt update` <br>
`sudo apt install git` <br><br>

Instalar Node (LTS):
`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash` <br>
`. ~/.bashrc` <br>
`nvm list-remote` <br>
Selecione a última versão estável (LTS), no momento a versão mais atual é a 16.14.2: <br>
`nvm install v16.14.2` <br><br>

Instalar Google Chrome: <br>
`wget -q -O - https://dl.google.com/linux/linux_signing_key.pub | sudo apt-key add -` <br>
`sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'` <br>
`sudo apt install google-chrome-stable` <br><br>

Instalar última versão do npm: <br>
`npm install -g npm@latest` <br><br>

Isso tudo é necessário para o bot funcionar corretamente. <br><br>

**1) Clone este projeto OU faça download da ultima release:** <br> 
Para clonar, digite os comandos abaixo no Terminal do seu sistema: <br><br>

`git clone https://github.com/thiagopivatto/Ultron-Ubuntu.git` <br>
`cd Ultron-Ubuntu` <br><br><br>


**2) Instale as dependências:** <br>
Antes de executar o comando abaixo, tenha certeza que você está no diretório do projeto que você clonou!<br><br>

`npm i` <br><br>


**3) Uso:** <br>
Dentro da pasta do projeto após ter realizado todos os passos anteriores, execute este comando.<br><br>

`npm start`<br><br>

Se for a sua primeira vez executando escaneie o QR Code com o seu celular (No modo BETA que não exige conexão com o celular) e digite no terminal SEU número de telefone COM CÓDIGO DO PAÍS no terminal. Ele irá encerrar o bot e você deverá inicia-lo novamente.<br><br><br>


**4) Funcionamento:**<br>
Após todos os passos anteriores feitos, seu bot já deve estar iniciando normalmente, use os comandos abaixo para visualizar os comandos disponíveis.<br><br>

!menu - Dá acesso ao MENU PRINCIPAL.<br>
!admin - Dá acesso ao MENU de ADMINISTRADOR/DONO DO BOT.<br><br>

Todos os comandos agora tem um guia ao digitar !comando guia<br><br>

Pronto! Seu bot já está funcionando!!<br>
Obs: Se você deseja utilizar os comandos !noticias (noticias atuais), !qualmusica(reconhecimento de músicas) e o recurso de anti-pornografia vá para o passo 5.<br><br>

Sugestão: Caso você esteja rodando o BOT em uma VM, execute os seguintes comandos para que o BOT siga em execução mesmo com o terminal fechado:<br><br>

Instalar tmux:<br>
`sudo apt install tmux`<br><br>

Criar uma sessão no tmux:<br>
`tmux new -s nome_da_sessao`<br><br>

Sair da sessão:<br>
Ctrl B + D<br><br>

Voltar a sessão:<br>
`tmux attach-session -t nome_da_sessao`<br><br><br>


**5) Obtenha as Chaves de APIs:**<br><br>

Primeiramente crie as chaves API. Para informações detalhadas sobre como obter as chaves do NewsAPI(Notícias), ACRCloud(Reconhecimento de Músicas) e DeepAI(Detector de Nudez e Pornografia) abra o arquivo "CHAVESAPI.md" na raiz do projeto com um editor de textos de sua preferência e siga o passo a passo corretamente.<br><br><br>



**6) Configuração do arquivo .env:**<br><br>

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


**7) Recursos Principais:**<br>
### Figurinhas

| Criador de Sticker |                Recursos        |
| :-----------: | :--------------------------------: |
|       ✅       | Foto para Sticker     |
|       ✅       | Sticker para foto              |
|       ✅       | Texto para Sticker                  |
|       ✅       | Texto para Sticker Animado                 |
|       ✅       | Video/GIF para Sticker |
|       ✅       | Foto para Sticker (Sem fundo) |

### Downloads 

| Downloads      |                Recursos            |
| :------------: | :---------------------------------------------: |
|       ✅        |   Download de aúdio/videos (Youtube)    |
|       ✅        |   Download de imagens/videos (Instagram)  |
|       ✅        |   Download de imagens/videos (Twitter)            |
|       ✅        |   Download de videos (Facebook)            |
|       ✅        |   Download de videos (Tiktok)            |
|       ✅        |   Pesquisa/Download de Imagens                  |

### Utilidades Gerais

| Utilitários |                     Recursos            |
| :------------: | :---------------------------------------------: |
|       ✅       | Efeitos de Aúdio
|       ✅        |   Texto para voz                   |
|       ✅        |   Letra de Música              |
|       ✅        |   Reconhecimento de músicas                 |
|       ✅        |   Detector de DDD             |
|       ✅        |   Consulta de Clima/Previsão do Tempo            |
|       ✅        |   Conversão de Moedas           |
|       ✅        |   Calculadora básica           |
|       ✅        |   Pesquisa Web                  |
|       ✅        |   Detector Anime                  |
|       ✅        |   Lançamentos recentes  - Animes                 |
|       ✅        |   Rastreamento Correios                  |
|       ✅        |   Noticias Atuais                 |
|       ✅        |   Tradutor                |

### Administração de Grupo

| Apenas Grupo  |                     Recursos             |
| :------------: | :---------------------------------------------: |
|       ✅        |   Promover usuário                  |
|       ✅        |   Rebaixar usuário                |
|       ✅        |   Remover usuário                     |
|       ✅        |   Adicionar usuário                      |
|       ✅        |   Marcar todos              |
|       ✅        |   Obter link do grupo               |
|       ✅        |   Redefinir link do grupo               |
|       ✅        |   Obter lista de administradores               |
|       ✅        |   Obter dono do grupo              |
|       ✅        |   Lista Negra  |
|       ✅        |   Mutar Grupo
|       ✅        |   Bem Vindo  |
|       ✅        |   Auto Sticker |
|       ✅        |   Anti Trava |
|       ✅        |   Anti Pornô |
|       ✅        |   Anti Fake |
|       ✅        |   Anti Link  |
|       ✅        |   Anti Flood  |
|       ✅        |   Contagem de mensagens |
|       ✅        |   Marcar inativos |
|       ✅        |   Banir inativos |
|       ✅        |   Bloquear/Desbloquear Comandos |
|       ✅        |   Votação de Ban |
|       ✅        |   Enquete |
|       ✅        |   Banir Todos  |
|       ✅        |   Apagar mensagens do bot  |

### Administração de Dono

| Apenas Dono do Bot  |              Recurso           |
| :------------: | :---------------------------------------------: |
|       ✅        |   Entrar em um grupo                 |
|       ✅        |   Sair de todos os grupos                  |
|       ✅        |   Limpar todos os chats              |
|       ✅        |   Broadcast - Anuncio Geral                     |
|       ✅        |   Bloquear/Desbloquear usuário                     |
|       ✅        |   Sistema de Tipos de Usuários        |
|       ✅        |   Limitador comandos diários (por usuário)            |
|       ✅        |   Limitador de comandos por minuto (por usuário)          |
|       ✅        |   Limitador de mensagens privadas (Anti-flood)    |
|       ✅        |   Auto Sticker Privado   |
|       ✅        |   Anti Trava Privado   |
|       ✅        |   Sair do grupo                     |
|       ✅        |   Limpar somente chat de contatos                 |
|       ✅        |   Obter lista de usuários bloqueados                |
|       ✅        |   Modificar status atual do bot                |

<br>