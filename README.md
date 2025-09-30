# BohrModel: Implementación Computacional del Átomo de Bohr  

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)  
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)  
[![GitHub Repo](https://img.shields.io/badge/GitHub-repo-blue.svg)](https://github.com/XxyamzxX/-tomo_bohr)  
Codigo en colab : https://colab.research.google.com/drive/1nfYc0X_7lZi1Sgqql9iO9DmtIJbiT1gY?usp=sharing#scrollTo=8vBLUqhOh--H
---

## 📖 Descripción General  

**BohrModel** es una librería en Python desarrollada como una herramienta académica para el estudio del **modelo atómico de Bohr** aplicado a átomos hidrogenoides.  
El paquete permite calcular de manera interactiva:  

- **Niveles de energía** en electronvoltios.  
- **Radios de órbitas electrónicas** en metros.  
- **Transiciones electrónicas**, incluyendo energía del fotón emitido/absorbido, frecuencia y longitud de onda.  
- **Visualización gráfica** de los niveles de energía y las órbitas electrónicas.  

Este proyecto combina conceptos de **física atómica** con **desarrollo de software científico**, fomentando la integración entre teoría y práctica en la enseñanza de la física moderna.  

---

## 🎯 Objetivos  

- Implementar computacionalmente el modelo atómico de Bohr en un entorno de programación científica.  
- Brindar una herramienta interactiva para el cálculo y visualización de propiedades atómicas.  
- Aplicar principios de **programación modular, documentación y buenas prácticas** en el desarrollo de software científico.  

---

## 🔬 Fundamento Teórico  

El modelo de Bohr describe los electrones en un átomo como partículas que orbitan el núcleo en niveles de energía cuantizados.  
Las principales ecuaciones implementadas son:  

1. **Energía de un nivel electrónico**:  

\[
E_n = - \frac{Z^2 R_H}{n^2}
\]

donde:  
- \( Z \) es el número atómico.  
- \( R_H \) es la constante de Rydberg para el hidrógeno.  
- \( n \) es el número cuántico principal.  

2. **Radio de la órbita**:  

\[
r_n = \frac{n^2 a_0}{Z}
\]

donde \( a_0 \) es el radio de Bohr.  

3. **Transiciones electrónicas**:  

\[
\Delta E = E_{n_2} - E_{n_1}
\]

lo que permite obtener la **frecuencia** (\( f = \Delta E / h \)) y la **longitud de onda** (\( \lambda = c/f \)).  

---

## ⚙️ Estructura del Proyecto  


-tomo_bohr/
│── pyproject.toml
│── README.md
│── src/
│ └── bohrmodel/
│ ├── energia.py # Cálculo de niveles de energía
│ ├── radios.py # Cálculo de radios orbitales
│ ├── transiciones.py # Cálculo de transiciones electrónicas
│ ├── graficos.py # Visualizaciones de niveles y órbitas
│ └── atom.py # Menú interactivo (main)
---

## 🖥️ Instalación  

Se recomienda trabajar en un **entorno virtual**:  

"bash"
git clone https://github.com/XxyamzxX/-tomo_bohr.git
cd -tomo_bohr
pip install -e .


🚀 Uso

Ejecutar el programa principal:

python3 -m bohrmodel.atom

=== MODELO DE BOHR PARA ÁTOMOS HIDROGENOIDES ===
Ingrese el número atómico Z (1=Hidrógeno): 1

Seleccione una opción:
1. Calcular energía de un nivel (en eV)
2. Calcular radio de una órbita
3. Calcular transición electrónica
4. Graficar niveles de energía
5. Graficar órbitas electrónicas
0. Salir


