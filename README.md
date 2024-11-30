# Predição de Dados Binários

O objetivo principal deste projeto é transformar a variação diária de um ativo financeiro em um dado binário (0 ou 1) e, com base nisso, aplicar um modelo de machine learning (modelo X) para prever essa informação. Para alcançar esse objetivo, os dados são deslocados temporalmente, permitindo que a variação do dia atual seja utilizada para prever o comportamento do ativo no dia seguinte .

Um dos pilares do projeto é o processo de feature engineering, que envolve a criação de variáveis explicativas projetadas para capturar os fatores que influenciam o movimento do preço no próximo dia. A eficácia da estratégia é medida por meio de métricas estatísticas, que proporcionam uma análise objetiva e precisa dos resultados.

Além disso, este projeto serve como alicerce para abordagens mais avançadas, focadas na otimização e na identificação das features com maior poder preditivo. Ele também permite avaliar a viabilidade prática da estratégia, levando em consideração aspectos fundamentais como a eficiência na execução e a alocação de capital necessária para sua implementação.

# Acesso ao Script

1. Instalação das bibliotecas 
    ```bash
    python -m pip install -r https://raw.githubusercontent.com/rianlucascs/predicao-dados-binarios/master/requirements.txt
    ```

2. Acessar os dados
    ```python

    import requests

    response = requests.get('https://raw.githubusercontent.com/rianlucascs/predicao-dados-binarios/master/api.py')

    exec(response.text, globals())

    # Indicado para consultas rápidas
    Market = MarketBehaviorForecaster('^BVSP', features=[1, 2], start='2012-05-11', end='2022-05-11', step_size=None).run_forecast()

    # Indicado para processos de otimização
    Market = MarketBehaviorForecasterLocal('^BVSP', features=[1, 2], start='2012-05-11', end='2022-05-11', step_size=None).run_forecast_local()
    ```


# Gráficos (Saídas)

![image](https://github.com/user-attachments/assets/7035df8f-b917-4280-ac62-efa7a1ab84ee)
![image](https://github.com/user-attachments/assets/e29f78e9-bdac-4fa4-9f3f-6fcdae1bf251)
![image](https://github.com/user-attachments/assets/3c12d30c-da16-4ebd-8024-8a1f7a4522c7)
![image](https://github.com/user-attachments/assets/00b4c505-8ccb-4bed-836b-c9fb051d522d)
![image](https://github.com/user-attachments/assets/0dd0d455-861d-4a6a-8b34-51596642dd1b)
![image](https://github.com/user-attachments/assets/2ae0e43e-2b88-43d2-9faf-71e879dd7a45)
![image](https://github.com/user-attachments/assets/7353ff3b-2049-4f7e-b34c-e7a7e52bc507)
![image](https://github.com/user-attachments/assets/9c84609e-caa6-4ecb-9661-e67d76781227)
![image](https://github.com/user-attachments/assets/1b8af7ea-8e2a-49b7-bcaa-64168352e0c2)
![image](https://github.com/user-attachments/assets/4c4d71d1-8865-4221-8cc7-c6b967e2ccc3)
![image](https://github.com/user-attachments/assets/f5e39d97-4ec9-44c0-8cfb-56a32c485976)
![image](https://github.com/user-attachments/assets/a89904cf-b2af-4eb7-9552-fa944d2d3155)
![image](https://github.com/user-attachments/assets/b249b685-12ed-49a4-b75f-2768c0623576)
![image](https://github.com/user-attachments/assets/94933d03-b5fa-4048-81e1-c59a34b13c05)
![image](https://github.com/user-attachments/assets/915f090a-29e1-4754-a53d-839ceb9f70b0)
![image](https://github.com/user-attachments/assets/0bdc64d6-8d7a-4c3c-86b7-03589bf2ae3b)
![image](https://github.com/user-attachments/assets/d3638744-0e5a-4406-b8f9-72ffa05597d2)
![image](https://github.com/user-attachments/assets/88069ef3-8426-4be4-a117-73727bfe925e)
![image](https://github.com/user-attachments/assets/0d9428a9-2279-424a-9e6f-2acf9e8830d8)
![image](https://github.com/user-attachments/assets/36b3ed5b-f1a8-4be8-bed8-28385134c0cc)
![image](https://github.com/user-attachments/assets/c3528b7f-81d7-4e56-ae25-2e370477f093)
![image](https://github.com/user-attachments/assets/0d96bdc5-fbf9-4a75-9481-cf3eef0f9ac3)
![image](https://github.com/user-attachments/assets/7096a07b-fb19-447d-a70f-795f5028a1bc)
