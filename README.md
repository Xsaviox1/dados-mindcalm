# Escolha dos Datasets

Nosso grupo optou por abordar um tema relacionado ao nosso projeto de mobile. Nosso aplicativo fornece ao usuário  ferramentas e técnicas para ajudá-lo a lidar com questões diárias relacionadas à saúde mental, melhorando assim sua qualidade de vida.  Selecionamos então o conjunto de dados da Wellcome e OMS sobre saúde mental.

# Datasets escolhidos

## Wellcome 

A Wellcome reuniu informações e dados em todo o mundo acerca das:

1. Percepções globais sobre a importância da saúde mental para o bem-estar geral.

2. Percepções globais sobre o papel da ciência na compreensão da saúde mental e na descoberta de soluções para a ansiedade e a depressão.

3. Diferentes abordagens que as pessoas com ansiedade ou depressão em todo o mundo utilizam para gerir a sua ansiedade ou depressão e a utilidade percebida dessas abordagens.

O questionário foi aplicado a um mínimo de 1000 pessoas em cada um dos 113 países incluídos. Este conjunto de dados apresenta alto nível de abrangência e detalhamento.

## OMS

-   **Atlas Global de Saúde Mental**
-   **Pesquisa Mundial de Saúde sobre Saúde Mental**
-   **Taxas de Suicídio por País**
-   **Prevalência de Transtornos de Depressão e Ansiedade**
-   **Disponibilidade de Serviços de Saúde Mental**
-   **Saúde Mental e Abuso de Substâncias**
-   **Leitos Psiquiátricos e Força de Trabalho em Saúde Mental**
-   **Psicólogos per capta**



# Analise exploratória inicial

### Wellcome

As principais limitações do Wellcome Global Monitor são:

-   Não foram fornecidos mais detalhes sobre o que foi entendido por ansiedade ou depressão aos entrevistados
-   O enfoque da pesquisa são os sentimentos de ansiedade ou depressão conforme definido na pesquisa e algumas pessoas podem ter se sentido desconfortáveis em algumas perguntas
-   Decisões relativas à exclusão de certos regiões em alguns países devido a fatores como agitação política, conflito ou afastamento.
-   Decisões relativas a quais idiomas foram usado para realizar a pesquisa em países com dezenas, centenas ou mesmo milhares de idiomas.
-   A decisão de entrevistar pessoas com 15 anos de idade ou mais velhos e a exclusão de institucionalizados segmentos da população.
-   COVID e telefone

Margem de erro:

Ao interpretar os resultados dos inquéritos, todos os inquéritos por amostragem estão sujeitos a vários tipos de erros potenciais. Por exemplo, podem ocorrer erros devido a não respostas (quando os entrevistados seleccionados nunca são contactados ou recusa em participar), erros administrativos dos entrevistadores (onde uma resposta pode ser digitada incorretamente ou mal interpretada por um entrevistador) ou respostas incompletas ou imprecisas dadas pelo entrevistado.

O desenho amostral empregado neste estudo foi utilizado para produzir estimativas imparciais da população-alvo declarada. Uma amostra imparcial terá as mesmas características e comportamentos da população total da qual foi extraída. Por outras palavras, se tivermos uma amostra adequadamente desenhada, podemos fazer afirmações sobre a população-alvo dentro de um intervalo específico de certeza. Erros de amostragem podem ser estimados e o nível deles 'podem ajudar a interpretar os resultados finais dos dados. A dimensão desses erros de amostragem depende em grande parte do número de entrevistas e da complexidade do desenho amostral.

A margem de erro (MOE), ou o nível de precisão que é possível utilizar ao estimar a proporção desconhecida da população ‘P’, pode ser derivado utilizando a seguinte fórmula*:

MOE = 1,96 * √(P*(1-P)/n)

onde ‘n’ é o tamanho da amostra (ou seja, o número de pesquisas concluídas). Mesmo se a suposição mais conservadora (P = 0,5) for usada, o MOE para um tamanho de amostra de 1.000 será de 1,96 * √(0,25/1000) = 3,1 pontos percentuais sob a suposição usada na amostragem aleatória simples. 

### OMS

Este conjunto de dados reúne indicadores de metadados de diversas organizações de saúde global, abordando temas cruciais da saúde mental em escala mundial. Ele oferece uma visão abrangente sobre recursos, políticas e condições relacionadas à saúde mental em diferentes países, permitindo uma análise detalhada das seguintes áreas:

O Atlas Global de Saúde Mental proporciona uma compreensão profunda dos recursos disponíveis e das políticas implementadas para o suporte à saúde mental. A pesquisa mundial de saúde mental amplia essa visão ao fornecer dados quantitativos e qualitativos sobre condições de saúde mental e práticas de tratamento em diferentes regiões.

As taxas de suicídio por país são analisadas para identificar tendências e variações significativas, enquanto a prevalência de transtornos de depressão e ansiedade oferece insights sobre a distribuição global dessas condições críticas.

A disponibilidade de serviços de saúde mental é um aspecto crucial abordado pelo conjunto de dados, destacando desigualdades e lacunas na acessibilidade aos serviços. Além disso, a interseção entre saúde mental e abuso de substâncias é examinada para entender melhor os desafios associados a essas condições coexistentes.

Informações sobre leitos psiquiátricos e a força de trabalho em saúde mental revelam a capacidade de resposta dos sistemas de saúde em lidar com crises e demandas emergentes. Por fim, a análise da proporção de psicólogos por capita em diferentes países oferece uma medida da disponibilidade de profissionais treinados para oferecer suporte psicológico adequado à população.

