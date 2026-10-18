# 1 · Diagnóstico: el problema no es la edad, es la confianza para pagar digital

**Recomendación:** intervenir con una apuesta pequeña y reversible. Proponemos un servicio de valor agregado para emisores, la *Red de Confianza*, y validarlo con un piloto antes de escalar.

**La oportunidad (datos verificados)**
- 8,0 M de personas de 60+ en Colombia (≈15,5% de la población, DANE). En 2036 habrá más personas de 60+ que menores de 15 años.
- 2,11 M de pensionados reciben su mesada en una cuenta (SFC, 2024). Otros 1,6 M reciben Colombia Mayor, con meta de 3,1 M en el pilar solidario.
- La población de 50+ consume ≈ COP 121 billones al año (≈12% del PIB, 2023).

**El problema que vale la pena resolver**
- Tienen ingresos estables, pero pagan en efectivo y desconfían de lo digital.
- Solo el 18,1% de las personas de 65+ usaba internet con regularidad (DANE, 2021), así que el "68%" del caso no se sostiene. Los 65+ son además el grupo con menor uso de depósitos (RIF 2024).
- Son el blanco principal del fraude por ingeniería social, y Bre-B (pagos inmediatos e irrevocables) amplía el riesgo. Hoy delegan de forma informal: comparten la clave y la tarjeta.

**¿Quién es el cliente?**
- Paga y decide: el emisor (banco o billetera), a través del VP de tarjetas y el área de riesgo de fraude.
- Usan: la persona de 60+ y su familiar o cuidador.
- Distribuye: el emisor, por su app, sus oficinas y su línea telefónica.
- También gana: el comercio, que vende más con tarjeta.

**Segmento priorizado: "60+ bancarizado en transición digital".** Personas de 60 a 74 años con tarjeta débito donde reciben su pensión o ingreso, que todavía usan efectivo, y su cuidador (30 a 59 años). Quedan para una segunda fase las personas de 75+ dependientes y las no bancarizadas.

---

# 2 · Estrategia: ser la capa de confianza del ecosistema, no un banco para mayores

**Propuesta de valor**
- **Persona de 60+:** "paga digital con autonomía y con alguien de confianza cerca".
- **Familiar o cuidador:** "tranquilidad sin quitarle el control".
- **Emisor:** "menos fraude y más uso de las cuentas de tus clientes 60+, sin tener que construirlo".

**Posicionamiento:** para los emisores que quieren retener y activar a sus clientes de 60+, la Red de Confianza es el servicio de la red de pagos que reduce el fraude y activa el uso digital con un círculo familiar consentido. A diferencia de los desarrollos de cada banco, funciona sobre la red y se activa sin desarrollos pesados.

**Alternativas evaluadas** (puntaje ponderado de 1 a 5; detalle en el Anexo C)

| Alternativa | Puntaje | Decisión |
|---|---|---|
| Servicio de valor agregado para emisores (Escudo + Círculo) | **4,45** | **Hacer ahora** |
| Modo Senior en datáfono y Tap to Phone | 3,10 | Fase 2 |
| Alianza con aseguradora (seguro contra fraude) | 3,00 | Fase 2 |
| Analítica "Silver" para comercios | 2,90 | No por ahora: la red no conoce la edad del tarjetahabiente |
| Dispersión de subsidios del pilar solidario | 2,80 | Monitorear: depende del Gobierno |
| Billetera B2C para mayores | 2,25 | No: compite con nuestros clientes |
| No intervenir | — | Descartado: el problema está validado y el riesgo se acota con el piloto |

**Trade-offs**
- Escala vía emisores vs. control de la experiencia final.
- Reglas explicables vs. IA más precisa.
- Protección vs. autonomía de la persona mayor.
- Rapidez (empezar con 60–74 bancarizados) vs. mayor necesidad social (75+).

**Qué haríamos:** un servicio *white-label* con consentimiento explícito, canal asistido y un piloto con grupo de control.
**Qué no haríamos:** actuar como banco o aseguradora, vender B2C, dar al cuidador acceso al dinero o a la clave, usar IA sin una línea base ni crear hardware nuevo en la fase 1.

---

# 3 · Solución: la Red de Confianza, dos módulos sobre la infraestructura actual

**Módulo 1 · Escudo Senior** (aplica a todas las tarjetas que el emisor marque como 60+)
- Reglas de fraude ajustadas a los patrones de las personas de 60+, aplicadas en la autorización.
- Verificación por WhatsApp o llamada antes de declinar una transacción.
- Bloqueo inmediato con un solo botón.

