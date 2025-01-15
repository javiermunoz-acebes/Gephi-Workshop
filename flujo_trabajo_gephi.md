---
output: 
  html_document: 
    toc: true
    theme: yeti
    toc_depth: 5
---

### Guía de flujo de trabajo en Gephi

Gephi es una herramienta poderosa para analizar y visualizar redes. Este flujo de trabajo te guiará a través de las etapas principales para trabajar eficazmente en Gephi. Puedes adaptarlo según las necesidades de tu proyecto.

---

#### 1. **Importar la Red**

- **Formato de datos**: Prepara tu red en un formato compatible, como CSV, GML, o GraphML. Asegúrate de que los nodos y las aristas estén correctamente definidos.
- **Configuración inicial**:
  - Abre Gephi y selecciona el archivo a importar.
  - Verifica los parámetros inferidos:
    - Si la red es dirigida (directed) o no dirigida (undirected).
    - Los tipos de datos (p. ej., pesos en las aristas).
  - Ajusta configuraciones según corresponda (p. ej., pesos negativos, duplicados).

---

#### 2. **Calcular Atributos**

- **Menú de Estadísticas**:
  - Ve al menú de “Estadísticas” para calcular los métricos deseados. Algunos ejemplos comunes:
    - **Grado (Degree)**: Determina el número de conexiones de cada nodo.
    - **Centralidad**:
      - Centralidad de Grado: Nodos con más conexiones directas.
      - Centralidad de Intermediación (Betweenness): Nodos que conectan comunidades.
      - Centralidad de Cercanía (Closeness): Nodos centrales en términos de distancia.
    - **Modularidad**: Detecta comunidades dentro de la red.
    - **Caminos más cortos**: Identifica la ruta más corta entre nodos.
- **Personalización**: Guarda los resultados en el espacio de trabajo o expórtalos para análisis adicionales.

---

#### 3. **Apariencia**

- **Visualizar Atributos**:
  - En el panel de “Apariencia”, aplica colores, tamaños y formas a los nodos/aristas según los atributos calculados.
    - Ejemplo: Usa un gradiente de colores para la centralidad o el tamaño de los nodos basado en su grado.
- **Etiquetas**:
  - Activa etiquetas relevantes (nombres, valores) para facilitar la interpretación de los datos.
- **Opciones de Layout**:
  - Aplica algoritmos de distribución de nodos (“Layout”), como Force Atlas, Yifan Hu, o Circular.
    - Asegúrate de ajustar las configuraciones (p. ej., gravedad, repulsión) para evitar superposiciones.

---

#### 4. **Filtrar**

- **Simplificar la Red**:
  - Utiliza filtros para eliminar ruido y resaltar los aspectos clave de la red:
    - Filtra nodos según su grado, centralidad, o comunidad.
    - Elimina aristas con pesos bajos o redundantes.
- **Panel de Filtros**:
  - Arrastra y suelta los criterios de filtrado necesarios al área de trabajo.
- **Comparación Dinámica**:
  - Si tu red tiene un componente temporal, utiliza el filtro de “Intervalos” para explorar la evolución.

---

#### 5. **Exportar**

- **Opciones de Exportación**:
  - Imagen:
    - Ajusta la resolución y el formato (PNG, SVG, PDF) desde el panel de previsualización.
  - Datos estructurados:
    - Guarda los nodos y aristas como un archivo CSV, GEXF, o GraphML para análisis futuros.
- **Previsualización**:
  - Ajusta los detalles visuales (colores, tamaños, etiquetas) antes de exportar la imagen final.

---

### Consejos adicionales

- **Guardar el proyecto regularmente**: Utiliza el formato de proyecto de Gephi (.gephi) para evitar pérdida de datos.
- **Prueba diferentes configuraciones**: Explora combinaciones de métricas y visualizaciones para destacar patrones interesantes.
- **Complementos**: Instala plugins adicionales desde el marketplace de Gephi para extender las capacidades de análisis.

---
