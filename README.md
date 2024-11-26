### Desafio Final de Power BI: E-commerce de Bebidas Ambev

Você é contratado como analista de dados para o e-commerce de bebidas da Ambev. Sua missão é criar um painel interativo que ajude os gestores a tomar decisões estratégicas com base nos dados fornecidos.

#### **Objetivo Geral:**
Criar um relatório completo no Power BI que combine **ETL no Power Query (M)**, **relacionamento entre tabelas**, **cálculos avançados com DAX** e **visualizações interativas**.

---

### **Tarefas do Desafio**

#### **ETL com M**
1. **Carregar os dados**:
   - Importe os arquivos CSV fornecidos (Produtos, Clientes, Pedidos, ItensPedido e Estoque) para o Power BI.
   
2. **Limpeza e transformação**:
   - Crie uma **coluna calculada** no Power Query que agrupe os produtos por categoria, somando o valor total de vendas por categoria.
   - Crie uma **coluna personalizada** para classificar os clientes com base no valor total dos pedidos:
     - **Regular**: Valor total de pedidos inferior a R$500.
     - **VIP**: Valor total de pedidos superior a R$500.

3. **Conexões externas**:
   - Simule um dado externo no Power Query, criando uma tabela manual com as metas de vendas por categoria:
     - Exemplo:
       | Categoria     | Meta de Vendas (R$) |
       |---------------|---------------------|
       | Cerveja       | 50,000             |
       | Refrigerante  | 30,000             |
       | Água          | 10,000             |

#### **Relacionamento entre tabelas**
- Crie relacionamentos entre as tabelas com base nas chaves primárias e estrangeiras:
  - **Pedidos** e **ItensPedido** (ID_Pedido)
  - **ItensPedido** e **Produtos** (ID_Produto)
  - **Pedidos** e **Clientes** (ID_Cliente)

---

#### **Funções com DAX**
1. **Métricas principais**:
   - Crie uma medida chamada `Total Vendas` que soma os valores totais das vendas:
     
   - Crie uma medida para calcular a **média de vendas por pedido**:
    
   - Crie uma medida que calcule o **estoque total disponível**:
    

2. **KPI (Indicadores-Chave de Desempenho) de metas**:
   - Crie uma medida que mostre se as vendas de cada categoria atingiram a meta:
     

3. **Análise de clientes**:
   - Crie uma coluna calculada para classificar clientes como:
     - **Alta Frequência** (mais de 5 pedidos)
     - **Baixa Frequência** (5 pedidos ou menos)
    

---

#### **Gráficos e Visualizações**
1. **Gráficos obrigatórios**:
   - **Gráfico de barras**: Total de vendas por categoria.
   - **Gráfico de linhas**: Evolução de vendas por mês.
   - **Gráfico de pizza**: Distribuição das categorias mais vendidas.
   - **Cartões**:
     - Total de vendas.
     - Total de clientes.
     - Estoque total disponível.

2. **Filtros e interatividade**:
   - Adicione slicers para permitir a seleção por **ano**, **categoria de produto**, e **tipo de cliente** (Regular ou VIP).
   - Crie uma tabela interativa que mostre os **produtos mais vendidos** com suas respectivas categorias e valor total de vendas.

---

#### **Entrega Final**
Seu relatório deve incluir:
- Um painel inicial com os principais KPIs (Indicadores-Chave de Desempenho) .
- Uma aba detalhada para análise de produtos.
- Uma aba para análise de clientes e desempenho.
