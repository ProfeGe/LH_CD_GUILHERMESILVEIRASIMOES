# LH_CD_GUILHERMESILVEIRASIMOES
Entregas para Desafio Tecnico Lighthouse

No terminal, deverá ser digitado o comando abaixo

import pickle

with open('predicao_apt_LH_CD_Guilherme_Silveira_Simoes.pkl', 'rb') as f:
    models = pickle.load(f)

import pandas as pd
from sklearn.linear_model import LinearRegression
import numpy as np


Para precificação, deverá colocar, na predição, qual o Room_type (no exemplo, 'Entire home/apt')
Colocando, os dados, na ordem: Latitude, Longitude, Disponibilidade Ano, Calculado Host, Reviews por Mês
Ex:
apartamentoTeste = np.array([[40.7128, -74.0060, 355, 2, 0.38]])

predicao_apt = models['Entire home/apt'].predict(apartamentoTeste)
