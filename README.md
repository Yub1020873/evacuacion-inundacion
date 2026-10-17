# Evacuación en zona inundada: cuando el camino más corto no es el mejor

## Qué hace
Simula un terreno inundado (riesgo 1-10, 99 = bloqueado) y compara BFS, Dijkstra y A*
para llegar a un refugio, distinguiendo entre una ruta corta y una ruta conveniente.

## Cómo ejecutarlo
1. Abre `evacuacion_inundacion.ipynb` en Google Colab (Archivo → Abrir cuaderno → GitHub).
2. Entorno de ejecución → Ejecutar todo. No necesita instalar nada extra.

## Contenido
- Estrategias: BFS, Dijkstra y A* (costo por paso = 1 + peso·(riesgo−1), con umbral de riesgo).
- Pruebas P1-P5, mapa aleatorio 12x12, casos límite y prueba contra fuerza bruta (300 mapas).
- Tabla comparativa con costo, nodos expandidos/generados y tiempo de ejecuciones reales.

## Integrantes
- Mendoza Lopez Daniel
- Ciau Lopez Jose Alfredo Reyes
- Pool Sanchez Esteban Roman
- Villanueva Cruz Angel David
- Estradas Salas Abril Monserrat
  

## Uso de IA
Usamos Claude (Anthropic) como asistente para generar la estructura inicial del código (BFS, Dijkstra, A*, validador, visualización y pruebas) y para revisar el notebook. Verificamos el código de la siguiente manera: (1) ejecutamos todas las celdas y revisamos visualmente las rutas en los mapas; (2) cada ruta pasó por validar_ruta; (3) usamos aserciones en las pruebas P2, P3 y P5; (4) comparamos Dijkstra y A* contra una implementación de fuerza bruta en 300 mapas aleatorios; (5) revisamos que todos los números de las conclusiones coincidan con la salida del notebook, sin estimaciones ni resultados inventados. Cada integrante puede explicar el funcionamiento de los algoritmos y las decisiones del diseño.
