# Sistema de Recomendação de Músicas com PySpark
Este projeto implementa um sistema de recomendação de músicas utilizando técnicas de processamento de dados em larga escala e aprendizado de máquina. O objetivo é fornecer recomendações de músicas com base em suas características, utilizando PySpark para gerenciar grandes volumes de dados.

## Funcionalidades
- Processamento de grandes volumes de dados de músicas.
- Normalização de dados com StandardScaler para padronizar as variáveis antes de aplicar o algoritmo.
- Redução de dimensionalidade com PCA (Principal Component Analysis).
- Agrupamento de músicas similares utilizando K-Means.
- Geração de recomendações baseadas na distância euclidiana entre as músicas.
- Visualização gráfica dos clusters e recomendações.

## Tecnologias Utilizadas
- **PySpark:** Biblioteca para processamento distribuído de dados.
- **StandardScaler:** Para normalização dos dados antes da clusterização.
- **PCA:** Técnica de redução de dimensionalidade para lidar com conjuntos de dados de alta dimensionalidade.
- **K-Means:** Algoritmo de clusterização para agrupar músicas semelhantes.
- **Plotly/Seaborn:** Para visualizações gráficas.

## Como Funciona
1. **Pré-processamento dos Dados:** Os dados das músicas são limpos e preparados para análise.
2. **Normalização dos Dados:** Utilizamos o StandardScaler para normalizar as variáveis, garantindo que todas estejam na mesma escala.
3. **Redução de Dimensionalidade:** Aplicamos PCA para reduzir o número de variáveis, mantendo as principais características dos dados.
4. **Clusterização:** Músicas similares são agrupadas usando o algoritmo K-Means.
5. **Recomendação:** Para uma música escolhida, o sistema recomenda músicas similares com base na distância entre os vetores de características.

## Como Executar o Projeto
1. Clone o repositório:
```
git clone https://github.com/headyschwi/spark_music_recommendation.git
```
3. Instale as dependências:
```
pip install -r requirements.txt
```
4. Execute o Jupyter Notebook `main.ipynb` para ver os resultados e gerar recomendações.

## Preview da Análise dos Dados
Semelhança entre gêneros musicais:
![newplot](https://github.com/user-attachments/assets/f75c81fd-60b9-4454-b56d-2b7375459fa5)

## Exemplo de Uso
```
recomenda("Lose Yourself")
```
![image](https://github.com/user-attachments/assets/411adf32-3d04-46c3-9d48-38aedf8d79de)

## Conclusão
Este projeto demonstra como aplicar técnicas de aprendizado de máquina e processamento distribuído de dados para construir um sistema de recomendação de músicas. O uso de PySpark e técnicas como StandardScaler para normalização e PCA para redução de dimensionalidade, combinado com a clusterização via K-Means, permite identificar e recomendar músicas semelhantes com eficiência.
