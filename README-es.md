## Cleaner - Robot Aspirador Inteligente con IA

Este repositorio está disponible en varios idiomas:

- [Português](README.md)
- [English](README-en.md)

---

<img src="./.github/1.png" alt="robot-aspirador-inteligente" title="Robot Aspirador Inteligente">

---

### Tecnologías Utilizadas:

- **Python**: El lenguaje principal utilizado en el desarrollo.
- **Programación Orientada a Objetos (POO)**: Clases y objetos para representar el robot y el entorno.
- **Algoritmos Autónomos**: Lógica de control basada en el estado de las habitaciones, utilizando técnicas de toma de decisiones.
- **Inteligencia Artificial**: El proyecto aplica métodos de **aprendizaje supervisado** y **no supervisado** para optimizar la estrategia de limpieza del robot.

---

### Visión General del Proyecto:

Este proyecto simula el comportamiento de un robot aspirador inteligente que puede moverse entre varias habitaciones y limpiarlas en función de diferentes estrategias de control. El robot puede operar en modo manual, donde el usuario controla sus acciones, o en modo autónomo, donde el robot toma decisiones basadas en la suciedad detectada en las habitaciones.

Las funciones impulsadas por IA utilizan **aprendizaje supervisado** para reconocer patrones de limpieza de las habitaciones y **aprendizaje no supervisado** para adaptar el enfoque de limpieza del robot en función de las condiciones ambientales y las experiencias previas.

**Las estrategias de control incluyen**:
1. **Control Base**: El robot sigue un camino predefinido limpiando las habitaciones en función de su posición actual.
2. **Control Manual**: El usuario controla directamente los movimientos del robot.
3. **Control Omnisciente**: El robot conoce la posición de toda la suciedad y elige el orden ideal para limpiar.

---

### Cómo Ejecutar el Proyecto:

**Requisitos previos**:
- Asegúrate de que **Python** esté instalado en tu máquina. Si no, descárgalo desde [python.org](https://www.python.org/downloads/).

**Instalando el Proyecto**:

1. Clona el repositorio:
    ```bash
    git clone https://github.com/YourUsername/RobotAspiradorInteligente.git
    cd RobotAspiradorInteligente
    ```

2. Ejecuta el programa:
    ```bash
    python main.py
    ```

---

### Desglose de la Lógica del Código:

#### **Cleaner.py**:
La clase `Cleaner` representa el robot aspirador, encargado de:
- Limpiar la habitación en la que se encuentra.
- Moverse hacia la izquierda o derecha entre las habitaciones.
- Verificar si la habitación está sucia.
- Actualizar su memoria, registrando las habitaciones que ha limpiado.

Métodos principales:
- `limpiar(salas)`: Limpia la habitación.
- `mover_derecha(salas)`: Mueve el robot a la habitación de la derecha.
- `mover_izquierda(salas)`: Mueve el robot a la habitación de la izquierda.
- `verifica_limpo(salas)`: Verifica si la habitación está sucia.
- `actualiza_memoria()`: Registra la habitación limpia en la memoria del robot.

#### **Controlador.py**:
El controlador gestiona el movimiento y la limpieza del robot con varias lógicas de control:

1. **logica_robo_base**: El robot se mueve de izquierda a derecha, limpiando las habitaciones.
2. **logica_robo_onisciente**: El robot, sabiendo la ubicación de la suciedad, elige el orden óptimo de limpieza.
3. **manual_base**: El robot es controlado manualmente por el usuario, con opciones para mover, limpiar o detener el programa.
4. **Funciones auxiliares**: Como `verifica_suciedad_lejos`, que determina dónde está la suciedad más lejana.

#### **Características de IA**:
- **Aprendizaje Supervisado**: El robot es entrenado para reconocer patrones de limpieza en las habitaciones (sucias o limpias) y usa estos datos para mejorar sus estrategias de limpieza.
- **Aprendizaje No Supervisado**: El robot adapta su comportamiento según los cambios en el entorno. Ajusta dinámicamente el orden de las tareas de limpieza para minimizar el tiempo y el consumo de energía, aprendiendo de las sesiones de limpieza anteriores.

---

### 👨‍💼 Autor

<table>
  <tr>
    <td align="center">
      <a href="#">
        <img src="https://github.com/GianDutra.png" width="100px;" alt="Foto de Gian en GitHub"/><br>
        <sub>
          <b>Gian Dutra</b>
        </sub>
      </a>
    </td>
  </tr>
</table>
