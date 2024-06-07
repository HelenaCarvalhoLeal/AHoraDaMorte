# AHoraDaMorte
## Descrição
"A Hora da Morte" foi um projeto para a disciplina de Física Computacional, utilizando a linguagem Scilab, para calcular a quanto tempo o corpo está morto depois de ter sido encontrado.

O programa implementa a Lei do Resfriamento de Newton para estimar o tempo da morte de um corpo encontrado, dado algumas temperaturas e tempos observados. A Lei do Resfriamento de Newton descreve que a taxa de variação da temperatura de um corpo é proporcional à diferença entre a temperatura do corpo e a temperatura ambiente.

## Como funciona
O programa recebe como entrada a temperatura inicial do corpo, a hora em que o corpo foi encontrado, a temperatura ambiente e a temperatura do corpo uma hora após ser encontrado. Utiliza essas informações para calcular a constante de resfriamento 𝑘 e estima o tempo desde que o corpo morreu (tv) e a hora exata da morte (tf).

## Entradas
- Temperatura inicial do corpo (°C): Temperatura do corpo no momento em que foi encontrado.
- Hora que o corpo foi encontrado: Hora exata em que o corpo foi descoberto (em horas).
- Temperatura do ambiente (°C): Temperatura do ambiente em que o corpo foi encontrado.
- Temperatura do corpo após uma hora (°C): Temperatura do corpo uma hora após ter sido encontrado.

## Saídas
- Gráfico de Temperatura x Tempo: Um gráfico que mostra a variação da temperatura do corpo ao longo do tempo.
- Arquivo "Horadamorte.txt": Arquivo de texto contendo o tempo desde a morte (em minutos) e a hora estimada da morte.
