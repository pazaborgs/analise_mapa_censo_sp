# 🗺️ Análise Espacial: População e Domicílios em São Paulo (Censo 2022)

![Mapa do censo populacional de SP (2022)](capa.png "a Mapa do censo populacional de SP (2022)")

Este projeto realiza uma análise geoespacial exploratória dos dados do Censo Demográfico 2022 para o estado de São Paulo. O objetivo é visualizar a distribuição populacional e densidade domiciliar através de mapas coropléticos.

## 🛠️ Tecnologias Utilizadas
* **Python**
* **Pandas:** Manipulação e limpeza de dados (ETL).
* **Folium:** Visualização de mapas interativos (Leaflet.js).
* **Jupyter Notebook:** Ambiente de desenvolvimento.

## 📂 Fontes de Dados (Data Sources)

1.  **Resultados do Universo (População e Domicílios):**
    * Fonte: [IBGE - Censo Demográfico 2022](https://www.ibge.gov.br/estatisticas/sociais/populacao/22827-censo-demografico-2022.html?edicao=37225)

    * *Nota: Os dados foram tratados para agrupar setores censitários em municípios.*

2.  **Malha Geográfica (GeoJSON):**
    * Fonte: [tbrugz/geodata-br (GitHub)](https://github.com/tbrugz/geodata-br/tree/master)
    * Arquivo utilizado: `geojs-100-mun.json`
    * Licença: Creative Commons CC0 1.0 Universal (Domínio Público).

## 📊 Metodologia
1.  **Coleta:** Importação dos microdados do IBGE e da malha geográfica.
2.  **Limpeza:** Remoção de colunas auxiliares e filtragem exclusiva para o estado de SP (`NM_UF == 'São Paulo'`).
3.  **Transformação:** Agrupamento de dados por Código de Município (`CD_MUN`) e aplicação de escala logarítmica para suavizar a disparidade visual entre a capital e o interior.
4.  **Visualização:** Renderização de mapa coroplético com *tooltips* interativos.

---

[👉🏽 Desenvolvedor do Código](https://www.linkedin.com/in/patrickrgsanjos)