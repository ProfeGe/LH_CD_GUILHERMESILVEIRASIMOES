# LH_CD_GUILHERMESILVEIRASIMOES
Entregas para Desafio Tecnico Lighthouse

No terminal, deverá ser digitado o comando abaixo


    import pandas as pd
    from sklearn.linear_model import LinearRegression
    import numpy as np
    import pickle
        with open('predicao_apt_LH_CD_Guilherme_Silveira_Simoes.pkl', 'rb') as f:
            models = pickle.load(f)


Para precificação, deverá colocar, na predição, qual o Room_type (no exemplo, 'Entire home/apt')
Colocando, os dados, na ordem: Latitude, Longitude, Disponibilidade Ano, Calculado Host, Reviews por Mês
Ex:

    apartamentoTeste = np.array([[40.7128, -74.0060, 355, 2, 0.38]])

Para precificação, deverá colocar, na predição, qual o Room_type (no exemplo, 'Entire home/apt')

    predicao_apt = models['Entire home/apt'].predict(apartamentoTeste)
    print(f"Preço previsto para 'Entire home/apt': {predicao_apt[0]}")

O valor resultado deverá ser

    Preço previsto para 'Entire home/apt': 327.4777603868133
