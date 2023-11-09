# Metodologia da reportagem "Em São Paulo, falta de luz na periferia é até 8 vezes mais frequente que em áreas centrais"

## Dados
* Os dados de “[Interrupções de Energia Elétrica nas Redes de Distribuição](https://dadosabertos.aneel.gov.br/dataset/interrupcoes-de-energia-eletrica-nas-redes-de-distribuicao)” foram baixados do Portal de Dados Abertos da Agência Nacional de Energia Elétrica (ANEEL) no dia 8 de novembro de 2023. O arquivo pode ser consultado aqui;
* A localização dos conjuntos de unidades consumidoras foram exportados no [Portal de Dados Geográficos](https://dadosabertos-aneel.opendata.arcgis.com/) da ANEEL. Selecionamos apenas os dados do ano de [2022](https://dadosabertos-aneel.opendata.arcgis.com/datasets/6422007586134edf8b3504a456072ff0/about);
* Os dados georreferenciados dos [distritos](http://dados.prefeitura.sp.gov.br/pt_PT/dataset/distritos) de São Paulo foram obtidos no Portal de Dados Abertos da Prefeitura do município;

## Análise
* Os arquivos georreferenciados de distritos de São Paulo e de conjuntos de unidades consumidoras foram sobrepostos utilizando o software QGIS;
* Em seguida, inserimos os indicadores de continuidade (DEC e FEC) no mapa, nas camadas sobrepostas;
* Um conjunto pode abastecer diferentes distritos do município e cidades vizinhas, bem como um distrito pode ser atendido por mais de um conjunto de unidades consumidoras. Levamos em consideração essa definição durante a análise: incluímos os dados de indicadores de DEC e FEC por conjunto de unidades consumidoras que atendem distritos de São Paulo. Se um conjunto da Enel não atende o município, ele foi desconsiderado; se atende um distrito, mas atende outras cidades e distritos vizinhos, ele foi considerado.