Este conjunto de dados é uma ferramenta essencial para pesquisadores, formuladores de políticas e profissionais de saúde interessados em promover melhorias significativas na saúde mental global. Ao consolidar esses indicadores em uma única fonte acessível, ele facilita a identificação de áreas críticas de intervenção e a implementação de estratégias eficazes para mitigar os desafios enfrentados pelas comunidades em todo o mundo.

### Dimensões

Wellcome - 119000 linhas e 89 colunas

Psicólogos per capta - 120 linhas e 34 colunas

Atlas Global de Saúde Mental - 6420 linhas e 8 colunas

Pesquisa Mundial de Saúde sobre Saúde Mental - 6840 linhas e 8 colunas

Taxas de Suicídio por País - 22 linhas e 4 colunas

Prevalência de Transtornos de Depressão e Ansiedade - 22 linhas e 9 colunas

Disponibilidade de Serviços de Saúde Mental - 26 linhas e 6 colunas

Saúde Mental e Abuso de Substâncias - 10 linhas e 7 colunas

Leitos Psiquiátricos e Força de Trabalho em Saúde Mental 15 linhas e 4 colunas

# Tratamento de dados
### Wellcome
O tratamento da Wellcome foi focado em três pontos:
##### Na coluna EMP_2010
Aqui é identifico um padrão em Poland onde apenas neste pais teve resultado nulo, assim é identificado que foi um problema na distribuição interna do questionário.
Para solucionar este problema identificamos que a maior parte da população trabalha no formato 
Full-time e a partir disso, vamos supor que estes outros 10 também trabalhem desta forma.

##### Muitos dados nulos 
Isso de primeira vista parece deixar o Dataset inutilizável mas olhando melhor o dicionário podemos ver que existem questões que levam a outra, por exemplo, quem respondeu que possui ansiedade vai também responder de qual maneira ela trata a sua ansiedade, logo quem não respondeu terá muitas colunas nulas.

##### Muitos campos com objetos, string e float desordenados
Visto que é um dicionário e não importa como vai ser respondido para fins de pesquisa, não é um problema da parte de quem realizou mas do ponto de vista de quem vai analisar os dados isso é um problemas pois é muito fácil se perder em dados variados por isso eles ficarão por padrão como inteiro.

### OMS
O tratamento da Wellcome foi focado em dois pontos:
##### Na coluna Code
Isso de primeira vista parece que o Dataset é estranho pois tem muitos campos nulos mais vemos no dicionario que Code significa um código para o pais  porem nem tudo salvo ali são países, o Dataset também salva regiões como por exemplo, Africa, America do Sul, Leste Europeu e etc; e isso realmente não tem uma sigla correta como por exemplo, Brasil - 'BR', Estados Unidos - 'EUA'.
##### Colunas nulas
No Dataset ***Psicólogos per Capta***  é possível notar que existem muitas colunas com todos os seus dados nulos, o que torna ela completamente inútil, por este motivo serão dropadas.

# Insights 
#### Faixa etária
Com essa informação podemos ter uma persona mais bem embasada e direcionar melhor os conteúdos visando atingir um público mais especifico.

#### Porcentagem de Pessoas ansiosas nas redes sociais
Notando que a esmagadora maioria das pessoas ansiosas utilizam as redes sociais, podemos identificar um local ideal para direcionar o marketing do aplicativo para atingir o público, evitando desperdício de capital em outras mídias que trariam menos pessoas.

#### Porcentagem de pessoas ansiosas 
Ao vender o aplicativo a uma empresa temos o marcante número que 30% da população brasileira é ansiosa e se no futuro pretendermos migrar para outro pais, poder localizar um local mais propicio.

#### Diferença entre homens e mulheres com ansiedade 
 É importante saber a maioria do público para poder focar melhor as propagandas e o conteúdo fornecido 
 
#### Psicólogos per capta
Como o aplicativo vai contar com psicólogos realizando os atendimentos é importante ter a noção do quantitativo profissional antes de iniciarmos os negócios.

#### População que sofre de baixa energia por ansiedade
Como o aplicativo será vendido para empresas, poder mostrar o quanto a ansiedade afeta a empresa e a saúde dos funcionários é importante na hora de mostrar os benefícios na hora de adotar o MindCalm.

#### População que sofre de falta de sono por ansiedade
Como o aplicativo será vendido para empresas, poder mostrar o quanto a ansiedade afeta a empresa e a saúde dos funcionários é importante na hora de mostrar os benefícios na hora de adotar o MindCalm.


# Utilização do Atlas
O Atlas foi conectado e usado de forma a manter os dados originais para ter uma consulta mais rápida do que precisar inserir diretamente os dados e por segurança pois como estão na nuvem eles não serão perdidos e nem destruídos por um tratamento errado.

# Arquivo requirements.txt
O arquivo guarda informação para a instalação do **pyspark** e o **pymongo** em versão que são compatíveis no momento da criação evitando problemas futuros de versão.

# Dicionário de Dados

### Abrange a maior parte das variáveis


![Parte 1](https://i.ibb.co/J3kxT6b/image.jpg)
#### ibb.co/J3kxT6b


![Parte 2](https://i.ibb.co/f0TX0zM/image.png)
#### ibb.co/f0TX0zM


![Parte 3](https://i.ibb.co/RhrDx24/image.png)
#### ibb.co/RhrDx24


![Parte 4](https://i.ibb.co/qyfSxn9/image.png)
#### ibb.co/qyfSxn9


![Parte 5](https://i.ibb.co/19T26J7/image.png)
#### ibb.co/19T26J7


![Parte 6](https://i.ibb.co/ykYfLQz/image.png)
#### ibb.co/ykYfLQz


![Parte  7](https://i.ibb.co/mhxjFzb/image.png)
#### ibb.co/mhxjFzb


![Parte 8](https://i.ibb.co/nL2WXgW/image.png)
#### ibb.co/nL2WXgW