**Módulo 2 · Círculo de Confianza** (opcional, la persona se inscribe)
- La persona mayor elige 1 o 2 personas de confianza, que reciben alertas en tiempo real.
- Límites configurables: monto diario y compras en línea activadas o desactivadas.
- Co-aprobación de compras en línea de alto riesgo mediante 3-D Secure.
- La persona puede revocar el permiso cuando quiera. El cuidador nunca ve la clave ni mueve dinero.

**Customer journey**
1. **Descubre:** el banco le ofrece el servicio en la oficina o por llamada, el día de pago de la mesada.
2. **Se inscribe:** con ayuda de un asesor o un familiar, en 5 minutos y con consentimiento grabado.
3. **Paga:** en datáfono, Tap to Phone o en línea.
4. **Queda protegido:** recibe una alerta o verificación y su familiar queda informado.
5. **Resuelve:** a través de una línea humana o bloqueando con un clic.

**Experiencia:** digital (WhatsApp y la app del banco, con letra grande, lenguaje simple y voz) y asistida (oficina, corresponsal y línea humana). Cumple el estándar de accesibilidad WCAG 2.2 AA.

**Seguridad y confianza:** PCI DSS, tokenización, consentimiento según la Ley 1581 de 2012 y registro de auditoría. Para evitar el abuso por parte del cuidador, la persona mayor recibe copia de todo y una alerta si el cuidador cambia los límites.

**Tecnología y datos**
- Se apoya en el switch de autorización y el motor de reglas actuales.
- Nuevo: API de inscripción para emisores, servicio de notificaciones y portal del cuidador.
- La IA queda para la fase 2, solo si las reglas no alcanzan las metas de fraude y de falsos positivos.

---

# 4 · Validación y roadmap: aprender antes de escalar, 12 meses y 3 decisiones

**Hipótesis y umbrales de éxito**
- **H1 (persona mayor):** al menos el 20% de los invitados se inscribe en el Círculo con canal asistido.
- **H2 (cuidador):** al menos el 60% activa las alertas y sigue activo a los 60 días.
- **H3 (valor):** frente al grupo de control, 30% menos fraude y 10% más pagos con tarjeta.
- **H4 (disposición a pagar):** al menos 2 de 5 emisores firman una carta de intención con precio de COP 200 o más por tarjeta.
- **H5 (viabilidad):** integración en 8 semanas o menos y falsos positivos de 2% o menos.

**MVP:** Escudo con 5 reglas y Círculo con alertas por WhatsApp y límites, con inscripción asistida. Se prueba con 1 emisor y 5.000 tarjetas de 60+, más un grupo de control, durante 12 semanas.

**North Star:** porcentaje de personas inscritas que hacen 4 o más pagos digitales al mes.

**Kill criteria (cuándo abandonar)**
- Menos del 10% de inscripción a las 8 semanas.
- Fraude menos de 10% por debajo y uso menos de 5% por encima del grupo de control.
- Ningún emisor dispuesto a pagar.
- Más del 0,5% de casos de abuso del rol del cuidador.

| Mes | Fase | Gate de decisión |
|---|---|---|
| 1–2 | Discovery: 30 personas mayores, 15 cuidadores, 6 emisores; datos de fraude y revisión jurídica | 2 o más cartas de intención |
| 3–4 | Diseño accesible y MVP | 80% o más completa las tareas en las pruebas de usabilidad |
| 5–7 | Piloto con grupo de control | Kill criteria |
| 8–9 | Lanzamiento con 2 o 3 emisores | Precio validado |
| 10–12 | Escalamiento: Bre-B, programa "Comercio amigable" y alianza con aseguradora | Metas de adopción |

**Dependencias:** datos de edad y de fraude del emisor, proveedor 3-DS, WhatsApp Business, área jurídica y franquicias.
**Riesgos:** baja adopción B2B, abuso del cuidador, falsos positivos y competencia con Bre-B por prioridad interna.
**Capacidades:** un squad de 7 personas (PO, UX accesible, 3 desarrolladores, analista de fraude y analista de datos), más jurídico, ventas *key account* y CX.

---

# 5 · Business case: Aprobado con condiciones

**Mercado (COP, base 2025):** TAM de 8,0 M de personas de 60+, SAM de 3,5 M con tarjeta activa y SOM de 1,4 M tarjetas en emisores clientes. Se espera que en el año 3 haya 560.000 tarjetas cubiertas por el Escudo y 78.400 inscritas en el Círculo.

**Quién paga:** el emisor. Escudo: COP 250 por tarjeta al mes. Círculo: COP 1.200 por tarjeta inscrita al mes. A esto se suma el 0,20% del gasto incremental procesado.

