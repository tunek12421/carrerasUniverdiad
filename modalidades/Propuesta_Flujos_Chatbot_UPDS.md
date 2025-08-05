# 🤖 Propuesta de Flujos para Chatbot UPDS - Chatfuel

## 📊 Análisis del Sistema Actual

| Característica | Valor |
|----------------|-------|
| **Límite de tokens** | 12,000 |
| **Reglas máximas** | 10 (actualmente 2/10 utilizadas) |
| **Funcionalidad** | Redirección a flujos específicos |
| **Estructura** | Base de conocimientos + Reglas |

---

## 🎯 Flujos Principales Propuestos

### 1. 🎓 **FLUJO_INFORMACION_CARRERAS**

**Reglas de activación:**
- Usuario pregunta sobre carreras disponibles
- Usuario menciona nombres específicos de carreras
- Usuario busca información de planes de estudio
- Usuario consulta sobre duración de carreras

**Palabras clave:** `"carrera"`, `"estudiar"`, `"qué carreras"`, `"plan de estudios"`, `"cuánto dura"`

**Subcategorías:**
- → `Flujo_Carreras_Ingenieria`
- → `Flujo_Carreras_Salud`  
- → `Flujo_Carreras_Empresariales`
- → `Flujo_Carreras_Sociales`

---

### 2. 📚 **FLUJO_MODALIDADES_ESTUDIO**

**Reglas de activación:**
- Usuario pregunta sobre modalidades
- Usuario consulta presencial vs semipresencial
- Usuario busca flexibilidad de horarios
- Usuario pregunta sobre estudiar trabajando

**Palabras clave:** `"modalidad"`, `"presencial"`, `"semipresencial"`, `"virtual"`, `"horarios"`, `"trabajar y estudiar"`

**Respuestas automatizadas:**
- ✅ Explicación modalidad presencial
- ✅ Ventajas modalidad semipresencial
- ✅ Comparación entre modalidades
- ✅ Público objetivo cada modalidad

---

### 3. 📝 **FLUJO_ADMISIONES_INSCRIPCIONES**

**Reglas de activación:**
- Usuario pregunta sobre requisitos de inscripción
- Usuario consulta proceso de admisión
- Usuario busca documentos necesarios
- Usuario pregunta fechas de inscripción

**Palabras clave:** `"inscribirse"`, `"requisitos"`, `"documentos"`, `"admisión"`, `"inscripción"`

**Información automatizada:**
- 📋 Lista de documentos requeridos
- 🔄 Proceso paso a paso
- 📅 Fechas importantes
- 📞 Contactos de admisiones

---

### 4. 💰 **FLUJO_BECAS_FINANCIAMIENTO**

**Reglas de activación:**
- Usuario consulta sobre becas
- Usuario pregunta ayuda económica
- Usuario busca financiamiento
- Usuario menciona "no tengo dinero"

**Palabras clave:** `"beca"`, `"ayuda económica"`, `"financiamiento"`, `"costo"`, `"precio"`, `"pagar"`

**Redirección:** → `Flujo_Plataforma` (ya existente)

---

### 5. 📍 **FLUJO_SEDES_UBICACIONES**

**Reglas de activación:**
- Usuario pregunta sobre sedes
- Usuario consulta ubicaciones
- Usuario busca direcciones
- Usuario pregunta "dónde está"

**Palabras clave:** `"sede"`, `"ubicación"`, `"dirección"`, `"dónde"`, `"campus"`

**Información automatizada:**
- 🏢 Lista de 8 sedes principales
- 📍 Direcciones específicas
- 🎓 Carreras por sede
- 📞 Contactos por ubicación

---

### 6. 🤝 **FLUJO_BIENESTAR_ESTUDIANTIL**

**Reglas de activación:**
- Usuario pregunta sobre apoyo estudiantil
- Usuario consulta servicios de bienestar
- Usuario busca ayuda académica
- Usuario menciona problemas personales

**Palabras clave:** `"bienestar"`, `"apoyo"`, `"ayuda"`, `"psicológico"`, `"académico"`, `"problemas"`

**Información automatizada:**
- 🏥 Servicios disponibles
- 📞 Contacto: +591 65366933
- 📧 Email: rondal.perez@upds.edu.bo
- 🎯 Programas de apoyo

---

### 7. 🎉 **FLUJO_GRADUACION_TITULACION**

**Reglas de activación:**
- Usuario pregunta sobre graduación
- Usuario consulta modalidades de grado
- Usuario busca requisitos de titulación
- Usuario pregunta sobre tesis

**Palabras clave:** `"graduarse"`, `"título"`, `"tesis"`, `"trabajo dirigido"`, `"examen de grado"`

**Información automatizada:**
- 🏆 5 modalidades de graduación
- ✅ Requisitos específicos
- ⏱️ Procesos y tiempos
- 📄 Documentación necesaria

---

### 8. ⏰ **FLUJO_HORARIOS_CALENDARIOS**

**Reglas de activación:**
- Usuario pregunta sobre horarios
- Usuario consulta calendarios académicos
- Usuario busca fechas de exámenes
- Usuario pregunta turnos disponibles

