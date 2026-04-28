# sistema-de-tareas-
sistema que recuerda tareas y hace tareas 

🤖 SISTEMA COMPLETO DE GESTOR DE TAREAS CON 7 AGENTES + GUI
Diego Mercedes Llauger (2026-0048)
Ingeniería en Ciberseguridad | Universidad Dominicano Americana  

📊 ANÁLISIS DE TU SOLICITUD
Entiendo que necesitas:
AgenteFunciónEntradaSalida
1. ParseadorConvierte texto → estructura"Trabajo urgente para el 25"JSON 
tarea
2. ValidadorVerifica datos completosTarea sin completarLista de errores/OK
3. AsignadorCalcula urgencia y metadatosTarea válidaTarea + urgencia/días
4. Generador PortadaCrea portada profesionalTarea + datos estudianteMD/PDF portada
5. ChatbotResponde preguntas sobre tareas"¿Cuándo entrego esto?"Respuesta natural
6. RecomendadorSugiere mejorar el trabajoTarea + descripciónSugerencias de mejora
7. Aprendizaje de DatosAnaliza patrones de tareasHistorial de tareasInsights y estadísticas
Almacenamiento:
Base de datos SQLite (mejor que JSON)

Interfaz: GUI con Tkinter (simple, sin dependencias externas)

Calendario: Integración visual de fechas límite


🏗️ ARQUITECTURA DEL SISTEMA COMPLETO

┌─────────────────────────────────────────────────────────┐
│               GUI PRINCIPAL (Tkinter)                   │
│  ┌──────────────┬──────────────┬──────────────┐         │
│  │ Crear Tarea  │ Ver Tareas   │ Ver Portada  │         │
│  │ Calendario   │ Estadísticas │ Chatbot      │         │
│  └──────────────┴──────────────┴──────────────┘         │
└────────┬────────────────────────────────────┬────────────┘
         │                                    │
    ┌────▼────────────────────────────────────▼────┐
    │        ORQUESTADOR (gestor_tareas.py)        │
    │  Coordina los 7 agentes                      │
    └────┬──────────────────────────────────────────┘
         │
    ┌────▼──────────────────────────────────────────┐
    │           7 AGENTES ESPECIALIZADOS            │
    │                                               │
    │  1. Parseador      → Texto → Estructura      │
    │  2. Validador      → Verifica datos          │
    │  3. Asignador      → Calcula urgencia        │
    │  4. Generador      → Crea portadas           │
    │  5. Chatbot        → Responde preguntas      │
    │  6. Recomendador   → Mejora trabajos         │
    │  7. Aprendizaje    → Analiza patrones        │
    │                                               │
    └────┬──────────────────────────────────────────┘
         │
    ┌────▼────────────────────────────────────────┐
    │     BASE DE DATOS SQLite (datos.db)         │
    │  ┌─────────────┬──────────────┬────────┐   │
    │  │ Estudiantes │ Tareas       │ Logs   │   │
    │  │ Asignaturas │ Recomendaciones      │   │
    │  └─────────────┴──────────────┴────────┘   │
    └────────────────────────────────────────────┘


Autor: Diego Mercedes Llauger (2026-0048)
Carrera: Ingeniería en Ciberseguridad | UNICDA
Fecha: 27 de Abril de 2026

