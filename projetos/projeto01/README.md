![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/cyclistic.png)




# Introdução
Seja bem-vindo ao estudo de caso da análise de compartilhamento de bicicletas da empresa Cyclist. Você trabalha para uma grande empresa ficcional chamada Cyclistic, juntamente com alguns membros importantes do time. Para responder algumas perguntas de negócio, siga os passos no processo de análise de dados: Perguntar, Preparar, Processar, Analisar, Compartilhar e Agir. 
Ao longo do caminho, as tabelas da Trilha do Estudo de Caso – incluindo perguntas orientadas e tarefas-chave - o ajudarão a permanecer no caminho certo.

<br>

### Cenário
Eu sou um analista júnior trabalhando na equipe de analistas de marketing da Cyclistic, uma empresa de compartilhamento de bicicletas em Chicago. O diretor de marketing acredita que o sucesso da empresa no futuro depende do aumento de membros anuais. No entanto, o time quer entender como ciclistas casuais e membros anuais utilizam as bicicletas da Cyclistic diferentemente. A partir desses insights, a equipe criará uma nova estratégia de marketing para converter ciclistas casuais para membros anuais.


<br>


## Personagens e time
- Cyclistic: Um programa de compartilhamento de bicicletas, que conta com mais de 5.800 bicicletas e 600 estações de acoplamento. Cyclistic se diferencia por também oferecer bicicletas reclináveis, triciclos manuais e bicicletas de carga, tornando o compartilhamento de bicicleta mais inclusivo para pessoas com deficiência e ciclistas que não podem usar bicicleta padrão de duas rodas. A maioria dos ciclistas optam por bicicletas tradicionais; em torno de 8% dos ciclistas usam opções de assistência. Os clientes da Cyclistic têm o costume de pedalar por lazer, mas algo em torno de 30% usam as bicicletas para ir ao trabalho todo dia.

- Lily Moreno: O diretor de marketing e o seu gerente. Moreno é responsável pelo desenvolvimento de campanhas e iniciativas para promover o programa de compartilhamento de bicicletas. Essas podem incluir email, mídias sociais, e outros canais.


<br>

## Sobre a empresa
Em 2016, a Cyclistic promoveu uma oferta bem-sucedida de compartilhamento de bicicletas. Desde então, o programa cresceu para uma frota de 5.824 bicicletas que são rastreadas geograficamente e bloqueadas em uma rede de 692 estações em Chicago. As bicicletas podem ser destravadas em uma estação e devolvidas em outra estação do sistema a qualquer momento.

Até agora, a estratégia de marketing da Cyclistic se baseava na conscientização geral e no apelo a amplos segmentos de consumidores. Uma abordagem que ajudou essas coisas se tornarem possíveis foi a flexibilidade de preços nos planos: passe de viagem única, passe de um dia inteiro e associações anuais. Clientes que compram passe de viagem única ou passe de um dia inteiro são associados como ciclistas casuais. Clientes que compram associação anual são membros da Cyclistic.

Os analistas de finanças concluíram que os membros anuais são muito mais lucrativos do que os ciclistas casuais. Embora a flexibilidade no preço ajude a Cyclistic a atrair mais clientes. Moreno acredita que aumentar o número de membros anuais é a chave para o crescimento no futuro. Mais do que criar uma campanha de marketing focada apenas em novos clientes. Moreno acredita que há uma oportunidade sólida em converter ciclistas casuais em membros. Ela notou que ciclistas casuais já estão cientes sobre o programa da Cyclistic e o escolheram para suas necessidades de mobilidade.

Moreno estabeleceu uma meta clara: __Projetar estratégias de marketing destinadas a converter ciclistas casuais em membros anuais.__ Para fazer isso, no entanto, o time precisa entender melhor como os membros anuais e ciclistas casuais se diferem, por que um ciclista casual se tornaria um membro, e como as mídias digitais podem afetar suas táticas de marketing. Moreno e seu time estão interessados em analisar os dados históricos de viagens de bicicleta e identificar tendências.

<br>
<br>
<br>

# Objetivos
### Perguntar
- 1. Formas que os membros anuais e ciclistas casuais utilizam as bicicletas da Cyclistc 
- 2. Por qual motivo os ciclistas casuais se tornariam membros anuais?
- 3. Como a Cyclistc poderia usar mídias digitais para influenciar ciclistas casuais a se tornarem membros?

 <br>
 