| COP millones · 3 años | Conservador | Base | Optimista |
|---|---|---|---|
| Ingresos año 3 | 975 | 2.978 | 5.714 |
| EBITDA año 3 | (58) | 1.586 | 3.863 |
| Margen EBITDA año 3 | −6,0% | 53,3% | 67,6% |
| Inversión inicial | 920 | 800 | 720 |
| ROI a 3 años | −172% | **149%** | 651% |
| VAN @15% | (1.326) | **633** | 3.071 |
| Payback | > 36 meses | **27 meses** | 18 meses |

**Punto de equilibrio:** 168.000 tarjetas cubiertas (12% del SOM). Precio mínimo del Escudo para que el VAN sea 0: COP 169 al mes. El VAN esperado, ponderando los escenarios 25/50/25, es de COP 753 M.

**Impacto adicional (no incluido en el ROI):** retención de emisores, argumento para atraer nuevos (cooperativas y billeteras) y venta cruzada de antifraude y Bre-B. Para el emisor, el valor estimado es ≈1,4 veces el precio, más la retención de las mesadas.

**Decisión:** aprobar ≈COP 850 M para discovery, MVP y piloto, que es la pérdida máxima acotada. El escalamiento se decide en el mes 7 según los kill criteria. La variable más sensible es cuántos emisores firman, y es lo primero que se valida.

---

# Anexo A · Validación de los datos del caso

| Enunciado del caso | Clasificación | Qué encontramos y cómo lo tratamos |
|---|---|---|
| 166 M de personas de 50+ en ALC (2024) y ~280 M en 2050 | Requiere contrastación | 2050: cobertura del Grupo Banco Mundial (2026) habla de más de 280 M (≈40%). 2024: no hallamos la fuente primaria. Se usa solo como contexto. |
| ALC envejece más rápido; Colombia y Brasil en "envejecimiento avanzado" según UN WPP | Parcialmente incorrecto | La clasificación es de CEPAL y ubica a Colombia en envejecimiento moderado pero acelerado. Corregido. |
| AARP: el 50+ es el 34% del PIB mundial (US$45 billones) en 2022 | Hecho con error de fecha | Las cifras son de 2020 (informe de noviembre de 2022). Dato global, solo contexto. |
| Las personas mayores son mejores pagadoras (Banco Mundial) | Interpretación no verificada | Sin fuente primaria. No se usa, porque el crédito no es nuestro rol. |
| 52% sin ahorros suficientes para la vejez (WEF) | No verificado | Se reemplaza por CEPAL 2023: 43,4% de los 65+ sin pensión o con pensión bajo la línea de pobreza. |
| DANE: 60+ = persona mayor (Ley 1251 de 2008); 7,1 M (13,9%) en 2021 | Hecho verificado | Es la base de la segmentación y del TAM. |
| 68% de las personas de 60+ usa banca móvil o billeteras | Contradicho | DANE: 36,4% de los 65+ con acceso a internet y 18,1% con uso regular. Se descarta, y explica por qué la solución es asistida. |

**Método:** cada dato se clasificó como hecho, dato a contrastar, supuesto, hipótesis o interpretación, se buscó su fuente primaria y se decidió si entraba al business case.

---

# Anexo B · Evidencia, fuentes y preguntas abiertas (consulta: 18 de octubre de 2026)

| Dato | Fuente |
|---|---|
| 7,1 M de personas de 60+ (13,9%) en 2021; ≈15,5% en 2024 | DANE, nota estadística sobre personas mayores |
| 36,4% de los 65+ con acceso a internet; 18,1% con uso regular | DANE 2021, citado por la Alcaldía de Bogotá |
| Los 65+ tienen el menor uso de depósitos; acceso total a depósitos de 96,5% (2025) | Banca de las Oportunidades y SFC, RIF 2024 y 2025 |
| 2.111.953 pensionados | SFC, 2024 |
| 1,6 M de beneficiarios de Colombia Mayor; meta de 3,1 M en el pilar solidario | Prosperidad Social, 2025 |
| El efectivo es ≈78% de las transacciones | Banco de la República, encuesta de instrumentos de pago |
| 50,2 M de tarjetas débito y 16,7 M de crédito | SFC, 2025 |
| Credibanco: COP 130 billones procesados en 2024, ~300.000 puntos de acceso, integrado a Bre-B | Portafolio y Valora Analitik |
| Bre-B: más de 500 M de transacciones en 5 meses | El Tiempo (ACI Worldwide) |
| La población de 50+ consume ≈ COP 121 billones al año | La República y Portafolio, 2023 |
| Las llamadas fraudulentas afectan sobre todo a adultos mayores | Banco de Bogotá, citado por Portafolio |

