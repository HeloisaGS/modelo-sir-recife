# Simulação do Modelo SIR para Catapora (Varicela) em Recife

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16zVm627Bx279YjW1NW_hW4Vzxiu-hBra)

Este repositório contém a atividade prática desenvolvida para a disciplina de **Elementos de Epidemiologia Computacional**. O objetivo do projeto é modelar a dinâmica de transmissão da catapora (Varicela) na população do Recife utilizando o modelo compartimental SIR em linguagem R, explorando variações nos parâmetros de transmissibilidade ($\beta$) e recuperação ($\gamma$).

---

## 🎯 Questões da Atividade
1. Escolher uma doença arbitrária para ser estudada na cidade do Recife.
2. Utilizar o modelo SIR para modelar a doença (com simplificações necessárias).
3. Determinar os parâmetros iniciais que serão usados no modelo SIR e justificar a escolha.
4. Implementar o modelo SIR e determinar após quantos dias a doença atingirá o pico, exibindo o número de pessoas em cada compartimento ($S, I, R$) no pico.
5. Realizar pelo menos 6 variações nas taxas de contaminação e recuperação, apresentando os gráficos obtidos e comentando os resultados.
6. Identificar as lacunas ao utilizar esse modelo para a doença escolhida.

---

## 📌 Parâmetros Iniciais (Cenário Base)
* **População de Recife ($N$):** 1.588.376 (Estimativa IBGE 2025)
* **Infectados Iniciais ($I_0$):** 10 | **Suscetíveis Iniciais ($S_0$):** 1.588.366
* **Tempo Médio de Infecção ($D$):** 7 dias ($\gamma = 1/7 \approx 0,143$)
* **Número Básico de Reprodução ($R_0$):** 9 ($\beta = R_0 \cdot \gamma \approx 1,286$)

---

## 📊 Resultados do Pico Epidêmico
Com base na simulação do cenário base:
* **Dia do Pico:** 13 dias
* **Suscetíveis no Pico ($S$):** 113.594
* **Infectados no Pico ($I$):** 1.009.241
* **Recuperados no Pico ($R$):** 465.541

---

## 🛠️ Tecnologias e Pacotes Utilizados
* **Linguagem:** R
* **Pacotes:** `deSolve`, `ggplot2`, `reshape2`

---

## 📚 Fontes dos Dados
* [Ministério da Saúde - Guia de Varicela/Catapora](https://www.gov.br/saude/pt-br/assuntos/saude-de-a-a-z/c/catapora-varicela)
* [IBGE Cidades - Recife/PE](https://cidades.ibge.gov.br/brasil/pe/recife/panorama)
