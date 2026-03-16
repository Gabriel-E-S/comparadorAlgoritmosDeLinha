# Line Algorithm Comparator 

<div align="right">
  <a href="./README.md">🇧🇷 Português</a> | 🇺🇸 English
</div>
<br>

<div align="center">
  <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java"/>
</div>
<br>

Welcome! This repository contains an application focused on comparing two classic methods for drawing lines on a pixel grid (rasterization). 

## 🎯 Objective

The main goal of this project is to demonstrate, in practice, the differences in implementation, performance, and calculation between the traditional mathematical equation of a line and the optimized Bresenham's line algorithm, widely used in Computer Graphics.

## 🧠 Understanding the Algorithms

### 1. Geometric Definition (Analytical Approach)
Uses the fundamental algebraic equation of a line: 

$$y = m \cdot x + b$$

Where $m$ is the slope (calculated by $m = \frac{\Delta y}{\Delta x}$) and $b$ is the Y-intercept. 
* **Computational disadvantage:** This method requires continuous floating-point calculations (divisions and multiplications) and rounding to find the $(x, y)$ coordinates of each pixel, which is computationally heavy and slow for the processor to render in real-time.

### 2. Bresenham's Algorithm
Created in 1962, it is one of the most important algorithms in computer graphics. It completely eliminates the need for floating-point numbers or divisions.

The algorithm evaluates the accumulated error and uses only simple integer arithmetic operations (addition, subtraction, and bit shifting) to determine which pixel is closest to the ideal line that should be illuminated on the screen. This makes it extremely fast and efficient.

## 🚀 Program Features

* Drawing lines on the screen using the geometric line equation.
* Drawing lines on the screen using Bresenham's Algorithm.
* Simultaneous parallel drawing of both algorithms.
* Simultaneous sequential drawing of both algorithms.
* Drawing multiple lines at once.
* Option to save your drawing as an image.

## 🛠️ Technologies Used

* **Language:** Java
* **Graphics Library:** Java, Java2D

## 💻 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Gabriel-E-S/comparadorAlgoritmosDeLinha.git

