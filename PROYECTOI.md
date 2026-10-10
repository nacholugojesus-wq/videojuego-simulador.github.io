# nacholugojesus-wq.github.io
Proyecto juego-simulador


INFORME TÉCNICO: Desarrollo de Videojuego de Carreras en Python (Menú, Selección y Simulación)

Introducción y Objetivos
El objetivo de este proyecto es diseñar y desarrollar un videojuego de carreras en Python que funcione como una aplicación independiente. El sistema incluirá un flujo completo de pantallas: un menú principal con botón de inicio, pantallas de selección de personaje y vehículo, elección de pista, y el motor principal de la carrera en tiempo real.

Stack Tecnológico (Herramientas y Librerías)
Para cumplir con los requerimientos de gráficos 2D, gestión de eventos y empaquetado, utilizaremos:
• Lenguaje: Python 3.x.
• Motor Gráfico: Pygame, ideal para manejar bucles de juego (game loops), renderizado de sprites, música, efectos de sonido y detección de colisiones en tiempo real.
• Empaquetado (Compilación a App): PyInstaller, para convertir el código y todos los recursos multimedia en un único archivo ejecutable (.exe) independiente.

Arquitectura y Estructura del Código
El proyecto se estructurará de forma modular utilizando una máquina de estados para controlar las distintas pantallas:
• main.py: Archivo principal que inicializa Pygame y controla el cambio de pantallas (Menú -> Selección -> Pista -> Juego).
• menu.py: Lógica y renderizado del menú principal y los botones interactivos.
• select_screen.py: Interfaz para elegir personajes, estadísticas de los autos y circuitos.
• game_engine.py: Núcleo de la carrera (físicas de aceleración, frenado, curvas y colisiones con los bordes de la pista).
• assets/: Carpeta contenedora de recursos (sprites de autos, fondos de pistas, avatares de personajes, música y efectos de sonido).

Fases de Implementación (Plan de Trabajo)

Fase 1: Arquitectura de Pantallas y Menú
• Programación del bucle principal y diseño de la interfaz del menú de inicio con el botón "Play".
• Creación de las pantallas intermedias para que el usuario pueda navegar y elegir su personaje, el auto deseado y la pista en la que competirá.

Fase 2: Lógica de Selección y Almacenamiento Temporal
• Implementación de variables globales o de sesión que almacenen las elecciones del usuario (ej: auto_seleccionado, pista_elegida) para pasarlas al motor de la carrera al iniciar.

Fase 3: Motor de Carreras (Gameplay)
• Desarrollo de la física de movimiento del vehículo (rotación, velocidad en función del auto elegido).
• Carga de los escenarios/pistas y renderizado de la interfaz visual durante la competencia.

Fase 4: Empaquetado y Distribución
• Uso de PyInstaller mediante consola para generar el instalable final utilizando el comando: pyinstaller --noconsole --onefile main.py
• Verificación de que el ejecutable funcione correctamente en otra PC sin necesidad de tener Python instalado.

Conclusión
Este desarrollo demuestra la capacidad de integrar programación orientada a eventos, gestión de interfaces gráficas múltiples y estructuración de software modular en Python, logrando un producto lúdico completamente funcional y listo para distribuir.