Moreno designou a você a primeira pergunta a ser respondida: Como os membros anuais e casuais utilizam as bicicletas de forma diferente?

<br>

Você produzirá um relatório com os seguintes resultados:
- 1. Uma descrição clara das tarefas de negócios
- 2. Uma descrição de todas as fontes de dados usadas
- 3. Documentação de qualquer limpeza ou manipulação dos dados
- 4. Um resumo da sua análise
- 5. Visualizações de apoio e principais conclusões
- 6. Top três recomendações baseadas nas suas análises

<br>
<br>


### Preparar

Use os dados históricos para analisar e identificar tendências. (Observação: os conjuntos de dados têm um nome diferente porque a Cyclistic é uma empresa fictícia. Para os fins deste estudo de caso, os conjuntos de dados são apropriados e permitirão que você responda às perguntas comerciais. Os dados foram disponibilizados pela Motivate International Inc. sob esta licença). Esses são dados públicos que você pode usar para explorar como diferentes tipos de clientes estão usando as bicicletas Cyclistic. Mas observe que as questões de privacidade de dados o proíbem de usar as informações de identificação pessoal dos ciclistas. Isso significa que você não poderá conectar as compras de passes aos números de cartão de crédito para determinar se os ciclistas casuais moram na área de serviço da Cyclistic ou se eles compraram vários passes individuais.

- 1. Onde os dados estão localizados?
   - [DIVVY TRIP DATA](https://divvy-tripdata.s3.amazonaws.com/index.html)

<br>

 
- 2. Como eles foram organizados?
  - Foram coletados 12 arquivos csv. Cada arquivo csv corresponde ao mês do ano. ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/import_csv.png)

<br>


- 3.  Há algum problema com viés ou credibilidade nesses dados?
  - A fonte de onde os dados foram coletados é confiável.  Todas as colunas correspondem umas às outras.

<br>

 
- 4. Como você está lidando com o licenciamento, privacidade, seguro e acessibilidade desses dados?
  - Nenhum único dado foi alterado. As informações como nomes e endereços não foram divulgadas, assim como o percurso do usuário.

<br>

 
- 5. Como você verificou a integridade dos dados?
  - Analisei todos os arquivos. Os que tiveram dados nulos ou duplicados foram removidos. ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/check_values.png) ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/show_values.png)

<br>


- 6. Como isso pode ajudá-lo a responder suas perguntas?
  - Após a concatenação, limpeza e manipulação dos dados, medidas de tendência central e dispersão irão ajudar a conseguir alguns insights após a análise. 

<br>

- 7. Há algum problema com os dados?
  - Dados nulos, faltantes e inconsistentes.
 
<br>

 ### Processamento

- 1. Quais ferramentas você escolheu e por quê?
  - Foi usado Python e Google Sheets para o armazenamento, concatenação, limpeza, análise e visualização dos dados.

<br>

- 2. Você garantiu a identidade dos dados?
  - Nenhum dado foi alterado ou modificado. Os valores duplicados, faltantes ou inconsistentes foram removidos. Dados com o tempo NEGATIVO de viagens com bicicletas também foram removidos.

<br>

- 3. Quais são os passos que você seguiu para garantir que seus dados estão limpos?
  - Os dados nulos, faltantes ou duplicados foram removidos.
 ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/prop_dataframe.png) 
![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/output_result.png)

<br>

 - Removendo valores nulos
   - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/drop_na.png)
   - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/post_drop_na.png)
 
 <br>
 
 - DataFrame após a remoção dos valores nulos
   - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/dataframe_na.png)

<br>
  
 - 4.  Como você pode verificar que seus dados estão limpos e prontos para serem analisados?
   - Fazendo buscas de dados duplicados, faltantes inconsistentes.

<br>
<br>

 ### Análise 
 - 1. Como você deve organizar seus dados para realizar uma análise sobre eles?
   - Com a conclusão dos dados inconsistentes, converti as colunas 'started_at' e 'ended_at' para datetime64[ns]
     - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/convert_code.png)
     - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/datetime.png)

