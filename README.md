# prefered_games_sim
Implementação de Teste A/B em Simulador de Preferências de Jogos

## Relatório de Resultados do Teste A/B

## Introdução

Este relatório descreve a implementação, execução e análise de um teste A/B realizado em um conjunto de dados simulados de usuários e jogos. O objetivo do teste A/B foi observar o impacto de uma alteração específica no tempo médio de jogo de um dos jogos ("Jogo A") sobre a escolha dos usuários.

## Classes e Estruturas de Dados

### Classe `Usuario`

A classe `Usuario` representa um usuário com as seguintes propriedades:
- `idade`: a idade do usuário.
- `genero`: o gênero do usuário.
- `preferencias_genero`: uma lista de gêneros de jogos preferidos pelo usuário.
- `tempo_medio_jogo`: o tempo médio que o usuário joga por dia.

### Classe `Jogo`

A classe `Jogo` representa um jogo com as seguintes propriedades:
- `nome`: o nome do jogo.
- `genero`: o gênero do jogo.
- `faixa_etaria`: a faixa etária recomendada para o jogo.
- `tempo_medio_jogo`: o tempo médio necessário para completar o jogo.

### Função de Escolha de Jogo
A função escolher_jogo seleciona aleatoriamente um jogo preferido para um usuário, com base nas preferências de gênero do usuário.

## Implementação do Teste A/B

### Aplicação da Alteração
A função aplicar_teste_ab altera o tempo médio de jogo do "Jogo A" de 40 minutos para 60 minutos.

### Coleta de Dados
A função coletar_dados_teste_ab coleta as escolhas dos usuários antes e depois da alteração.

### Análise dos Resultados
A função analisar_resultados conta as escolhas dos jogos antes e depois da alteração.

### Função Principal
A função main executa o teste A/B, coleta os dados, realiza a análise e gera o relatório.

Este relatório documenta o processo de realização de um teste A/B para avaliar o impacto da alteração do tempo médio de jogo do "Jogo A" sobre a escolha dos usuários. Através da coleta de dados antes e depois da alteração e da análise dos resultados, foi possível observar a variação nas escolhas dos usuários, permitindo uma compreensão mais aprofundada do impacto dessa alteração.
