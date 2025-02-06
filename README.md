# LH_CD_GUILHERMESILVEIRASIMOES
Entregas para Desafio Tecnico Lighthouse

No terminal, deverá ser digitado o comando abaixo

with open('predicao_apt_LH_CD_Guilherme_Silveira_Simoes.pkl', 'rb') as f:
    models = pickle.load(f)

Para precificação, deverá colocar, na predição, qual o Room_type (no exemplo, 'Entire home/apt')
Colocando, os dados, na ordem: Latitude, Longitude, Disponibilidade Ano, Calculado Host, Reviews por Mês

predicao_apt = models['Entire home/apt'].predict(apartamentoTeste)
