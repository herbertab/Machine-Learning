# Previsão de Churn utilizando deep learning

## Descrição
Este projeto se concentra na previsão de churn de clientes por meio de um modelo de aprendizado de máquina. Utiliza-se um conjunto de dados que inclui informações de clientes e suas transações.

## Etapas Realizadas
1. **Pré-processamento dos Dados:**
   - Identificação do intervalo de tempo entre a primeira e última compra de cada cliente.
   - Cálculo do número de vendas por cliente, itens únicos, descontos utilizados e outras métricas relevantes.
   - Estabelecimento de uma data de referência para identificar clientes propensos ao churn.

2. **Engenharia de Features:**
   - Criação de novos atributos, como frequência de pedidos, taxa de uso de cupons, média de itens por pedido, entre outros.

3. **Preparação dos Dados:**
   - Remoção de colunas desnecessárias.
   - Codificação de rótulos para atributos não numéricos.
   - Divisão do conjunto de dados em treino e teste.

4. **Modelagem:**
   - Implementação de uma rede neural com diferentes configurações de topologia, learning_rate e otimizadores.
   - Utilização de pesos para lidar com o desbalanceamento das classes.
   - Ajuste nos pesos das classes para melhorar o recall da classe de churn.

## Resultados
O ajuste nos pesos das classes proporcionou melhorias na detecção de churn:
- **Peso 1.3:** Recall da classe 1 (churn) subiu para 68%.
- **Peso 2.0:** Recall da classe 1 atingiu 78%, mas houve uma pequena queda na acurácia (66%).

## Conclusão
Os ajustes nos pesos das classes impactaram diretamente na capacidade do modelo em identificar clientes propensos ao churn. Ao elevar os pesos da classe de churn, o modelo aprimorou consideravelmente a detecção de verdadeiros positivos, embora tenha havido uma leve diminuição na acurácia.
