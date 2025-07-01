# Análise Exploratória de Dados de Jogadores de Futebol

Este projeto realiza uma análise exploratória do desempenho de jogadores de futebol, usando métricas como gols, assistências, passes, desarmes e avaliação geral. Também tratamos dados faltantes, outliers e criamos novas métricas para auxiliar a análise.

---

## 1. Introdução

O objetivo é entender o desempenho dos jogadores através de variáveis estatísticas, verificando distribuições, relações e padrões importantes para avaliação.

---

## 2. Tratamento dos Dados

- Valores ausentes foram tratados, preenchendo com zeros ou médias conforme o caso.
- Colunas irrelevantes e duplicatas foram removidas.
- Outliers em colunas como "avaliação" e "gols" foram limitados para evitar distorções.
- Novas colunas foram criadas:  
  - `gols + assistências` (soma dos gols e assistências)  
  - `aproveitamento_passes` (taxa de passes precisos)

---

## 3. Distribuição da Avaliação dos Jogadores

![Distribuição da Avaliação](imagens_readme/hist_avaliacao.png)

Observamos que a avaliação dos jogadores segue uma distribuição que pode ser aproximada por uma curva normal, com maior concentração na faixa média.

---

## 4. Análise dos Gols

![Boxplot de Gols](imagens_readme/boxplot_gols.png)

O boxplot dos gols mostra a distribuição dos valores, permitindo identificar possíveis outliers e entender o comportamento da variável.

---

## 5. Relação entre Assistências e Gols

![Assistências vs Gols](imagens_readme/scatter_assist_gols.png)

O scatterplot evidencia uma correlação positiva entre assistências e gols, indicando que jogadores que marcam mais gols tendem a ter também mais assistências.

---

## 6. Conclusão

Este estudo inicial possibilita compreender melhor os dados e preparar o terreno para modelos preditivos e análises mais profundas.

---

## Como usar

Coloque a pasta `imagens_readme` na raiz do repositório para que os gráficos apareçam corretamente no README.

---

Qualquer dúvida ou sugestão, fique à vontade para abrir uma issue!

---

*Projeto desenvolvido por [Seu Nome]*
"""

path = "/mnt/data/README.md"
with open(path, "w", encoding="utf-8") as f:
    f.write(conteudo_readme)

path
