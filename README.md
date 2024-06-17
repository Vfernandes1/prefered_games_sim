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

---------------

# Mudanças Realizadas:

### Explicação das Alterações

**Geração de Dados Simulados:** A função gerar_dados_usuarios gera um conjunto maior de dados simulados de usuários para tornar a análise estatística mais relevante.

**Função para Calcular o p-valor:** A função calcular_p_valor agora usa um teste z para calcular o p-valor com base nas proporções das escolhas antes e depois da alteração. Isso fornece uma análise estatística mais precisa.

**Relatório de Resultados:** O relatório inclui os p-valores calculados para cada jogo, ajudando a avaliar a significância estatística das mudanças observadas.

Com as mudanças realizadas a análise é um pouco mais robusta e capaz de detectar variações estatisticamente significativas nas escolhas dos usuários após a alteração do tempo médio de jogo.

### Análise de Dados

Segmentação de Dados: A segmentação de dados não foi explicitamente incluída neste exemplo devido ao pequeno conjunto de dados. No entanto, em um cenário real, segmentaríamos os usuários por idade, gênero, ou outras características relevantes para observar como diferentes segmentos respondem à alteração.

Cálculo do Tamanho da Amostra: O tamanho da amostra é calculado com base na variância, margem de erro e z-score, mas no exemplo acima, usamos todos os dados disponíveis.

Execução do Teste A/B: A função aplicar_teste_ab modifica o atributo de interesse (tempo médio de jogo). A coleta de dados antes e depois da alteração permite a comparação.

Análise dos Resultados: Utilizamos o teste t para comparar as médias das escolhas antes e depois da alteração, calculando os p-valores para avaliar a significância das mudanças observadas.

## Relatório Final

### Design Experimental

O teste A/B foi desenhado para avaliar o impacto de aumentar o tempo médio de jogo do "Jogo A" nas escolhas dos usuários.

### Execução do Teste

**Coleta de Dados:** Coletamos as escolhas dos usuários antes e depois da alteração.

**Alteração Implementada:** O tempo médio de jogo do "Jogo A" foi alterado para 60 minutos.

**Análise dos Resultados**
A contagem de escolhas para cada jogo foi comparada antes e depois da alteração. Os p-valores foram calculados para determinar se as mudanças observadas foram estatisticamente significativas.

### Conclusões
Os resultados indicaram que não houve variação significativa nas escolhas dos usuários após a alteração, com p-valores acima do nível usual de significância (0.05). Isso sugere que a alteração no tempo médio de jogo do "Jogo A" não afetou significativamente as preferências dos usuários.

### Variáveis Confundidoras e Importância da Segmentação
É importante considerar variáveis confundidoras, como outras características dos usuários (idade, gênero, preferências específicas), que podem influenciar as escolhas. A segmentação de dados pode fornecer insights mais detalhados sobre como diferentes grupos de usuários respondem a mudanças específicas.






