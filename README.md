# **Diferencias Finitas vs Diferenciación Automática** 
![Banner del Proyecto](banner.png)

El objetivo de este trabajo es comparar el desempeño de dos métodos numéricos, diferencias finitas y diferenciación automática (mediante PINNs, por sus siglas en inglés), en la resolución de ecuaciones diferenciales seleccionadas. Para evaluar la precisión de ambos enfoques, se emplea la solución exacta heurística como referencia cuando esta esté disponible.

---

## **Tabla de Contenidos**
1. [Resumen](#resumen)  
2. [Características](#características)  
3. [Instalación](#instalación)
4. [Elementos](#ielementos)
5. [Créditos](#créditos)
6. [Autor](#alumno) 
7. [Contacto](#contacto)   

---

## **Resumen**
En este trabajo se abordan dos problemas numéricos mediante el uso de métodos de redes neuronales físicas (PINN) y el método tradicional de diferencias finitas. El primer problema consiste en resolver la ecuación de Poisson lineal en un dominio unitario, mientras que el segundo trata la ecuación de conducción de calor con un término fuente no lineal. Ambos problemas fueron resueltos utilizando redes neuronales con diferentes arquitecturas y utilizando grillas de diferentes tamaños (5×5, 10×10, 20×20) para el método de diferencias finitas. En el caso de diferenciación automática, se utilizaron PINN con configuraciones de capas [2, 3, 3, 1], [2, 5, 5, 1] y [2, 10, 10, 1]. Se compararon las soluciones obtenidas con las solución exacta, observando que, para la ecuación sinusoidal, las soluciones por diferencias finitas tienden a sobrestimar la intensidad, especialmente en el centro del dominio, mientras que las soluciones por PINN subestiman la intensidad. Además, se discutió el efecto de la arquitectura de la red en la precisión de las soluciones, encontrando que la implementación de condiciones de frontera estrictas y la adimensionalización de la ecuación mejora la precisión de las soluciones. En el segundo problema, se observó que la morfología de las soluciones obtenidas mediante PINN y diferencias finitas es similar, pero con diferencias en la extensión del mínimo en la esquina superior derecha del dominio. Finalmente, se observó que la distribución de los puntos de colocación no tuvo un impacto significativo en los resultados, independientemente de la distribución utilizada o el tamaño de la red neuronal. Estos resultados destacan la capacidad de PINN para abordar problemas complejos, pero también muestran las limitaciones en cuanto a la precisión y la dependencia de la resolución espacial y la configuración de la red.

---

## **Características**
- ✅ Fácil de usar.  
- 📖 Didáctico.  
- 💻​ Escaso costo computacional.  
- 📝 Investigativo.

---

## **Instalación**
Pasos para instalar y configurar el proyecto:  

### Requisitos Previos 
- ![Python](https://img.shields.io/badge/-Python-333333?style=flat&logo=python) 
- 🛜 Acceso a internet  

### Pasos
1. Clona el repositorio:  
   ```bash  
   git clone https://github.com/fabriciolopretto/Diferencias-Finitas-vs-Diferenciaci-n-Autom-tica.git  
   cd Diferencias-Finitas-vs-Diferenciaci-n-Autom-tica

---

## **Elementos**
1. Enunciado del problema.
2. Informe.
3. Presentación.
4. Notebooks con desarrollo de los experimentos.

---
## **Créditos**
Agradecimientos a las siguientes bibliotecas y recursos:

- Matplotlib
- Numpy
- Pytorch

---

## **Autor**
Lic. Fabricio Lopretto <img src="https://raw.githubusercontent.com/iampavangandhi/iampavangandhi/master/gifs/Hi.gif" width="30px"></h1>.

---

## **Contacto**
Para dudas o sugerencias, contacto en:
<a href="mailto:fabriciolopretto@gmail.com.ar">
  <img alt="Email" src="https://img.shields.io/badge/Gmail-fabriciolopretto@gmail.com-blue?style=flat-square&logo=gmail">
</a>
<a href="https://www.linkedin.com/in/fabricio-lopretto-scientific-analyst/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Fabricio%20Lopretto-blue?style=flat-square&logo=linkedin"></a>