**Datos que no pudimos confirmar:** fraude por edad en Colombia, participación de Credibanco en el procesamiento de emisores y la disposición a pagar de los bancos. Son las primeras preguntas del discovery.

**Preguntas que haríamos al comité:**
1. ¿Qué participación tiene Credibanco en el procesamiento de los emisores?
2. ¿Hay datos de fraude por rango de edad?
3. ¿Cuál es el apetito para vender servicios de valor agregado a emisores?
4. ¿Qué capacidades tiene hoy el motor antifraude?
5. ¿Hay relación con proveedores de 3-DS y WhatsApp Business?
6. ¿Cuál es el umbral de inversión que se puede aprobar sin pasar por la junta?

---

# Anexo C · Segmentación, tamaño de mercado y priorización

**¿Por qué 60+ y no 50+?** Las personas de 50 a 59 años pagan igual que la población activa. Las necesidades distintas (brecha digital, fraude, dependencia de cuidadores) aparecen desde los 60. Además, 60+ es la definición legal (Ley 1251 de 2008) y la que usa el DANE, lo que permite medir de forma consistente.

| Nivel | Definición | Cifra | Tipo |
|---|---|---|---|
| TAM | Personas de 60+ en Colombia (2025) | 8,0 M | Dato (DANE) |
| SAM | 60+ con tarjeta débito o crédito activa | 3,0 / 3,5 / 4,0 M | Supuesto anclado en 2,11 M pensionados |
| SOM | Tarjetas en emisores clientes de Credibanco | 1,05 / 1,40 / 1,60 M | Supuesto (35–40%) |
| Adopción año 3 | Tarjetas cubiertas por el Escudo | 262.500 / 560.000 / 800.000 | Supuesto (25–50% del SOM) |
| Adopción año 3 | Tarjetas inscritas en el Círculo | 26.250 / 78.400 / 144.000 | Hipótesis H1 (10–18%) |

**Subsegmentos:**
1. 60–74 años bancarizados (prioridad).
2. Cuidadores de 30 a 59 años (usuarios del Círculo).
3. 75+ dependientes (fase 2).
4. No bancarizados con subsidio (fase 2, vía alianza).

**Matriz de priorización de alternativas**

Pesos de los criterios: valor para el usuario 25%, disposición a pagar B2B 25%, ajuste con las capacidades actuales 20%, tiempo a mercado 15% y riesgo bajo 15%.

| Alternativa | Usuario | Pago B2B | Capacidades | Tiempo | Riesgo | Total |
|---|---|---|---|---|---|---|
| Servicio para emisores (Escudo + Círculo) | 5 | 4 | 5 | 4 | 4 | **4,45** |
| Modo Senior en datáfono y Tap to Phone | 3 | 2 | 4 | 3 | 4 | 3,10 |
| Alianza con aseguradora | 3 | 3 | 3 | 3 | 3 | 3,00 |
| Analítica "Silver" para comercios | 2 | 3 | 3 | 4 | 3 | 2,90 |
| Dispersión de subsidios del pilar solidario | 4 | 3 | 3 | 1 | 2 | 2,80 |
| Billetera B2C para mayores | 4 | 1 | 2 | 2 | 2 | 2,25 |

**Marcos usados:** Double Diamond, Jobs to be Done, Opportunity Solution Tree, matriz ponderada, Lean Startup (experimentos con umbral de éxito) y piloto con grupo de control.

---

# Anexo D · Roles, arquitectura de referencia y riesgos

| Actor | Rol | Qué gana |
|---|---|---|
| Persona de 60+ | Usuario principal | Seguridad y autonomía |
| Familiar o cuidador | Usuario secundario | Tranquilidad y visibilidad |
| Emisor (banco o billetera) | Cliente: paga, decide y distribuye | Menos fraude, más uso y retención de mesadas |
| Comercio | Beneficiario | Más ventas con tarjeta |
| Credibanco | Proveedor de la red | Ingresos por servicios de valor agregado, retención de emisores y nuevas transacciones |

**Arquitectura de referencia**

