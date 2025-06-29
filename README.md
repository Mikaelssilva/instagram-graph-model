## __Instagram-graph-model__
Este projeto tem como objetivo modelar o Instagram como um grafo, utilizando dados de interações (seguidores, curtidas, comentários) para explorar padrões, comunidades e influenciadores dentro de uma rede social simulada. Através da aplicação de algoritmos clássicos de grafos e métricas da Ciência das Redes, buscamos entender a estrutura da rede e o comportamento dos usuários.

## __Recursos e Funcionalidades__
Modelagem de Rede Social: Representação de usuários (User), postagens (Post) e conexões (Conection) como um grafo.

Gerenciamento de Usuários e Conexões: Funcionalidades para adicionar/remover usuários e estabelecer/desfazer relações de seguimento.

Publicação de Postagens: Usuários logados podem criar e visualizar postagens.

## __Algoritmos de Grafo__

Busca em Largura (BFS - Breadth-First Search): Utilizado para encontrar os caminhos mais curtos entre usuários e para gerar recomendações de amizade (amigos de amigos).

Busca em Profundidade (DFS - Depth-First Search): Aplicado para explorar a profundidade das conexões e a acessibilidade entre os usuários.

Sistema de Recomendação: Um algoritmo inteligente que sugere novos usuários para seguir com base nas conexões existentes.

Métricas da Ciência das Redes: Cálculo e análise de importantes métricas para entender a estrutura e a dinâmica da rede, incluindo:

Grau dos Nós: Mede o número de conexões de entrada e saída de cada usuário.

Centralidade: Identifica os usuários mais influentes ou centrais na rede (ex: Centralidade de Grau, de Proximidade, de Intermediação).

Componentes Conectados: Identificação de subgrupos de usuários que estão conectados entre si.

Diâmetro da Rede: A maior distância (caminho mais curto) entre quaisquer dois nós na rede.

Visualização Interativa do Grafo: Representação gráfica da rede para destacar padrões, subgrupos e nós centrais (implementado com NetworkX e Matplotlib/Plotly).

Interface Gráfica de Usuário (GUI): Uma aplicação interativa desenvolvida com tkinter para facilitar a interação com a rede social, incluindo login, feed de postagens e visualização de recomendações.

## __Estrutura de Dados do Grafo__
A rede é modelada como um grafo direcionado onde:

Nós (Vértices): Representados pela classe User, contendo informações como nome de usuário e e-mail.

Arestas (Conexões): Representadas pela classe Conection, que define uma relação de "segue" de um User para outro. As arestas possuem pesos (n_interacoes), indicando o nível de interação entre os usuários.

Representação Interna: O grafo é armazenado na classe UniPoli utilizando uma combinação de um dicionário para os usuários (para acesso rápido aos nós) e uma lista de arestas (self.conections). Além disso, uma lista de adjacência (self.adj_list) é utilizada para otimizar as operações de busca e travessia do grafo.

## __Como usar__
Pré-requisitos: Certifique-se de ter o Python 3.x instalado em sua máquina.

Instalação das Bibliotecas: Instale as bibliotecas necessárias utilizando pip:

``Bash``

``pip install matplotlib networkx
(datetime e tkinter geralmente vêm com a instalação padrão do Python)``

## __Execução__

É preferível usar ambientes de notebooks Jupyter (.ipynb). Abra o arquivo instagram_graph.ipynb em um ambiente Jupyter (Jupyter Lab, Jupyter Notebook, VS Code com extensão Jupyter).

Execute todas as células do notebook sequencialmente. A interface gráfica (tkinter) será iniciada automaticamente.

Interaja com a GUI para criar usuários, fazer login, adicionar conexões, postar e visualizar recomendações e análises do grafo.

## __Autoria__
Esse projeto foi totalmente desenvolvido por Mikael Silva, aluno do curso de Engenharia da Computação da UPE.

## __Licença__
[Ver licença disponível](https://github.com/Mikaelssilva/Instagram-graph-model/blob/main/LICENSE)
