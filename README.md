# Graficación: Unidad 2 - Graficacion 2D



##  Índice
* [2.1 Transformaciones Bidimensionales](#21-transformaciones-bidimensionales)
    * [Traslación](#211-traslación)
    * [Escalamiento](#212-escalamiento)
    * [Rotación](#213-rotación)
    * [Sesgado (Shear)](#214-sesgado)
* [2.2 Representación Matricial](#22-representación-matricial)
* [2.3 Trazo de Líneas Curvas](#23-trazo-de-líneas-curvas)
    * [Curvas de Bézier](#231-bézier)
    * [B-splines](#232-b-spline)
* [2.4 Fractales](#24-fractales)
* [2.5 Fuentes de Texto](#25-uso-y-creación-de-fuentes-de-texto)

---

## 2.1 Transformaciones Bidimensionales
Las transformaciones permiten alterar las propiedades geométricas de los objetos en un plano cartesiano.

### 2.1.1 Traslación
Desplazamiento de un objeto a una nueva posición mediante la suma de distancias $(t_x, t_y)$ a las coordenadas actuales.

### 2.1.2 Escalamiento
Alteración del tamaño de un objeto mediante factores de multiplicación. 
- **Uniforme:** $s_x = s_y$
- **No uniforme:** $s_x \neq s_y$

### 2.1.3 Rotación
Giro de un objeto sobre un punto pivote (normalmente el origen) siguiendo un ángulo $\theta$. Utiliza las funciones trigonométricas seno y coseno.

### 2.1.4 Sesgado
Distorsión de la forma del objeto en la que los puntos se desplazan proporcionalmente a su distancia de un eje fijo, creando un efecto de inclinación.

---

## 2.2 Representación Matricial
Para optimizar el procesamiento gráfico, las transformaciones se representan mediante matrices de $3 \times 3$ utilizando **Coordenadas Homogéneas**. Esto permite que múltiples transformaciones (como rotar y luego trasladar) se combinen en una sola matriz resultante mediante la multiplicación de las mismas.

---

## 2.3 Trazo de Líneas Curvas
Modelado matemático para generar trayectorias suaves.

### 2.3.1 Bézier
Basadas en polinomios de Bernstein. La curva es definida por puntos de control: el primero y el último son los extremos, mientras que los intermedios actúan como imanes de curvatura.

### 2.3.2 B-spline
Ofrecen un control local más preciso que las de Bézier. Modificar un punto de control solo afecta a un segmento de la curva, no a su totalidad.

---

## 2.4 Fractales
Estudio de formas geométricas que poseen **autosimilitud** a diferentes escalas. Se generan mediante procesos recursivos o iterativos y son fundamentales para modelar fenómenos naturales (nubes, montañas, costas).

---

## 2.5 Uso y Creación de Fuentes de Texto
Representación de caracteres mediante técnicas gráficas:
- **Fuentes de Mapa de Bits:** Definidas por arreglos de píxeles.
- **Fuentes Vectoriales:** Definidas matemáticamente (usualmente mediante curvas de Bézier), permitiendo escalabilidad infinita sin pérdida de resolución.

---

## 🛠️ Tecnologías sugeridas
- Lenguajes: C++, Python, Java.
- Librerías: OpenGL, SFML, Pygame, Canvas API.
