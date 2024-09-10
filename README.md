# Análise de Rentabilidade do CDI

Este projeto foi desenvolvido com o objetivo de analisar a rentabilidade do CDI ao longo do tempo, obtendo dados diretamente do Banco Central. A partir de 1994, foi criada uma calculadora de retorno, avaliando janelas de retornos e oferecendo insights sobre a lucratividade de diferentes períodos e condições.

## Questões Abordadas

**Questão 1: Cálculo de Lucro com SELIC**

O fundo mais lucrativo da principal empresa de gestão de ativos de Gotham City segue uma regra simples: o lucro é baseado no cálculo de juros compostos com a taxa SELIC. O desafio aqui é construir um programa que calcule o lucro total dado um valor inicial de capital e um período específico, respeitando as seguintes restrições:

- A data de início deve ser maior ou igual a 1995-01-01.
- A data de término deve ser posterior à data de início.
- A frequência do cálculo deve ser uma das seguintes: diária, mensal ou anual.

**Passos para a Solução:**
1. **Instalar e importar os módulos e bibliotecas necessárias.**
2. **Coletar dados do usuário:**
    - Capital inicial
    - Data de início
    - Data de término
    - Frequência do cálculo
3. **Tratar os dados coletados.**
4. **Obter dados da SELIC a partir do Banco Central.**
5. **Calcular o retorno do capital para o período fornecido.**

## Questão 2: Período Mais Lucrativo de 500 Dias

Dada a janela de tempo entre 2000-01-01 e 2022-03-31, a tarefa aqui é identificar qual foi o período mais lucrativo de 500 dias consecutivos.

**Passos para a Solução:**
1. **Filtrar os dados da SELIC para o período de interesse (2000-01-01 a 2022-03-31).**
2. **Calcular a rentabilidade em janelas de 500 dias.**
3. **Gerar o intervalo de datas dentro da tabela de cálculo.**
4. **Identificar o maior retorno dentro da tabela de períodos.**

##Tecnologias Utilizadas
- **Linguagem de Programação**: Python
- **Bibliotecas**:
  - `pandas` para manipulação e análise de dados, utilizada para processar e organizar os dados financeiros coletados.
  - `matplotlib` para criação de gráficos, utilizada para visualização dos resultados de rentabilidade ao longo do tempo.
  - `numpy` para operações matemáticas e manipulação de arrays, utilizada no cálculo de retornos e janelas de tempo.
  - `bcb` para coleta de dados financeiros diretamente do Banco Central, utilizada para obter as séries históricas da taxa SELIC.
  - `datetime` para manipulação de datas, utilizada para gerenciar as datas de início, término e intervalos de cálculo.
