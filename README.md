# 📈 Análise de Mercado Financeiro com Estratégia de Médias Móveis

Este projeto em Python realiza uma análise de desempenho da ação **ALPA4.SA** (Alpargatas) utilizando uma estratégia simples baseada em **médias móveis**, comparando-a com o retorno da própria ação e com o **Ibovespa (índice Bovespa)**.

## ⚙️ Tecnologias e Bibliotecas Utilizadas

- [yFinance](https://pypi.org/project/yfinance/) `0.2.58` - para obtenção de dados históricos do mercado financeiro.
- [Pandas](https://pandas.pydata.org/) - para manipulação de dados.
- [NumPy](https://numpy.org/) - para cálculos vetorizados.
- [Matplotlib](https://matplotlib.org/) - para visualização dos resultados.
- [mplcyberpunk](https://pypi.org/project/mplcyberpunk/) - para estilização dos gráficos com visual futurista.

## 📊 Estratégia

A lógica da estratégia é baseada no cruzamento de duas médias móveis:

- **Média Rápida:** 7 dias
- **Média Lenta:** 40 dias

### Regras:

- Se a média rápida ultrapassa a média lenta → **compra (posição = 1)**
- Se a média rápida fica abaixo da média lenta → **venda (posição = -1)**

Os retornos são calculados e acumulados tanto para:
- A estratégia
- A própria ação
- O índice Ibovespa

Esses dados são plotados em um gráfico comparativo.

## 📦 Instalação

Clone o repositório e instale os pacotes necessários:

```bash
pip install yfinance==0.2.58
pip install mplcyberpunk
