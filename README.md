# Comparador De Algoritmos 

<div align="right">
  🇧🇷 Português | <a href="./README-en.md">🇺🇸 English</a>
</div>
<br>

<div align="center">
  <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java"/>
</div>
<br>

Bem-vindo! Este repositório contém uma aplicação focada em comparar dois métodos clássicos para o desenho de retas em uma grade de pixels (rasterização). 

## 🎯 Objetivo

O objetivo principal deste projeto é demonstrar, na prática, as diferenças de implementação, desempenho e cálculo entre a equação matemática tradicional de uma reta e o algoritmo otimizado de Bresenham, muito utilizado em Computação Gráfica.

## 🧠 Entendendo os Algoritmos

### 1. Definição Geométrica (Abordagem Analítica)
Utiliza a equação fundamental da reta algébrica: 

$$y = m \cdot x + b$$

Onde $m$ é o coeficiente angular (calculado por $m = \frac{\Delta y}{\Delta x}$) e $b$ é a interseção com o eixo Y. 
* **Desvantagem computacional:** Este método exige cálculos contínuos com números de ponto flutuante (divisões e multiplicações) e arredondamentos para descobrir as coordenadas $(x, y)$ de cada pixel, o que é pesado e lento para o processador renderizar em tempo real.

### 2. Algoritmo de Bresenham
Criado em 1962, é um dos algoritmos mais importantes da área gráfica. Ele elimina completamente a necessidade de usar ponto flutuante ou divisões.



O algoritmo avalia o erro acumulado e utiliza apenas operações matemáticas simples com números inteiros (adição, subtração e deslocamento de bits) para determinar qual é o pixel mais próximo da linha ideal que deve ser aceso na tela. Isso o torna extremamente rápido e eficiente.

## 🚀 Funcionalidades do Programa

* Desenho de linhas na tela utilizando a equação da reta.
* Desenho de linhas na tela utilizando o Algoritmo de Bresenham.
* Desenho simultâneo em paralelo dos dois algoritmos
* Desenho simultâneo sequencial dos dois algoritmos
* Desenho de mais de uma linha por vez
* Opção de salvar o seu desenho como foto

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Java
* **Biblioteca Gráfica:** Java, Java2D

## 💻 Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Gabriel-E-S/comparadorAlgoritmosDeLinha.git
   ```