# PA - Power BI - Análise de Dados do Airbnb em New York (2011-2019)

## Descrição do Projeto

Este projeto tem como objetivo desenvolver uma análise crítica de dados do Airbnb sobre o mercado de locação de quartos na cidade de Nova York. O CEO da empresa *Tudo Aqui* solicitou um relatório no Power BI que contenha dois dashboards interativas, sendo uma com análises gráficas e outra com detalhes em forma de tabelas ou matrizes. Os dados utilizados são provenientes do conjunto de dados do Airbnb, que inclui informações de 2011 a 2019 para a cidade de Nova York.

Os dados podem ser acessados através do seguinte [link do Kaggle](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data).

## Objetivo

- Criar uma análise detalhada dos dados do Airbnb em Nova York.
- Organizar os dados para análise no Power BI.
- Implementar dois dashboards:
  1. **Dashboard Gráfico**: Análises visuais interativas.
  2. **Dashboard de Detalhes**: Informações detalhadas em formato de tabela ou matriz.
- Adicionar uma segmentação interativa com base na classificação de tipos de acomodação (Baixo Padrão, Médio Padrão, Alto Padrão, Altíssimo Padrão).

## Requisitos

### Colunas e Tipos de Dados

As colunas a serem analisadas e seus respectivos tipos de dados são:

| Coluna              | Tipo de Dados       |
|---------------------|---------------------|
| last_review         | Data                |
| id                  | Número Inteiro      |
| name                | Texto               |
| host_id             | Número Inteiro      |
| host_name           | Texto               |
| neighbourhood_group | Texto               |
| neighbourhood       | Texto               |
| latitude            | Número Decimal      |
| longitude           | Número Decimal      |
| room_type           | Texto               |
| price               | Número Decimal      |
| minimum_nights      | Número Inteiro      |
| number_of_reviews   | Número Inteiro      |

### Considerações

1. **Tratamento de Dados**:
   - Remover nulos, dados inconsistentes ou brancos.
   - Utilizar o recurso “remover erros” do Power Query para limpar os dados.
   - Testar cada coluna individualmente para garantir a importação correta dos dados.
   
2. **Cálculos e Transformações**:
   - **Preço Mínimo Final**: Preço por noite multiplicado pela quantidade mínima de noites.
   - **Classificação de Preços**:
     - "Baixo Padrão" para preço mínimo final ≤ R$1.000.
     - "Médio Padrão" para preço mínimo final > R$1.000 e ≤ R$10.000.
     - "Alto Padrão" para preço mínimo final > R$10.000 e ≤ R$100.000.
     - "Altíssimo Padrão" para preço mínimo final > R$100.000.
   - Organizar a segmentação de acordo com a classificação acima.
   
3. **Formatação de Dados**:
   - Garantir que todos os campos do tipo texto estejam em **maiúsculas**.
   
4. **Visualização**:
   - O tema do Power BI deverá ser **Bloom** (tema visual da empresa).
   - Incluir uma imagem de plano de fundo que remeta a viagens, criando um menu interativo.

5. **Tabela Calendário**:
   - Criar uma tabela calendário para análises temporais.

## Implementação

### 1. Preparação dos Dados
- **Importação e Transformação**: Utilize o Power Query para importar os dados e garantir que as colunas estejam no formato correto, removendo nulos e dados inconsistentes.
- **Criação de Tabela Calendário**: Desenvolva uma tabela calendário para análises temporais.

### 2. Cálculos
- **Criação de Coluna de Classificação de Preços**: Adicione uma coluna para classificar o preço mínimo final de acordo com a regra solicitada.

### 3. Dashboards
- **Dashboard Gráfico**: Utilize gráficos interativos, como gráficos de barras, linhas e dispersão, para analisar as tendências de preços e número de avaliações ao longo do tempo.
- **Dashboard de Detalhes**: Crie uma tabela ou matriz que exiba dados detalhados sobre as acomodações, incluindo preço, tipo de quarto, e número de avaliações.

### 4. Segmentação e Interatividade
- Adicione uma segmentação que permita aos usuários escolher a classificação de preço para filtrar os dados (Baixo Padrão, Médio Padrão, etc.).
- Crie um menu interativo com uma imagem de fundo relacionada a viagens.

## Conclusão

Este relatório foi desenvolvido para atender às necessidades do CEO e do Corpo Diretivo da *Tudo Aqui*, proporcionando uma análise clara e acessível dos dados de locação de quartos em Nova York, com foco na classificação de preços e tendências temporais.

---

## Tecnologias Utilizadas

- **Power BI**: Ferramenta principal para visualização e análise de dados.
- **Kaggle**: Fonte dos dados do Airbnb.
- **Power Query**: Utilizado para limpar e transformar os dados antes da análise.

---

## Como Utilizar

**Clone o Repositório**:
   - Para clonar o repositório e começar a trabalhar no projeto, execute:
   ```bash
   git clone https://github.com/seu_usuario/seu_repositorio.git
