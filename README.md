Football Match Conversation App
Este projeto implementa uma aplicação interativa em Streamlit que permite aos usuários conversar sobre partidas de futebol, consultar detalhes de competições, partidas, e jogadores, além de interagir com um agente de IA para obter respostas e análises relacionadas ao futebol.

Tecnologias Utilizadas
Streamlit: Framework para criar aplicações web interativas com Python.
Langchain: Biblioteca para desenvolvimento de agentes de IA conversacionais.
Football Stats API: Para buscar dados de competições e partidas de futebol.
Google Cloud API: Para configurar credenciais de acesso à API de inteligência artificial.
Plotly: Para visualização de dados.
Funcionalidad

1. Seleção de Competição, Temporada e Partida
A aplicação permite que os usuários escolham uma competição, temporada e partida específica a partir de uma lista de opções disponíveis, carregadas dinamicamente a partir da API de dados de futebol.

2. Interação com um Agente de IA
Após selecionar uma partida, os usuários podem conversar com um agente de IA para obter respostas relacionadas à partida, como estatísticas, jogadores, comentários especializados, e muito mais. O agente pode responder em diferentes estilos, como humorístico, formal ou técnico.

3. Perfil do Jogador
A aplicação oferece a possibilidade de pesquisar o perfil de um jogador, fornecendo informações detalhadas sobre o desempenho e estatísticas do jogador na partida selecionada.

4. Comentários de Especialistas
O agente também pode fornecer comentários especializados sobre a partida selecionada, com base nas informações da partida e nas estatísticas dos jogadores.

5. Armazenamento de Histórico de Conversa
A aplicação armazena o histórico de conversa entre o usuário e a IA, permitindo consultas subsequentes sobre as interações passadas.

Como Rodar a Aplicação
Pré-requisitos
Python 3.8 ou superior
Bibliotecas:
streamlit
langchain
plotly
football_stats (API de dados de futebol)
google-cloud (para configuração do Google Cloud)
langchain_community


Estrutura do Código
Configuração Inicial:

Definindo variáveis de ambiente para autenticação do Google Cloud.
Configuração do Streamlit (título, layout, etc.).
Funções de Carregamento de Dados:

Funções para carregar competições, temporadas, partidas e perfis de jogadores, utilizando dados da API de futebol.
Memória de Conversa:

A aplicação usa o ConversationBufferMemory da biblioteca Langchain para armazenar e recuperar o histórico de conversa.
Seleção e Exibição:

Os usuários selecionam uma competição, temporada e partida via barra lateral no Streamlit. As informações da partida selecionada são exibidas, junto com a possibilidade de interagir com o agente de IA.
Processamento de Respostas da IA:

A IA gera respostas com base na entrada do usuário, podendo fornecer análises, comentários especializados e informações estatísticas.


