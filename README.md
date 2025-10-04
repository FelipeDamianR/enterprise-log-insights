# 📊 Enterprise Log Insights

Proyecto de análisis de bitácoras empresariales con **Python** a partir de archivos **Parquet**.  
Se identificaron concentraciones de errores críticos, patrones de fallos por país, usuarios con comportamientos atípicos y posibles automatizaciones sospechosas.

---

## ⚙️ Tecnologías usadas
- Python 3  
- Librerías: pandas, numpy, matplotlib, seaborn, os, ast, json, re  
- Archivos Parquet para datos

---

## 🚀 Principales hallazgos
1. **Errores críticos concentrados en pocos usuarios**  
   - Solo 5 usuarios generaron los 22,525 errores más graves.  
   - En algunos casos, un único usuario provocó más de 16,000 fallos repetidos.  

2. **Errores diferenciados por país**  
   - 🇲🇽 México → fallas en la lógica de negocio.  
   - 🇬🇧 Reino Unido → errores de interoperabilidad y estructuras de datos.  
   - 🇺🇸 Estados Unidos → fallas en la interfaz y experiencia de usuario.  
   - Aunque México tuvo más errores en total, EE. UU. presentó la mayor proporción de fallas graves.  

3. **Usuarios con alta diversidad de errores**  
   - Algunos usuarios generaron hasta **68 tipos distintos de errores**.  
   - Esto apunta a configuraciones incorrectas, mal uso o entornos específicos problemáticos.  

4. **Posible automatización / anomalías**  
   - Un usuario acumuló más de **1 millón de registros**, con operaciones nocturnas repetitivas.  
   - Indicios de procesos automatizados o scripts no supervisados.  

5. **Métodos raramente usados**  
   - Algunos métodos fueron ejecutados miles de veces, pero por muy pocos usuarios.  
   - Este comportamiento es relevante para **seguridad y auditoría**.  

---

## 📈 Impacto empresarial
- Permite focalizar acciones correctivas en **usuarios específicos**.  
- Detecta **riesgos de seguridad y mantenimiento** por automatizaciones no documentadas.  
- Ofrece una visión **geográfica y por roles** para priorizar soporte técnico y auditorías.  

---

## 👥 Autores
- Felipe de Jesús Damián Rodríguez  
- Gabriela Marissa Mosquera  
- Humberto Mondragón García  
---
