# desafio-tempo-medio-entre-picos
O problema dos tempos médios foi dada e com a sugestão implícita de gerar gráficos para validar a solução proposta.
Logo, foi feito:
    1 - Código para implementar um gráfico de pontos aleatório
        *Foi usado uma API do google para implementar gráficos de pontos
        *Foi usado HTML, CSS e javascript puros para implementar a lógica visual e de processamento de dados
        *Os pontos gerados foram implementados usando a biblioteca matemática do javascript para criar pontos aleatórios (Math.random())
        *Usei a liberdade de observar o gráfico anterior do problema para gerar uma emulação de 70 segundos de pontos, para o problema, que pede um ponto para segundo, foram 70 pontos
    2 - Além de criar os pontos, gerar os gráficos, houve também:
        *A análise do problema, onde os picos reais só podem ser considerados se forem maiores que 50 e não tiverem picos anteriores maiores que os picos atuais, ou seja, os pontos sucessores e antecessores a esse pico precisam ser menores que 50 para ter garantia.
        *Transformação dos valores decimais de segundos para minutos e segundos, como pedido, usando a lógica de resto da divisão de inteiros por 60 para achar os segundos até no máximo de 59 e divisão do valor de segundos por 60, para achar a quantidade de minutos, caso resulte em resultados maiores que 1
        *por exemplo:
            - 120segundos => 120/60 = 2 minutos, 120%60 = 0 segundos, logo: 02:00