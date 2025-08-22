<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Economía Profundizada - Presentación Completa</title>
    <style>
        :root {
            --dark-bg: #121212;
            --dark-card: #1E1E1E;
            --accent: #FFA500;
            --text: #E0E0E0;
            --text-secondary: #B0B0B0;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--dark-bg);
            color: var(--text);
            line-height: 1.6;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            min-height: 100vh;
        }
        
        .presentation-container {
            display: flex;
            width: 100%;
            height: 100vh;
        }
        
        .sidebar {
            width: 280px;
            background-color: #1A1A1A;
            padding: 1.5rem;
            overflow-y: auto;
            border-right: 1px solid #333;
        }
        
        .sidebar h3 {
            color: var(--accent);
            margin-bottom: 1.5rem;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid var(--accent);
        }
        
        .sidebar ul {
            list-style: none;
            padding: 0;
        }
        
        .sidebar li {
            margin-bottom: 0.8rem;
        }
        
        .sidebar a {
            color: var(--text-secondary);
            text-decoration: none;
            display: block;
            padding: 0.5rem;
            border-radius: 4px;
            transition: all 0.3s ease;
            font-size: 0.95rem;
        }
        
        .sidebar a:hover, .sidebar a.active {
            background-color: #333;
            color: var(--accent);
            padding-left: 1rem;
        }
        
        .main-content {
            flex: 1;
            padding: 2rem 3rem;
            overflow-y: auto;
            position: relative;
        }
        
        h1 {
            color: var(--accent);
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            border-bottom: 3px solid var(--accent);
            padding-bottom: 0.5rem;
        }
        
        h2 {
            color: var(--accent);
            font-size: 1.8rem;
            margin: 2rem 0 1rem 0;
        }
        
        p, li {
            font-size: 1.1rem;
            color: var(--text);
            margin-bottom: 1rem;
            max-width: 800px;
            line-height: 1.7;
        }
        
        .content-card {
            background-color: var(--dark-card);
            border-radius: 10px;
            padding: 1.8rem;
            margin: 1.8rem 0;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
            border-left: 4px solid var(--accent);
        }
        
        .image-container {
            margin: 2rem 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 1.5rem;
        }
        
        .image-card {
            max-width: 45%;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
            position: relative;
            transition: transform 0.3s ease;
        }
        
        .image-card:hover {
            transform: translateY(-5px);
        }
        
        .image-card img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .image-caption {
            background: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 0.8rem;
            text-align: center;
            font-size: 0.9rem;
        }
        
        .quote {
            font-style: italic;
            color: var(--text-secondary);
            border-left: 4px solid var(--accent);
            padding: 1.2rem 1.8rem;
            margin: 2rem 0;
            background-color: rgba(30, 30, 30, 0.7);
            max-width: 700px;
        }
        
        .quote-author {
            text-align: right;
            font-weight: bold;
            color: var(--accent);
            margin-top: 0.8rem;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 1.8rem 0;
            background-color: var(--dark-card);
            max-width: 800px;
        }
        
        th, td {
            padding: 0.8rem;
            text-align: left;
            border-bottom: 1px solid #333;
        }
        
        th {
            background-color: #333;
            color: var(--accent);
        }
        
        tr:nth-child(even) {
            background-color: #252525;
        }
        
        .two-column {
            display: flex;
            gap: 2rem;
            margin: 2rem 0;
        }
        
        .column {
            flex: 1;
            min-width: 0;
        }
        
        .navigation-buttons {
            display: flex;
            justify-content: space-between;
            margin-top: 2rem;
            padding-top: 1rem;
            border-top: 1px solid #333;
        }
        
        .nav-btn {
            background-color: #333;
            color: var(--accent);
            border: none;
            padding: 0.8rem 1.5rem;
            border-radius: 4px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        
        .nav-btn:hover {
            background-color: var(--accent);
            color: #121212;
        }
        
        @media (max-width: 1200px) {
            .presentation-container {
                flex-direction: column;
            }
            
            .sidebar {
                width: 100%;
                height: auto;
                max-height: 200px;
                border-right: none;
                border-bottom: 1px solid #333;
            }
            
            .image-container {
                flex-direction: column;
            }
            
            .image-card {
                max-width: 100%;
            }
            
            .two-column {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="presentation-container">
        <div class="sidebar">
            <h3>Contenido</h3>
            <ul>
                <li><a href="#intro" class="active">Introducción</a></li>
                <li><a href="#definicion">Definición</a></li>
                <li><a href="#adam-smith">Adam Smith</a></li>
                <li><a href="#karl-marx">Karl Marx</a></li>
                <li><a href="#revoluciones">Revoluciones Industriales</a></li>
                <li><a href="#microeconomia">Microeconomía</a></li>
                <li><a href="#empresa">La Empresa</a></li>
                <li><a href="#empresas-mexico">Empresas en México</a></li>
                <li><a href="#macroeconomia">Macroeconomía</a></li>
                <li><a href="#referencias">Referencias</a></li>
            </ul>
        </div>
        
        <div class="main-content" id="main-content">
            <!-- Introducción a la economía -->
            <section id="intro">
                <h1>Introducción a la Economía</h1>
                
                <div class="content-card">
                    <p>La economía es una <strong>ciencia social</strong> que estudia cómo los individuos, empresas y gobiernos <strong>toman decisiones</strong> para asignar <strong>recursos limitados</strong> que tienen usos alternativos, con el objetivo de satisfacer <strong>necesidades ilimitadas</strong>.</p>
                    
                    <p>Esta disciplina analiza los procesos de producción, distribución, intercambio y consumo de bienes y servicios en una sociedad.</p>
                </div>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1450101499163-c8848c66ca85?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Flujo económico">
                        <div class="image-caption">El flujo circular de la economía muestra la interacción entre hogares y empresas</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Actividad económica">
                        <div class="image-caption">La economía estudia toda la actividad productiva de una sociedad</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Divisiones principales</h2>
                    
                    <div class="two-column">
                        <div class="column">
                            <h3>Microeconomía</h3>
                            <p>Estudia el comportamiento de unidades económicas individuales:</p>
                            <ul>
                                <li>Consumidores y sus decisiones</li>
                                <li>Empresas y sus estrategias</li>
                                <li>Mercados específicos</li>
                                <li>Formación de precios</li>
                            </ul>
                        </div>
                        
                        <div class="column">
                            <h3>Macroeconomía</h3>
                            <p>Analiza variables económicas agregadas:</p>
                            <ul>
                                <li>Producto Interno Bruto (PIB)</li>
                                <li>Inflación y desempleo</li>
                                <li>Políticas económicas</li>
                                <li>Crecimiento económico</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="quote">
                    "La economía es el estudio de cómo la sociedad gestiona sus recursos escasos."
                    <div class="quote-author">- Gregory Mankiw</div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('intro')">Inicio</button>
                    <button class="nav-btn" onclick="scrollToSection('definicion')">Siguiente →</button>
                </div>
            </section>
            
            <!-- Definición de economía -->
            <section id="definicion">
                <h1>Definición de Economía</h1>
                
                <div class="content-card">
                    <h2>Definición clásica</h2>
                    <p>Según <strong>Lionel Robbins</strong> (1932), la economía es:</p>
                    <div class="quote">
                        "La ciencia que estudia el comportamiento humano como una relación entre fines y medios escasos que tienen usos alternativos."
                        <div class="quote-author">- Lionel Robbins</div>
                    </div>
                    <p>Esta definición enfatiza tres conceptos clave:</p>
                    <ol>
                        <li><strong>Fines múltiples:</strong> Necesidades y deseos ilimitados</li>
                        <li><strong>Medios escasos:</strong> Recursos limitados</li>
                        <li><strong>Usos alternativos:</strong> Los recursos pueden asignarse de diferentes maneras</li>
                    </ol>
                </div>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Toma de decisiones económicas">
                        <div class="image-caption">La economía estudia cómo tomamos decisiones con recursos limitados</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1434626881859-194d67b2b86f?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Escasez de recursos">
                        <div class="image-caption">La escasez es el problema fundamental que estudia la economía</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Problema económico fundamental</h2>
                    <p>El <strong>problema fundamental</strong> que estudia la economía surge de la <strong>escasez</strong> (recursos limitados frente a necesidades ilimitadas), lo que obliga a:</p>
                    <ul>
                        <li><strong>Elegir</strong> entre alternativas</li>
                        <li>Considerar el <strong>costo de oportunidad</strong> (lo que se sacrifica al elegir una opción)</li>
                        <li>Buscar la <strong>eficiencia</strong> en la asignación de recursos</li>
                    </ul>
                    
                    <div class="quote">
                        "En economía, no existe el almuerzo gratis. Todo tiene un costo."
                        <div class="quote-author">- Milton Friedman</div>
                    </div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('intro')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('adam-smith')">Siguiente →</button>
                </div>
            </section>
            
            <!-- Adam Smith -->
            <section id="adam-smith">
                <h1>Adam Smith: Padre de la Economía Moderna</h1>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/d/d4/Adam_Smith_The_Muir_portrait.jpg" alt="Retrato de Adam Smith">
                        <div class="image-caption">Adam Smith (1723-1790), considerado el padre de la economía moderna</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/5/5a/Wealth_of_Nations.jpg" alt="La riqueza de las naciones">
                        <div class="image-caption">Portada original de "La riqueza de las naciones" (1776)</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Vida y obra</h2>
                    <p><strong>Adam Smith</strong> fue un filósofo y economista escocés cuya obra <em>La riqueza de las naciones</em> (1776) sentó las bases del <strong>liberalismo económico</strong> y la <strong>economía clásica</strong>.</p>
                    
                    <p>Smith analizó cómo el <strong>interés individual</strong> y la <strong>competencia</strong> en mercados libres pueden conducir al <strong>bienestar colectivo</strong> a través del mecanismo que llamó "la mano invisible".</p>
                    
                    <div class="two-column">
                        <div class="column">
                            <h3>Principales ideas</h3>
                            <ul>
                                <li>La división del trabajo aumenta la productividad</li>
                                <li>Los mercados libres conducen a la eficiencia</li>
                                <li>El estado debe limitar su intervención</li>
                                <li>El trabajo es la fuente real de la riqueza</li>
                            </ul>
                        </div>
                        
                        <div class="column">
                            <h3>Conceptos clave</h3>
                            <ul>
                                <li>Mano invisible del mercado</li>
                                <li>División del trabajo</li>
                                <li>Ventaja absoluta</li>
                                <li>Teoría del valor-trabajo</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>La mano invisible</h2>
                    <p>El concepto más famoso de Smith describe cómo el mercado se autorregula:</p>
                    
                    <div class="quote">
                        "No es por la benevolencia del carnicero, del cervecero o del panadero que podemos esperar nuestra cena, sino por su propio interés."
                        <div class="quote-author">- Adam Smith, La riqueza de las naciones</div>
                    </div>
                    
                    <p>Smith argumentó que cuando los individuos buscan su propio beneficio en un mercado competitivo, son guiados como por una <strong>"mano invisible"</strong> a promover el bienestar social, aunque ese no sea su intención.</p>
                    
                    <div class="image-container">
                        <div class="image-card">
                            <img src="https://upload.wikimedia.org/wikipedia/commons/0/03/Coalbrookdale_by_Night.jpg" alt="Revolución industrial">
                            <div class="image-caption">Paisaje industrial que surgió tras las ideas de Smith</div>
                        </div>
                    </div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('definicion')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('karl-marx')">Siguiente →</button>
                </div>
            </section>
            
            <!-- Karl Marx -->
            <section id="karl-marx">
                <h1>Karl Marx: Crítica al Capitalismo</h1>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/d/d4/Karl_Marx_001.jpg" alt="Retrato de Karl Marx">
                        <div class="image-caption">Karl Marx (1818-1883), filósofo y economista crítico del capitalismo</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Das_Kapital.jpg" alt="El Capital de Marx">
                        <div class="image-caption">Portada original de "El Capital" (1867)</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Vida y obra</h2>
                    <p><strong>Karl Marx</strong> fue un filósofo, economista y revolucionario alemán cuyo análisis crítico del <strong>capitalismo</strong> influyó profundamente en la historia del siglo XX.</p>
                    
                    <p>Su obra principal, <em>El Capital</em> (1867), es un análisis exhaustivo del sistema capitalista y sus contradicciones internas, donde desarrolla conceptos como la plusvalía, la explotación y la lucha de clases.</p>
                    
                    <div class="two-column">
                        <div class="column">
                            <h3>Obras principales</h3>
                            <ul>
                                <li><em>El Capital</em> (1867)</li>
                                <li><em>Manifiesto Comunista</em> (1848, con Engels)</li>
                                <li><em>Contribución a la crítica de la economía política</em> (1859)</li>
                            </ul>
                        </div>
                        
                        <div class="column">
                            <h3>Influencia</h3>
                            <ul>
                                <li>Fundador del socialismo científico</li>
                                <li>Inspiró movimientos revolucionarios</li>
                                <li>Crítica fundamental al capitalismo</li>
                                <li>Base teórica para sistemas comunistas</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Conceptos clave del marxismo</h2>
                    
                    <table>
                        <tr>
                            <th>Concepto</th>
                            <th>Explicación</th>
                            <th>Relevancia actual</th>
                        </tr>
                        <tr>
                            <td>Plusvalía</td>
                            <td>Valor que los trabajadores producen pero no reciben, apropiado por los capitalistas</td>
                            <td>Debates sobre salarios justos</td>
                        </tr>
                        <tr>
                            <td>Lucha de clases</td>
                            <td>Conflicto histórico entre clases sociales por el control de los medios de producción</td>
                            <td>Desigualdad económica</td>
                        </tr>
                        <tr>
                            <td>Materialismo histórico</td>
                            <td>Las condiciones materiales determinan la estructura social y política</td>
                            <td>Análisis de sistemas económicos</td>
                        </tr>
                        <tr>
                            <td>Alienación</td>
                            <td>Separación del trabajador del producto y proceso de su trabajo</td>
                            <td>Crítica al trabajo moderno</td>
                        </tr>
                    </table>
                    
                    <div class="quote">
                        "Los filósofos no han hecho más que interpretar el mundo de diversos modos; de lo que se trata es de transformarlo."
                        <div class="quote-author">- Karl Marx, Tesis sobre Feuerbach</div>
                    </div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('adam-smith')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('revoluciones')">Siguiente →</button>
                </div>
            </section>
            
            <!-- Revoluciones Industriales -->
            <section id="revoluciones">
                <h1>Revoluciones Industriales</h1>
                
                <div class="content-card">
                    <h2>Las cuatro revoluciones industriales</h2>
                    <p>Las revoluciones industriales representan cambios profundos en los sistemas de producción que transformaron radicalmente la estructura económica y social:</p>
                    
                    <table>
                        <tr>
                            <th>Revolución</th>
                            <th>Periodo</th>
                            <th>Innovaciones clave</th>
                            <th>Impacto económico</th>
                        </tr>
                        <tr>
                            <td>Primera</td>
                            <td>1760-1840</td>
                            <td>Máquina de vapor, energía hidráulica, mecanización textil</td>
                            <td>Producción en masa, urbanización, surgimiento del proletariado</td>
                        </tr>
                        <tr>
                            <td>Segunda</td>
                            <td>1870-1914</td>
                            <td>Electricidad, motor de combustión, producción en cadena</td>
                            <td>Grandes corporaciones, expansión de mercados, economía de escala</td>
                        </tr>
                        <tr>
                            <td>Tercera</td>
                            <td>1960-2000</td>
                            <td>Computadoras, automatización, electrónica, internet</td>
                            <td>Globalización, economía del conocimiento, desindustrialización</td>
                        </tr>
                        <tr>
                            <td>Cuarta</td>
                            <td>2000-presente</td>
                            <td>Inteligencia artificial, robótica avanzada, IoT, blockchain</td>
                            <td>Automatización total, economía digital, flexibilización laboral</td>
                        </tr>
                    </table>
                </div>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/4/4d/Ford_assembly_line_-_1913.jpg" alt="Línea de ensamblaje de Ford">
                        <div class="image-caption">Línea de ensamblaje de Ford (1913), símbolo de la segunda revolución industrial</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/3/3a/Intel_D4040_2293B_top.jpg" alt="Microprocesador Intel">
                        <div class="image-caption">Microprocesador Intel 4004 (1971), clave en la tercera revolución industrial</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Impacto de las revoluciones industriales</h2>
                    
                    <div class="two-column">
                        <div class="column">
                            <h3>Cambios económicos</h3>
                            <ul>
                                <li>Transición de economía agraria a industrial</li>
                                <li>Aumento de productividad y producción</li>
                                <li>Desarrollo del comercio internacional</li>
                                <li>Surgimiento del capitalismo moderno</li>
                                <li>Cambios en la estructura del empleo</li>
                            </ul>
                        </div>
                        
                        <div class="column">
                            <h3>Cambios sociales</h3>
                            <ul>
                                <li>Crecimiento urbano y migraciones</li>
                                <li>Surgimiento de nuevas clases sociales</li>
                                <li>Cambios en la organización del trabajo</li>
                                <li>Mejoras en calidad de vida (a largo plazo)</li>
                                <li>Nuevas formas de desigualdad</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="quote">
                        "La revolución industrial cambió no solo la forma de producir, sino la estructura misma de la sociedad."
                        <div class="quote-author">- Eric Hobsbawm</div>
                    </div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('karl-marx')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('microeconomia')">Siguiente →</button>
                </div>
            </section>
            
            <!-- Microeconomía -->
            <section id="microeconomia">
                <h1>Microeconomía: Fundamentos</h1>
                
                <div class="content-card">
                    <h2>¿Qué es la microeconomía?</h2>
                    <p>La microeconomía es la rama de la economía que estudia el <strong>comportamiento de unidades económicas individuales</strong> (consumidores, empresas, mercados específicos) y cómo toman decisiones para <strong>asignar recursos limitados</strong>.</p>
                    
                    <p>Se enfoca en comprender:</p>
                    <ul>
                        <li>Cómo los individuos toman decisiones de consumo</li>
                        <li>Cómo las empresas deciden qué y cuánto producir</li>
                        <li>Cómo interactúan oferentes y demandantes en mercados específicos</li>
                        <li>Cómo se determinan los precios de bienes y servicios</li>
                        <li>Cómo se asignan los recursos en una economía</li>
                    </ul>
                </div>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/3/3e/Supply-demand-right-shift-demand-curve.svg" alt="Curvas de oferta y demanda">
                        <div class="image-caption">Las curvas de oferta y demanda son fundamentales en el análisis microeconómico</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1554224155-6726b3ff858f?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Toma de decisiones económicas">
                        <div class="image-caption">La microeconomía estudia cómo los consumidores toman decisiones</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Conceptos clave de microeconomía</h2>
                    
                    <table>
                        <tr>
                            <th>Concepto</th>
                            <th>Explicación</th>
                            <th>Ejemplo</th>
                        </tr>
                        <tr>
                            <td>Oferta y demanda</td>
                            <td>Leyes que determinan precios y cantidades en el mercado</td>
                            <td>Precio de la gasolina varía según disponibilidad y consumo</td>
                        </tr>
                        <tr>
                            <td>Elasticidad</td>
                            <td>Sensibilidad de cantidad demandada u ofertada ante cambios de precio</td>
                            <td>Productos básicos tienen demanda inelástica (poca variación)</td>
                        </tr>
                        <tr>
                            <td>Costos de producción</td>
                            <td>Fijos (no varían con producción) y variables (sí varían)</td>
                            <td>Alquiler de local es costo fijo; materias primas son variables</td>
                        </tr>
                        <tr>
                            <td>Estructuras de mercado</td>
                            <td>Competencia perfecta, monopolio, oligopolio, competencia monopolística</td>
                            <td>Mercado de telecomunicaciones es oligopolio</td>
                        </tr>
                        <tr>
                            <td>Utilidad marginal</td>
                            <td>Satisfacción adicional que obtiene un consumidor al consumir una unidad más</td>
                            <td>Primer helado da más satisfacción que el quinto</td>
                        </tr>
                    </table>
                </div>
                
                <div class="content-card">
                    <h2>Teoría del consumidor</h2>
                    <p>La microeconomía analiza cómo los consumidores toman decisiones basadas en:</p>
                    
                    <div class="two-column">
                        <div class="column">
                            <h3>Preferencias</h3>
                            <ul>
                                <li>Completas: Pueden comparar todas las opciones</li>
                                <li>Transitivas: Si A > B y B > C, entonces A > C</li>
                                <li>Racionales: Buscan maximizar su satisfacción</li>
                                <li>No saciadas: Más es preferible a menos</li>
                            </ul>
                        </div>
                        
                        <div class="column">
                            <h3>Restricciones</h3>
                            <ul>
                                <li>Presupuesto limitado</li>
                                <li>Precios de los bienes</li>
                                <li>Disponibilidad de productos</li>
                                <li>Información disponible</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="quote">
                        "La microeconomía explica cómo asignamos nuestros recursos escasos entre infinitas necesidades."
                        <div class="quote-author">- Paul Samuelson</div>
                    </div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('revoluciones')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('empresa')">Siguiente →</button>
                </div>
            </section>
            
            <!-- La Empresa -->
            <section id="empresa">
                <h1>La Empresa en el Sistema Económico</h1>
                
                <div class="content-card">
                    <h2>¿Qué es una empresa?</h2>
                    <p>Una empresa es una <strong>unidad económica de producción</strong> que combina factores productivos (tierra, trabajo, capital) para <strong>crear bienes o servicios</strong> que se ofrecen en el mercado con el objetivo de obtener beneficios.</p>
                    
                    <p>Características esenciales:</p>
                    <ul>
                        <li>Organiza y coordina recursos productivos</li>
                        <li>Asume riesgos económicos</li>
                        <li>Busca maximizar beneficios (aunque no es su único objetivo)</li>
                        <li>Es el agente principal de la oferta en los mercados</li>
                        <li>Contribuye al crecimiento económico</li>
                    </ul>
                </div>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Empresa moderna">
                        <div class="image-caption">Las empresas son el motor de la actividad económica en el capitalismo</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1521791136064-7986c2920216?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Producción industrial">
                        <div class="image-caption">Las empresas transforman insumos en productos terminados</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Funciones y tipos de empresas</h2>
                    
                    <h3>Funciones principales:</h3>
                    <ol>
                        <li><strong>Producción:</strong> Transformar insumos en productos terminados</li>
                        <li><strong>Distribución:</strong> Hacer llegar los productos a los consumidores</li>
                        <li><strong>Inversión:</strong> Asignar recursos para crecimiento futuro</li>
                        <li><strong>Innovación:</strong> Desarrollar nuevos productos y procesos</li>
                        <li><strong>Generación de empleo:</strong> Contratar trabajadores</li>
                    </ol>
                    
                    <h3>Clasificación por tamaño:</h3>
                    <ul>
                        <li><strong>Microempresa:</strong> Hasta 10 empleados</li>
                        <li><strong>Pequeña empresa:</strong> 11-50 empleados</li>
                        <li><strong>Mediana empresa:</strong> 51-250 empleados</li>
                        <li><strong>Gran empresa:</strong> Más de 250 empleados</li>
                    </ul>
                    
                    <h3>Clasificación por actividad:</h3>
                    <ul>
                        <li><strong>Primario:</strong> Extracción de recursos (agricultura, minería)</li>
                        <li><strong>Secundario:</strong> Transformación (industria manufacturera)</li>
                        <li><strong>Terciario:</strong> Servicios (bancos, educación, salud)</li>
                        <li><strong>Cuaternario:</strong> Información y conocimiento (TI, investigación)</li>
                    </ul>
                </div>
                
                <div class="content-card">
                    <h2>Objetivos empresariales</h2>
                    
                    <div class="two-column">
                        <div class="column">
                            <h3>Objetivos principales</h3>
                            <ul>
                                <li><strong>Maximizar beneficios:</strong> Diferencia entre ingresos y costos</li>
                                <li><strong>Maximizar valor para accionistas:</strong> Aumentar valor de la empresa</li>
                                <li><strong>Crecimiento sostenible:</strong> Expansión a largo plazo</li>
                                <li><strong>Supervivencia:</strong> Mantener operaciones en el tiempo</li>
                            </ul>
                        </div>
                        
                        <div class="column">
                            <h3>Objetivos secundarios</h3>
                            <ul>
                                <li><strong>Responsabilidad social:</strong> Impacto positivo en sociedad</li>
                                <li><strong>Cuota de mercado:</strong> Porcentaje del mercado que controla</li>
                                <li><strong>Calidad:</strong> Excelencia en productos/servicios</li>
                                <li><strong>Satisfacción del cliente:</strong> Fidelizar consumidores</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="quote">
                        "El negocio de los negocios es el negocio."
                        <div class="quote-author">- Milton Friedman</div>
                    </div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('microeconomia')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('empresas-mexico')">Siguiente →</button>
                </div>
            </section>
            
            <!-- Empresas en México -->
            <section id="empresas-mexico">
                <h1>Historia Empresarial de México</h1>
                
                <div class="content-card">
                    <h2>Primeras empresas en México</h2>
                    <p>El desarrollo empresarial en México ha pasado por distintas etapas, desde la época colonial hasta la actualidad:</p>
                    
                    <table>
                        <tr>
                            <th>Empresa</th>
                            <th>Año</th>
                            <th>Sector</th>
                            <th>Importancia histórica</th>
                        </tr>
                        <tr>
                            <td>Real del Monte</td>
                            <td>1550s</td>
                            <td>Minería</td>
                            <td>Primera gran empresa colonial, explotación de plata</td>
                        </tr>
                        <tr>
                            <td>Fábrica de Tabacos</td>
                            <td>1764</td>
                            <td>Manufactura</td>
                            <td>Primera fábrica a gran escala en Nueva España</td>
                        </tr>
                        <tr>
                            <td>Compañía Fundidora de Fierro y Acero</td>
                            <td>1900</td>
                            <td>Siderurgia</td>
                            <td>Base de la industrialización mexicana</td>
                        </tr>
                        <tr>
                            <td>Cervecería Cuauhtémoc</td>
                            <td>1890</td>
                            <td>Bebidas</td>
                            <td>Modelo de desarrollo empresarial industrial</td>
                        </tr>
                        <tr>
                            <td>Pemex</td>
                            <td>1938</td>
                            <td>Energía</td>
                            <td>Resultado de la expropiación petrolera</td>
                        </tr>
                    </table>
                </div>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/3/3e/Fundidora_monterrey_1909.jpg" alt="Fundidora de Monterrey">
                        <div class="image-caption">Compañía Fundidora de Fierro y Acero de Monterrey (1909), símbolo de la industrialización</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/9/9b/PEMEX_Refineria_Cadereyta.jpg" alt="Refinería Pemex">
                        <div class="image-caption">Refinería de Pemex, empresa estatal creada tras la expropiación petrolera</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Evolución del sector empresarial mexicano</h2>
                    <p>El desarrollo empresarial en México ha seguido varias etapas:</p>
                    
                    <ol>
                        <li><strong>Época colonial (1521-1821):</strong> Empresas mineras y agrícolas bajo el modelo de encomienda</li>
                        <li><strong>Siglo XIX:</strong> Surgimiento de manufacturas textiles y cerveceras</li>
                        <li><strong>Porfiriato (1876-1911):</strong> Inversión extranjera en ferrocarriles y minería</li>
                        <li><strong>Siglo XX:</strong> Industrialización por sustitución de importaciones</li>
                        <li><strong>Neoliberalismo (1982-actualidad):</strong> Apertura comercial y privatizaciones</li>
                    </ol>
                    
                    <h3>Empresas mexicanas emblemáticas:</h3>
                    <ul>
                        <li><strong>Grupo Bimbo:</strong> Líder mundial en panificación</li>
                        <li><strong>Cemex:</strong> Tercer productor mundial de cemento</li>
                        <li><strong>Grupo México:</strong> Minera importante a nivel global</li>
                        <li><strong>América Móvil:</strong> Empresa de telecomunicaciones de Carlos Slim</li>
                        <li><strong>FEMSA:</strong> Dueña de Coca-Cola FEMSA y OXXO</li>
                    </ul>
                </div>
                
                <div class="content-card">
                    <h2>Desafíos actuales de las empresas mexicanas</h2>
                    
                    <div class="two-column">
                        <div class="column">
                            <h3>Desafíos internos</h3>
                            <ul>
                                <li>Baja productividad</li>
                                <li>Informalidad laboral</li>
                                <li>Corrupción</li>
                                <li>Falta de innovación</li>
                                <li>Acceso limitado a financiamiento</li>
                            </ul>
                        </div>
                        
                        <div class="column">
                            <h3>Desafíos externos</h3>
                            <ul>
                                <li>Competencia global</li>
                                <li>Dependencia económica de EE.UU.</li>
                                <li>Tratados comerciales</li>
                                <li>Cambios tecnológicos</li>
                                <li>Pandemia y crisis económicas</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="quote">
                        "La historia empresarial de México refleja nuestra compleja relación con el desarrollo económico."
                        <div class="quote-author">- Carlos Tello, economista mexicano</div>
                    </div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('empresa')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('macroeconomia')">Siguiente →</button>
                </div>
            </section>
            
            <!-- Macroeconomía -->
            <section id="macroeconomia">
                <h1>Macroeconomía: Visión Global</h1>
                
                <div class="content-card">
                    <h2>¿Qué es la macroeconomía?</h2>
                    <p>La macroeconomía es el estudio del <strong>comportamiento agregado</strong> de la economía, analizando variables como el crecimiento del PIB, inflación, desempleo y balanza comercial para comprender y mejorar el desempeño económico general.</p>
                    
                    <p>Principales objetivos de la política macroeconómica:</p>
                    <ol>
                        <li><strong>Crecimiento económico:</strong> Aumento sostenido del PIB</li>
                        <li><strong>Pleno empleo:</strong> Minimizar el desempleo</li>
                        <li><strong>Estabilidad de precios:</strong> Controlar la inflación</li>
                        <li><strong>Equilibrio externo:</strong> Balance adecuado en comercio internacional</li>
                        <li><strong>Distribución justa del ingreso:</strong> Reducir desigualdades</li>
                    </ol>
                </div>
                
                <div class="image-container">
                    <div class="image-card">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/7/7e/Macroeconomics_diagram_-_Business_cycle_in_united_states.svg" alt="Ciclo económico">
                        <div class="image-caption">El ciclo económico muestra las fluctuaciones en el crecimiento del PIB</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1611974789855-9c2a0a7236a3?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Indicadores económicos">
                        <div class="image-caption">La macroeconomía analiza indicadores agregados</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Indicadores macroeconómicos clave</h2>
                    
                    <table>
                        <tr>
                            <th>Indicador</th>
                            <th>Definición</th>
                            <th>Importancia</th>
                        </tr>
                        <tr>
                            <td>PIB (Producto Interno Bruto)</td>
                            <td>Valor total de bienes y servicios producidos en un país en un período</td>
                            <td>Mide el tamaño y crecimiento de la economía</td>
                        </tr>
                        <tr>
                            <td>Inflación</td>
                            <td>Aumento generalizado y sostenido de los precios</td>
                            <td>Afecta poder adquisitivo y decisiones económicas</td>
                        </tr>
                        <tr>
                            <td>Tasa de desempleo</td>
                            <td>Porcentaje de la fuerza laboral que busca empleo pero no lo encuentra</td>
                            <td>Indicador de bienestar social y eficiencia económica</td>
                        </tr>
                        <tr>
                            <td>Balanza comercial</td>
                            <td>Diferencia entre exportaciones e importaciones</td>
                            <td>Muestra competitividad internacional</td>
                        </tr>
                        <tr>
                            <td>Déficit fiscal</td>
                            <td>Cuando el gasto público supera los ingresos</td>
                            <td>Afecta deuda pública y estabilidad económica</td>
                        </tr>
                    </table>
                </div>
                
                <div class="content-card">
                    <h2>Políticas macroeconómicas</h2>
                    
                    <div class="two-column">
                        <div class="column">
                            <h3>Política fiscal</h3>
                            <p>Decisiones del gobierno sobre <strong>impuestos</strong> y <strong>gasto público</strong>:</p>
                            <ul>
                                <li><strong>Expansiva:</strong> Aumentar gasto público o reducir impuestos para estimular economía</li>
                                <li><strong>Contractiva:</strong> Reducir gasto público o aumentar impuestos para frenar inflación</li>
                                <li><strong>Instrumentos:</strong> Presupuesto nacional, impuestos, subsidios, obra pública</li>
                            </ul>
                        </div>
                        
                        <div class="column">
                            <h3>Política monetaria</h3>
                            <p>Control del banco central sobre <strong>oferta monetaria</strong> y <strong>tasas de interés</strong>:</p>
                            <ul>
                                <li><strong>Expansiva:</strong> Aumentar oferta monetaria, bajar tasas para estimular crédito</li>
                                <li><strong>Contractiva:</strong> Reducir oferta monetaria, subir tasas para controlar inflación</li>
                                <li><strong>Instrumentos:</strong> Operaciones de mercado abierto, encajes bancarios, tasa de descuento</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="quote">
                        "La macroeconomía nos ayuda a entender por qué algunas economías prosperan mientras otras se estancan."
                        <div class="quote-author">- Nouriel Roubini</div>
                    </div>
                </div>
                
                <div class="content-card">
                    <h2>Corrientes macroeconómicas</h2>
                    
                    <table>
                        <tr>
                            <th>Escuela</th>
                            <th>Representantes</th>
                            <th>Principales ideas</th>
                        </tr>
                        <tr>
                            <td>Clásica</td>
                            <td>Adam Smith, David Ricardo</td>
                            <td>Mercados se autorregulan, estado mínimo</td>
                        </tr>
                        <tr>
                            <td>Keynesiana</td>
                            <td>John Maynard Keynes</td>
                            <td>Intervención estatal para estabilizar economía</td>
                        </tr>
                        <tr>
                            <td>Monetarista</td>
                            <td>Milton Friedman</td>
                            <td>Control de oferta monetaria para controlar inflación</td>
                        </tr>
                        <tr>
                            <td>Neoclásica</td>
                            <td>Alfred Marshall, Léon Walras</td>
                            <td>Equilibrios de mercado, expectativas racionales</td>
                        </tr>
                    </table>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('empresas-mexico')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('referencias')">Siguiente →</button>
                </div>
            </section>
            
            <!-- Referencias -->
            <section id="referencias">
                <h1>Referencias Bibliográficas</h1>
                
                <div class="content-card">
                    <h2>Libros fundamentales</h2>
                    <ul>
                        <li><strong>Smith, A. (2003).</strong> <em>La riqueza de las naciones.</em> Alianza Editorial. (Original publicado en 1776)</li>
                        <li><strong>Marx, K. (2010).</strong> <em>El Capital.</em> (8ª ed.). Siglo XXI. (Original publicado en 1867)</li>
                        <li><strong>Keynes, J.M. (2018).</strong> <em>Teoría general del empleo, el interés y el dinero.</em> FCE. (Original publicado en 1936)</li>
                        <li><strong>Mankiw, G. (2020).</strong> <em>Principios de economía.</em> (8ª ed.). Cengage Learning.</li>
                        <li><strong>Samuelson, P. & Nordhaus, W. (2019).</strong> <em>Economía.</em> (19ª ed.). McGraw-Hill.</li>
                        <li><strong>Friedman, M. (2002).</strong> <em>Capitalismo y libertad.</em> RBA.</li>
                        <li><strong>Krugman, P. & Wells, R. (2018).</strong> <em>Economía.</em> Reverté.</li>
                        <li><strong>Piketty, T. (2014).</strong> <em>El capital en el siglo XXI.</em> FCE.</li>
                    </ul>
                </div>
                
                <div class="content-card">
                    <h2>Artículos académicos</h2>
                    <ul>
                        <li><strong>Robbins, L. (1932).</strong> <em>An Essay on the Nature and Significance of Economic Science.</em> Macmillan.</li>
                        <li><strong>Keynes, J.M. (1937).</strong> "The General Theory of Employment". <em>Quarterly Journal of Economics.</em></li>
                        <li><strong>Friedman, M. (1968).</strong> "The Role of Monetary Policy". <em>American Economic Review.</em></li>
                        <li><strong>Krugman, P. (2009).</strong> "The Return of Depression Economics and the Crisis of 2008." <em>W.W. Norton & Company.</em></li>
                        <li><strong>Stiglitz, J. (2015).</strong> "The Great Divide: Unequal Societies and What We Can Do About Them." <em>W.W. Norton & Company.</em></li>
                    </ul>
                </div>
                
                <div class="content-card">
                    <h2>Fuentes en línea y estadísticas</h2>
                    <ul>
                        <li><strong>Banco de México.</strong> (2025). Reportes trimestrales. Recuperado de: https://www.banxico.org.mx</li>
                        <li><strong>INEGI.</strong> (2025). Sistema de Cuentas Nacionales. Recuperado de: https://www.inegi.org.mx</li>
                        <li><strong>FMI.</strong> (2025). World Economic Outlook. Recuperado de: https://www.imf.org</li>
                        <li><strong>Banco Mundial.</strong> (2025). Indicadores de desarrollo mundial. Recuperado de: https://datos.bancomundial.org</li>
                        <li><strong>OCDE.</strong> (2025). Estadísticas económicas. Recuperado de: https://www.oecd.org</li>
                        <li><strong>SE.</strong> (2025). Información económica. Recuperado de: https://www.gob.mx/se</li>
                    </ul>
                </div>
                
                <div class="quote">
                    "El estudio de la economía no parece requerir ningún don especializado de un orden más que normalmente elevado. ¿No es una disciplina muy fácil comparada con las ramas superiores de la filosofía y la ciencia pura?"
                    <div class="quote-author">- John Maynard Keynes</div>
                </div>
                
                <div class="navigation-buttons">
                    <button class="nav-btn" onclick="scrollToSection('macroeconomia')">← Anterior</button>
                    <button class="nav-btn" onclick="scrollToSection('intro')">Volver al inicio</button>
                </div>
            </section>
        </div>
    </div>
    
    <script>
        // Función para desplazarse a secciones
        function scrollToSection(sectionId) {
            const element = document.getElementById(sectionId);
            if (element) {
                element.scrollIntoView({ behavior: 'smooth' });
                updateActiveLink(sectionId);
            }
        }
        
        // Actualizar enlace activo en el menú
        function updateActiveLink(sectionId) {
            const links = document.querySelectorAll('.sidebar a');
            links.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === `#${sectionId}`) {
                    link.classList.add('active');
                }
            });
        }
        
        // Actualizar navegación al hacer scroll
        const sections = document.querySelectorAll('section');
        const sidebarLinks = document.querySelectorAll('.sidebar a');
        
        window.addEventListener('scroll', () => {
            let current = '';
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                
                if (pageYOffset >= (sectionTop - 300)) {
                    current = section.getAttribute('id');
                }
            });
            
            sidebarLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === `#${current}`) {
                    link.classList.add('active');
                }
            });
        });
        
        // Configurar eventos de clic para los enlaces del menú
        sidebarLinks.forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault();
                const sectionId = link.getAttribute('href').substring(1);
                scrollToSection(sectionId);
            });
        });
        
        // Navegación por teclado
        document.addEventListener('keydown', (e) => {
            if (e.key === 'ArrowRight') {
                // Lógica para avanzar a la siguiente sección
                const currentSection = getCurrentSection();
                const nextSection = getNextSection(currentSection);
                if (nextSection) scrollToSection(nextSection);
            } else if (e.key === 'ArrowLeft') {
                // Lógica para retroceder a la sección anterior
                const currentSection = getCurrentSection();
                const prevSection = getPrevSection(currentSection);
                if (prevSection) scrollToSection(prevSection);
            }
        });
        
        function getCurrentSection() {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                if (pageYOffset >= (sectionTop - 300)) {
                    current = section.getAttribute('id');
                }
            });
            return current;
        }
        
        function getNextSection(currentSection) {
            const sectionIds = Array.from(sections).map(s => s.id);
            const currentIndex = sectionIds.indexOf(currentSection);
            if (currentIndex < sectionIds.length - 1) {
                return sectionIds[currentIndex + 1];
            }
            return null;
        }
        
        function getPrevSection(currentSection) {
            const sectionIds = Array.from(sections).map(s => s.id);
            const currentIndex = sectionIds.indexOf(currentSection);
            if (currentIndex > 0) {
                return sectionIds[currentIndex - 1];
            }
            return null;
        }
    </script>
</body>
</html>
