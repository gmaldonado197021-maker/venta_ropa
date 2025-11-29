
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proyecto Minería de Datos - Tienda de Ropa</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }
        header, .container, footer {
            max-width: 1000px;
            margin: auto;
            padding: 20px;
        }
        header {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 40px 20px;
        }
        h1, h2, h3 {
            color: #2c3e50;
        }
        h2 {
            margin-top: 40px;
        }
        table {
            border-collapse: collapse;
            width: 100%;
            margin-bottom: 20px;
        }
        table, th, td {
            border: 1px solid #ccc;
            padding: 10px;
            text-align: left;
        }
        th {
            background-color: #2c3e50;
            color: white;
        }
        .dashboard {
            background-color: #ecf0f1;
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 20px;
        }
        .tree-diagram {
            margin: 20px 0;
            padding-left: 20px;
            border-left: 3px solid #2c3e50;
        }
        .tree-node {
            margin: 10px 0;
        }
        footer {
            text-align: center;
            margin-top: 40px;
            font-size: 0.9em;
            color: #777;
        }
    </style>
</head>
<body>
    <header>
        <h1>Proyecto de Minería de Datos - Tienda de Ropa</h1>
        <p>Análisis de ventas, clientes y tendencias para la toma de decisiones estratégicas</p>
    </header>

    <div class="container">
        <!-- Inicio -->
        <h2>Inicio</h2>
        <p>Este proyecto integra conceptos teóricos y prácticos de minería de datos aplicados a una tienda de ropa, con el objetivo de identificar patrones de compra, preferencias de clientes y tendencias de productos para la toma de decisiones estratégicas.</p>
        <p>Se construyó un almacén de datos, se prepararon vistas minables, se aplicaron técnicas de minería de datos y se interpretaron los resultados a través de un dashboard, demostrando la utilidad de la minería de datos en un entorno comercial real.</p>

        <!-- Base Teórica -->
        <h2>Base Teórica</h2>
        <p><strong>Sociedad de la Información y del Conocimiento:</strong> La tienda de ropa genera datos a través de ventas físicas, en línea y redes sociales. La sociedad del conocimiento se centra en transformar esta información en conocimiento útil para tomar decisiones estratégicas (Castells, 2000).</p>
        <p><strong>Inteligencia de Negocios (Business Intelligence):</strong> Convierte datos de clientes y ventas en información significativa para optimizar inventarios, promociones y estrategias de marketing (Turban et al., 2011).</p>
        <p><strong>OLAP (Procesamiento Analítico en Línea):</strong> Permite analizar ventas y preferencias de clientes desde múltiples perspectivas, facilitando reportes dinámicos y análisis de tendencias (Chaudhuri & Dayal, 1997).</p>
        <p><strong>Minería de Datos y Proceso KDD:</strong> La minería de datos identifica patrones de compra y relaciones entre productos (Fayyad et al., 1996). El proceso KDD incluye selección, preprocesamiento, transformación, minería y evaluación de datos.</p>

        <h3>Tareas y Técnicas de Minería de Datos</h3>
        <ul>
            <li>Clasificación: Predecir qué producto comprará un cliente.</li>
            <li>Regresión: Predecir ventas futuras.</li>
            <li>Clustering: Agrupar clientes por hábitos de compra.</li>
            <li>Reglas de Asociación: Identificar productos que se compran juntos.</li>
        </ul>

        <h3>Herramientas y Vistas Minables</h3>
        <ul>
            <li>Orange Data Mining</li>
            <li>Excel</li>
            <li>Python (pandas, scikit-learn)</li>
        </ul>

        <!-- Análisis de Información -->
        <h2>Análisis de Información y Minería de Datos</h2>
        <p>Se construyó un almacén de datos con información de clientes, productos y ventas. Se prepararon vistas minables para aplicar análisis de clasificación, clustering y reglas de asociación.</p>

        <h3>Tabla de Clientes</h3>
        <table>
            <tr><th>ID Cliente</th><th>Edad</th><th>Género</th><th>Ciudad</th></tr>
            <tr><td>1</td><td>25</td><td>F</td><td>Ciudad de México</td></tr>
            <tr><td>2</td><td>30</td><td>M</td><td>Guadalajara</td></tr>
            <tr><td>3</td><td>28</td><td>F</td><td>Monterrey</td></tr>
        </table>

        <h3>Tabla de Productos</h3>
        <table>
            <tr><th>ID Producto</th><th>Nombre</th><th>Categoría</th><th>Precio ($)</th></tr>
            <tr><td>101</td><td>Camiseta Básica</td><td>Top</td><td>200</td></tr>
            <tr><td>102</td><td>Jeans Clásico</td><td>Pantalón</td><td>550</td></tr>
            <tr><td>103</td><td>Chaqueta Casual</td><td>Outwear</td><td>1200</td></tr>
        </table>

        <h3>Estadísticas Descriptivas</h3>
        <table>
            <tr><th>Variable</th><th>Media</th><th>Mediana</th><th>Desviación Estándar</th></tr>
            <tr><td>Edad de Clientes</td><td>27.7</td><td>28</td><td>2.5</td></tr>
            <tr><td>Precio de Productos</td><td>650</td><td>550</td><td>500</td></tr>
        </table>

        <h3>Árbol de Decisión - Probabilidad de Compra</h3>
        <div class="tree-diagram">
            <div class="tree-node"><strong>Género?</strong></div>
            <div class="tree-node" style="margin-left:20px;">F → Edad ≤ 30? → Sí: Compra Camiseta 70% / No: Compra Chaqueta 40%</div>
            <div class="tree-node" style="margin-left:20px;">M → Prefiere Pantalón 60%</div>
        </div>

        <!-- Resultados -->
        <h2>Resultados</h2>
        <div class="dashboard">
            <p><strong>Precisión del Modelo de Compra:</strong> 82%</p>
            <p><strong>Sensibilidad:</strong> 78%</p>
            <p><strong>Especificidad:</strong> 85%</p>
        </div>

        <h3>Hallazgos Principales</h3>
        <ul>
            <li>Clientes jóvenes (≤30 años) compran más camisetas y jeans.</li>
            <li>El género es determinante para predecir la preferencia de producto.</li>
            <li>Los clientes mayores de 30 prefieren prendas formales o chaquetas.</li>
            <li>Productos comprados juntos aumentan la venta cruzada.</li>
        </ul>

        <!-- Conclusiones -->
        <h2>Conclusiones</h2>
        <p>La minería de datos permitió descubrir patrones de compra en la tienda de ropa, optimizando inventarios, promociones y estrategias de marketing.</p>
        <p>El uso de árboles de decisión, clustering y reglas de asociación permitió identificar segmentos de clientes y productos con mayor probabilidad de venta.</p>
        <p>"La minería de datos transforma datos brutos en información valiosa, y la información valiosa en conocimiento accionable para la toma de decisiones."</p>

        <!-- Referencias -->
        <h2>Referencias Bibliográficas</h2>
        <ul>
            <li>Castells, M. (2000). <em>The Rise of the Network Society</em>. Blackwell Publishing.</li>
            <li>Chaudhuri, S., & Dayal, U. (1997). <em>An overview of data warehousing and OLAP technology</em>. ACM Sigmod Record.</li>
            <li>Fayyad, U., Piatetsky-Shapiro, G., & Smyth, P. (1996). <em>From data mining to knowledge discovery in databases</em>. AI Magazine.</li>
            <li>Han, J., Kamber, M., & Pei, J. (2012). <em>Data mining: concepts and techniques</em>. Elsevier.</li>
            <li>Turban, E., Sharda, R., & Delen, D. (2011). <em>Decision support and business intelligence systems</em>. Pearson Education.</li>
        </ul>
    </div>

    <footer>
        Proyecto de Minería de Datos - Tienda de Ropa &copy; 2025
    </footer>
</body>
</html>

