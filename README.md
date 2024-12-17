# 🏥 Modelado y Simulación de Sistemas de Salud con NetLogo

**Autores:** Diego Encinas, Verónica Scholz  
**Institución:** Instituto de Ingeniería y Agronomía, UNAJ  
**Fecha:** 2023

---

## 📘 **Introducción**

Las infecciones intrahospitalarias representan una de las principales amenazas para pacientes hospitalizados debido a la interacción entre pacientes, personal de salud y el medio ambiente. Este proyecto desarrolla una simulación en **NetLogo** utilizando el **paradigma basado en agentes** para evaluar el impacto de posibles medidas de control y optimización en un entorno hospitalario.

---

## ⚙️ **Descripción del Proyecto**

Se implementó un modelo simplificado de flujo de pacientes en una sala de guardia hospitalaria con las siguientes características:

1. **Agentes (Pacientes):**
   - **Energía (`energy`)**: Representa el nivel de salud, disminuye con el tiempo si no se recibe atención médica.
   - **Carga Viral (`viral`)**: Representa la exposición al virus al moverse por áreas infectadas.

2. **Entorno:**
   - La sala de espera y el triaje se modelan con cuadrantes específicos.
   - Los agentes acumulan carga viral al interactuar con áreas infectadas (parches rojos).

3. **Simulación del Proceso:**
   - Los pacientes llegan al triaje después de cierto número de `ticks`.
   - Se clasifican en **crítico**, **urgente** o **moderado** según su condición de salud.

![Imagen de la simulación en NetLogo](https://github.com/veroyols/netlogo/blob/main/netlogo.png)

---

## 🎯 **Objetivos**

- ✅ Analizar la infraestructura de sistemas de salud y representar una versión gráfica simplificada.
- ✅ Simular el flujo de pacientes y propagación de enfermedades en un servicio de urgencias.
- ✅ Implementar agentes que interactúan con el entorno y entre sí, variando su carga viral.

---

## 📝 **Actividades Desarrolladas**

- Adaptación del tutorial *Wolf-Sheep Predation* de NetLogo.
- Implementación de un modelo simplificado del flujo de pacientes.
- Simulación de las siguientes propiedades de los pacientes:
  - **Energía:** Se reduce con el tiempo.
  - **Carga Viral:** Aumenta al moverse por áreas infectadas.
- Clasificación de pacientes en el triaje según su estado de salud.

---

## 📊 **Resultados Obtenidos**

- Simulación de distintos escenarios al modificar parámetros iniciales.
- Evaluación de métricas como:
  - **Tiempo de espera**.
  - **Energía de los pacientes**.
  - **Capacidad del personal médico**.
- Identificación de **cuellos de botella** en situaciones de alta demanda.

---

## 🚧 **Obstáculos**

- Definición y desarrollo de máquinas de estados para modelar el proceso de:
  - **"Esperando atención"**
  - **"Siendo evaluado"**
  - **"Recibiendo tratamiento"**
- Modularización del comportamiento de los agentes y definición de parámetros clave.

---

## 📚 **Bibliografía**

1. **NetLogo:** [NetLogo Documentation](https://ccl.northwestern.edu/netlogo/)  
2. **Teoría de Colas:** Llano Monelos, P. de (1997). Aplicabilidad de la teoría de colas al fenómeno hospitalario. [Repositorio](http://hdl.handle.net/2183/18274)  
3. **SimHPC:** Encinas, D., et al. (2024). Enfoques de modelado y simulación en sistemas de HPC y Aplicaciones en Salud. XXVI WICC 2024.

---

## 🚀 **Ejecutar el Proyecto**

1. **Instalar NetLogo:**  
   [NetLogo Download](https://ccl.northwestern.edu/netlogo/download.shtml).

2. **Abrir el Archivo:**  
   `simulacion.nlogo` 

3. **Ejecutar la Simulación:**  
   Clic en `Setup` y luego en `Go` para iniciar la simulación.