| Componente | Propósito | Dependencia |
|---|---|---|
| Switch de autorización y motor de reglas (existente) | Aplicar las reglas del Escudo y los límites del Círculo en tiempo real | Que el emisor procese con Credibanco o comparta eventos |
| API de inscripción y consentimiento (nueva) | Que el emisor marque las tarjetas de 60+ e inscriba al cuidador | Integración con la app o el core del emisor |
| Servicio de notificaciones (nuevo) | Alertas y verificaciones por WhatsApp y SMS | Proveedor de WhatsApp Business |
| EMV 3-D Secure | Co-aprobación de compras en línea | Proveedor del ACS del emisor |
| Portal del cuidador (web ligera) | Ver alertas, ajustar límites y bloquear | Autenticación fuerte |
| Datos y auditoría (tokenizados, PCI DSS) | Medir el piloto y trazar los consentimientos | Ley 1581 de 2012 |

**Riesgos y mitigaciones**

| Riesgo | Mitigación |
|---|---|
| Los emisores no pagan | Piloto gratuito con métricas de fraude y uso; precio basado en valor |
| Abuso económico por parte del cuidador | Consentimiento revocable, copia de todo a la persona mayor, el cuidador no mueve dinero y alertas de cambios |
| Falsos positivos que frustran a la persona mayor | Verificación antes de declinar; meta de falsos positivos de 2% o menos |
| Regulatorio y de datos personales | Revisión de la Ley 1581 de 2012 y de las normas de la SFC en el discovery; privacidad desde el diseño |
| Prioridad interna frente a Bre-B | Integrarlo como capa de protección también para Bre-B en la fase 2 |

---

# Anexo E · Business case: supuestos, resultados y sensibilidad (COP)

| Supuesto | Valor | Lógica y forma de validarlo |
|---|---|---|
| Personas de 60+ con tarjeta activa (SAM) | 3,5 M | Pensionados más bancarizados; validar con datos de emisores |
| Participación de emisores clientes de Credibanco | 40% | Sin dato público; validar con el área comercial |
| Cobertura del Escudo, años 1/2/3 | 5% / 25% / 40% del SOM | Ciclo de venta B2B de 6 a 9 meses |
| Inscripción en el Círculo, años 1/2/3 | 4% / 10% / 14% | Hipótesis H1 |
| Precio del Escudo y del Círculo | COP 250 y 1.200 por tarjeta al mes | Valor para el emisor ≈1,4–1,5 veces el precio (H4) |
| Gasto con tarjeta y aumento | COP 600.000 al mes; +15% | Hipótesis H3 |
| Ingreso neto sobre el gasto incremental | 0,20% | Validar con Finanzas |
| Costo variable | COP 50 (Escudo) y COP 400 (Círculo) por tarjeta al mes | Mensajes de WhatsApp y soporte |
| Inversión inicial | COP 800 M | Squad de ~7 meses, más legal, infraestructura y piloto |
| Costos fijos, años 1/2/3 | COP 270 / 640 / 680 M | Equipo de operación |
| Tasa de descuento | 15% | Validar con Finanzas |

**Metodología (igual en los 3 escenarios):** ROI = (Σ EBITDA de 3 años − inversión) / inversión. El VAN se calcula sobre los flujos netos a 3 años, sin valor terminal. El payback son los meses hasta que el flujo acumulado llega a 0. El año 1 equivale a los primeros 12 meses tras la aprobación, y el piloto no se cobra.

**Estado de resultados (COP millones)**

| Escenario base | Año 1 | Año 2 | Año 3 |
|---|---|---|---|
| Tarjetas cubiertas / inscritas | 70.000 / 2.800 | 350.000 / 35.000 | 560.000 / 78.400 |
| Ingresos totales | 85 | 1.630 | 2.978 |
| Costos variables | (18) | (378) | (712) |
| Costos fijos | (270) | (640) | (680) |
| EBITDA | (203) | 612 | 1.586 |
| Inversión | (800) | – | – |
| Flujo acumulado | (1.003) | (391) | 1.195 |

| Flujo neto por año | Año 1 | Año 2 | Año 3 | Acumulado |
|---|---|---|---|---|
| Conservador | (1.198) | (324) | (58) | (1.581) |
| Base | (1.003) | 612 | 1.586 | 1.195 |
| Optimista | (830) | 1.657 | 3.863 | 4.690 |

**Sensibilidad del VAN base (±20% en cada supuesto)**

| Supuesto | VAN con −20% | VAN con +20% |
|---|---|---|
| Cobertura de emisores | 134 | 1.132 |
| Precio del Escudo | 241 | 1.025 |
| Precio del Círculo | 406 | 860 |
| Inscripción en el Círculo | 448 | 818 |
| Costos fijos | 866 | 400 |

**Lectura:** el negocio depende de cuántos emisores firmen, más que de cuántas personas mayores se inscriban. Por eso el gate 1 exige cartas de intención.
