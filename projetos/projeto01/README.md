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

### Preparar

Use os dados históricos para analisar e identificar tendências. (Observação: os conjuntos de dados têm um nome diferente porque a Cyclistic é uma empresa fictícia. Para os fins deste estudo de caso, os conjuntos de dados são apropriados e permitirão que você responda às perguntas comerciais. Os dados foram disponibilizados pela Motivate International Inc. sob esta licença). Esses são dados públicos que você pode usar para explorar como diferentes tipos de clientes estão usando as bicicletas Cyclistic. Mas observe que as questões de privacidade de dados o proíbem de usar as informações de identificação pessoal dos ciclistas. Isso significa que você não poderá conectar as compras de passes aos números de cartão de crédito para determinar se os ciclistas casuais moram na área de serviço da Cyclistic ou se eles compraram vários passes individuais.

- 1. Onde os dados estão localizados?
   - [DIVVY TRIP DATA](https://divvy-tripdata.s3.amazonaws.com/index.html)
 
- 2. Como eles foram organizados?
  - Foram coletados 12 arquivos csv. Cada arquivo csv corresponde ao mês do ano. ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/import_csv.png)

- 3.  Há algum problema com viés ou credibilidade nesses dados?
  - A fonte de onde os dados foram coletados é confiável.  Todas as colunas correspondem umas às outras.
 
- 4. Como você está lidando com o licenciamento, privacidade, seguro e acessibilidade desses dados?
  - Nenhum único dado foi alterado. As informações como nomes e endereços não foram divulgadas, assim como o percurso do usuário.
 
- 5. Como você verificou a integridade dos dados?
  - Analisei todos os arquivos. Os que tiveram dados nulos ou duplicados foram removidos. ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/check_values.png) ![](https://github.com/EVERmathias/projetos_portifolio/blob/main/projetos/projeto01/imagens/show_values.png)