**Palabras clave:** `"horario"`, `"calendario"`, `"cuándo"`, `"fechas"`, `"turnos"`

---

### 9. 📞 **FLUJO_CONTACTOS_INFORMACION**

**Reglas de activación:**
- Usuario busca números de teléfono
- Usuario consulta emails
- Usuario pregunta "cómo contactar"
- Usuario busca información específica

**Palabras clave:** `"teléfono"`, `"contacto"`, `"email"`, `"información"`, `"hablar con"`

---

### 10. 💳 **FLUJO_PAGOS_ARANCELES**

**Reglas de activación:**
- Usuario pregunta sobre pagos
- Usuario consulta aranceles
- Usuario busca costos
- Usuario menciona "cuánto cuesta"

**Palabras clave:** `"pagar"`, `"costo"`, `"precio"`, `"arancel"`, `"cuánto cuesta"`

**Redirección:** → `Flujo_Cajas` (ya existente)

---

## ⚙️ Estructura Técnica Recomendada

### 🔄 Reglas de Prioridad:
1. **Palabras clave específicas** (nombres de carreras)
2. **Intenciones generales** (información, costos, ubicación)
3. **Consultas de apoyo** (bienestar, ayuda)
4. **Redirecciones a departamentos** (cajas, plataforma)

### 💡 Optimización de Tokens:
- ✅ Respuestas concisas pero completas
- ✅ Información esencial por flujo
- ✅ Enlaces a información detallada
- ✅ Botones de navegación rápida

### 📋 Flujos Secundarios Sugeridos:
- `Flujo_Intercambios_Internacionales`
- `Flujo_Practicas_Profesionales`  
- `Flujo_Biblioteca_Recursos`
- `Flujo_Actividades_Extracurriculares`
- `Flujo_Egresados_Alumni`

---

## 🚀 Implementación Progresiva Sugerida

### 📈 **FASE 1** (Inmediata - 4 flujos):
1. ✅ `Flujo_Informacion_Carreras`
2. ✅ `Flujo_Modalidades_Estudio`
3. ✅ `Flujo_Admisiones_Inscripciones`
4. ✅ Mantener `Flujo_Cajas` y `Flujo_Plataforma` existentes

### 📈 **FASE 2** (Expansión - 3 flujos adicionales):
5. ✅ `Flujo_Graduacion_Titulacion`
6. ✅ `Flujo_Sedes_Ubicaciones`
7. ✅ `Flujo_Bienestar_Estudiantil`

### 📈 **FASE 3** (Completar - 3 flujos finales):
8. ✅ `Flujo_Horarios_Calendarios`
9. ✅ `Flujo_Contactos_Informacion`
10. ✅ Optimización y ajustes según uso

---

## 🎯 Ventajas del Sistema Propuesto

| Ventaja | Beneficio |
|---------|-----------|
| 📊 **Cobertura** | 90% de consultas estudiantiles frecuentes |
| ⚡ **Eficiencia** | Reducción significativa de consultas manuales |
| 🕐 **Disponibilidad** | Respuestas inmediatas 24/7 |
| 📝 **Consistencia** | Información actualizada y consistente |
| 🎯 **Redirección** | Eficiente a departamentos específicos |
| 😊 **Experiencia** | Mejor experiencia del usuario |
| 💰 **Recursos** | Optimización de recursos humanos |
| 📈 **Análisis** | Datos para análisis de consultas frecuentes |

---

## 🔧 Mantenimiento y Actualización

### 📅 **Cronograma de Mantenimiento:**
- **Mensual:** Revisión de efectividad de flujos
- **Trimestral:** Actualización según cambios académicos
- **Semestral:** Análisis de nuevas consultas no cubiertas
- **Anual:** Optimización completa del sistema

### 🔍 **Actividades de Monitoreo:**
- ✅ Monitoreo de nuevas consultas no cubiertas
- ✅ Optimización de palabras clave según uso real
- ✅ Feedback de usuarios para mejoras
- ✅ Coordinación con departamentos académicos

---

## 📚 Base de Conocimientos Disponible

Esta propuesta se fundamenta en la información completa documentada:

### 🎓 **Carreras Documentadas (14):**
- Ingeniería Industrial
- Medicina
- Fisioterapia y Kinesiología
- Nutrición y Dietética
- Bioquímica y Farmacia
- Ciencias de la Comunicación Social
- Contaduría Pública
- Derecho
- Administración de Empresas
- Ingeniería de Sistemas
- Ingeniería en Gestión Petrolera
- Ingeniería Comercial
- Ingeniería en Redes y Telecomunicaciones
- Psicología

### 📋 **Información Adicional:**
- ✅ Modalidades de estudio detalladas
- ✅ Servicios de bienestar estudiantil
- ✅ Procesos de admisión y graduación
- ✅ Contactos y ubicaciones
- ✅ Planes de estudio completos

---

> **Nota:** Esta propuesta maximiza el uso de la información universitaria disponible para crear un sistema automatizado eficiente que mejore significativamente la experiencia del usuario y optimice los recursos institucionales.