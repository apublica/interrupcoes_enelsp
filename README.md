# interrupcoes_enelsp

* Os dados de “Interrupções de Energia Elétrica nas Redes de Distribuição” foram baixados do portal de dados abertos da ANEEL no dia 8 de novembro de 2023. Os dados podem ser consultados aqui;
* A localização dos conjuntos de unidades consumidoras foram exportados no portal de dados georreferenciados da ANEEL. Selecionamos apenas os dados do ano de 2022;
* Os dados georreferenciados dos distritos de São Paulo foram obtidos no portal de dados abertos da Prefeitura do município;
* Os arquivos georreferenciados de distritos de São Paulo e de conjuntos de unidades consumidoras foram sobrepostos utilizando o software QGIS;
* Em seguida, inserimos os indicadores de continuidade (DEC e FEC) no mapa, nas camadas sobrepostas;
* Um conjunto pode abastecer diferentes distritos do município e cidades vizinhas, bem como um distrito pode ser atendido por mais de um conjunto de unidades consumidoras. Levamos em consideração essa definição durante a análise: incluímos os dados de indicadores de DEC e FEC por conjunto de unidades consumidoras que atendem distritos de São Paulo. Se um conjunto da Enel não atende o município, ele foi desconsiderado; se atende um distrito, mas atende outras cidades e distritos vizinhos, ele foi considerado.