<br>    

   - Após a conversão das tabelas 'started_at' e 'ended_at' para datetime64[ns], criei uma tabela chamada ‘ride_length’. Essa tabela mede a minutagem dos passeios de bicicleta subtraindo a tabela 'ended_at' pela tabela 'started_at'
     - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/ride_length_code.png)
     - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/ride_length_output.png)

<br>

  - Criei uma tabela chamada 'day_of_week', que basicamente é uma tabela que diz em qual dia da semana ocorreu o passeio.
    - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/day_of_week_code.png)
    - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/day_of_week_output.png)
   
<br>

  - Com todas as tabelas que necessitamos para a análise já criadas, resolvi ordernar os passeios por ordem crescente e descobri valores com dias negativos (-1); após identificar esses dados inconsistentes, resolvi removê-los e também remmovi viagens com uma minutagem menor que 1 minuto.
    - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/checking_code.png)

    - ### Antes
    - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/less_1_day_output.png)


    - ### Depois
    - ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/more_than_1_sec.png)
   
<br>
<br>

  - 2. Seus dados foram formatados corretamente?
    - Todos os dados foram corretamente formatados e tratados para a análise.

<br>
<br>

  - 3. Quais surpresas você descobriu nos dados?
```
Media do tempo de bicicleta por membro:
0 days 00:16:48.865997765

Máxima do do tempo de passeio:
1 days 01:09:22

Moda dos dias da semana:
0    Saturday

Name: day_of_week, dtype: object
```

<br>

```
Média por TIPO de membro:member_casual
casual   0 days 00:24:17.663328902
member   0 days 00:12:34.939364041
Name: ride_length, dtype: timedelta64[ns]
```

<br>

```
Totais usuários por TIPO de membro:member_casual
member    2661948
casual    1506113
Name: count, dtype: int64
```

<br>

![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/pizza_total_membro.png)
![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/pct_total_pizza.png)


<br>

```
A média de viagens feitas por dia semana
day_of_week
Friday      0 days 00:16:23.742431528
Monday      0 days 00:15:33.509199867
Saturday    0 days 00:20:42.221681871
Sunday      0 days 00:20:39.841482864
Thursday    0 days 00:14:48.170496050
Tuesday     0 days 00:14:28.754211349
Wednesday   0 days 00:15:00.878320665
Name: ride_length, dtype: timedelta64[ns]
```
![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/media_passeio_semana.png)

<br>
<br>

 - 4. Que tendências ou relações você encontrou nos dados?
  
```
day_of_week
Friday       593576
Monday       575485
Saturday     643778
Sunday       556125
Thursday     591823
Tuesday      579003
Wednesday    628271
Name: ride_length, dtype: int64
```
<br>

![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/quantidade_total_semana.png)

```python

# Separando o total de cada tipo de membro por dia da semana
ano_grupos = ano[['rideable_type','member_casual', 'day_of_week']].value_counts()
anos_gruposdf = pd.DataFrame(ano_grupos)
anos_gruposdf.groupby('member_casual')
anos_gruposdf_sorted = anos_gruposdf.sort_values(by=['member_casual'], ascending=False).reset_index()
anos_gruposdf_sorted_1 = anos_gruposdf_sorted.sort_values(by=['member_casual'])



# Criando uma coluna 'mes' correspondente com cada viagem por usuário
meses_ano = {
    1: 'Janeiro', 2: 'Fevereiro', 3: 'Março', 4: 'Abril',
    5: 'Maio', 6: 'Junho', 7: 'Julho', 8: 'Agosto',
    9: 'Setembro', 10: 'Outubro', 11: 'Novembro', 12: 'Dezembro'
}

ano['mes'] = ano['started_at'].dt.month.map(meses_ano)



#1.  Indexando os meses em ordem
#2. Criando o gráfico da quantidade de passeios ao longo do ano.


ano_mes_df = ano['mes'].value_counts().reset_index()
novo_indice = np.array([7,6,8,5,9,4,3,10,2,1,11,0])
ano_mes_df.index = novo_indice
ano_mes_df_1 = ano_mes_df.sort_index()
ano_mes_df_1.plot(kind='bar', x='mes', y='count', legend=False)
plt.xlabel('Meses')
plt.title('Quantidade de passeios ao longo do ano')
plt.show()

```
![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/mes_tendencia.png)
